---
title: Token Terminology
description: The vocabulary used to describe DS3's token system. Names, paths, values, aliases, and types.
status: stable
nav_order: 2
---

> **💡 Quick reference**
>
> **Token name** — dot-separated identifier, e.g. `button.color.primary.background.default`  
> **Path segment** — one part of that name, e.g. `button`, `color`, `default`  
> **Token** — an object with `$value`, `$type`, and optional metadata  
> **Alias** — a `$value` that points to another token by name  
> **Value** — can be primitive, alias, or composite

## Token name

A token name is a dot-separated string that uniquely identifies a token in the system.

`color.brand.primary.500`  
`dimension.12px`  
`borderRadius.md`  
`color.action.brand.background.default`  
`button.color.primary.background.hover`

Token names are made up of **path segments** and are used both to locate a token in the file structure and to reference it in aliases.

## Path segment

A path segment is a single part of a token name, everything between two dots.

```
button · color · primary · background · default
```

Each segment represents one level in the hierarchy. Segments don't carry fixed meaning on their own, meaning comes from context.

| Segment examples                          | What they typically represent |
| ----------------------------------------- | ----------------------------- |
| `button`, `container`, `listItem`         | Component scope               |
| `color`, `typography`, `padding`          | Property domain               |
| `primary`, `brand`, `md`                  | Variant or scale              |
| `default`, `hover`, `pressed`, `disabled` | Interaction state             |

Not all tokens include state segments. The final segment might be a state (`hover`), a variant (`primary`), a scale step (`500`, `md`), or just `default`. The meaning is always contextual, not enforced by the structure.

## Token

A token is an object that defines a value and its metadata. It lives at a specific token name in the file hierarchy.

Every token must include `$value`. It typically includes `$type`, and may include `$description`.

**`core.json`**

```json
"500": {
  "$type": "color",
  "$value": "#3d3e9f"
}
```

## Token structure

Tokens are nested in a hierarchy that mirrors their token name path. Each level of nesting corresponds to one path segment. The token itself lives at the final segment.

**`component.json`**

```json
{
  "button": {
    "color": {
      "primary": {
        "background": {
          "default": {
            "$type": "color",
            "$value": "{color.action.brand.background.default}"
          }
        }
      }
    }
  }
}
```

The token name for that object is `button.color.primary.background.default`.

## Value

The `$value` of a token can take three forms.

### Primitive

A raw, hardcoded value. Only core tokens should contain these.

**`core.json`**

```json
"500": {
  "$type": "color",
  "$value": "#3d3e9f"
}
```

A primitive can be a hex code, a pixel value, a font weight, or any other literal.

### Alias

A reference to another token by its token name. The full string is the alias, the value inside `{}` is the target token name.

**`light.json`**

```json
"default": {
  "$type": "color",
  "$value": "{color.action.brand.background.default}"
}
```

Aliases are how the semantic and component tiers point back at core values without duplicating them.

### Composite

A value made up of multiple properties. Can mix aliases and primitive values. Common for typography tokens.

**`semantic.json`**

```json
"default": {
  "$type": "typography",
  "$value": {
    "fontFamily": "{fontFamilies.bodyFamily}",
    "fontWeight": "{fontWeights.medium}",
    "fontSize": "{fontSizes.body}",
    "lineHeight": "24px"
  }
}
```

Each property inside the composite is itself either an alias or a primitive.

## Type

The `$type` property defines the token's type. DS3 follows Tokens Studio conventions for type names.

```
"$type": "color"
"$type": "dimension"
"$type": "fontWeights"
"$type": "typography"
```

### Singular vs. plural is deliberate

You'll see the same property written two ways depending on where it lives, and this is not a quirk or an inconsistency. Tokens Studio uses a specific syntax to distinguish a standalone property token from the same property used inside a composite.

A standalone font weight token uses the **plural** `fontWeights`:

**`core.json`**

```json
"medium": {
  "$type": "fontWeights",
  "$value": "500"
}
```

The same property referenced inside a Typography composite uses the **singular** `fontWeight`:

**`semantic.json`**

```json
"default": {
  "$type": "typography",
  "$value": {
    "fontWeight": "{fontWeights.medium}"
  }
}
```

> **💡 Why this matters at handoff**
>
> In the design-to-code pipeline, the SD-Transforms preprocessor automatically converts the Tokens Studio type `fontWeights` to the DTCG format type `fontWeight`. The two forms you see in the JSON are expected, not something to fix by hand.

## Composite typography properties

A Typography composite token can hold up to nine properties: `fontFamily`, `fontWeight`, `fontSize`, `lineHeight`, `letterSpacing`, `paragraphSpacing`, `paragraphIndent`, `textCase`, and `textDecoration`.

DS3 uses a subset. Our typography tokens define only `fontFamily`, `fontWeight`, `fontSize`, and `lineHeight`. The remaining properties are available in Tokens Studio but we don't apply them, so they won't appear in our token files.

## Core token naming

Core tokens hold the raw values that everything else references. Since core tokens cover very different kinds of values (dimensions, colors, font sizes), naming strategy varies by domain.

### Value-based

**Used for:** spacing, sizing, and layout primitives

The token name directly encodes the value.

**`core.json`**

```json
"12px": {
  "$type": "dimension",
  "$value": "12px"
}
```

This makes all primitive values centralized and easy to locate. `dimension.12px` means exactly what it says.

### Numeric scale

**Used for:** color ramps

Numbers represent steps in a scale, not literal values.

**`core.json`**

```json
"500": {
  "$type": "color",
  "$value": "#3d3e9f"
}
```

> **⚠️ Common misconception**
>
> `500` is not the value, it's a **position in a scale**. The scale runs from light to dark (e.g. `50` to `950`). The actual value is always the hex code.

### Semantic

**Used for:** typography and readability-related tokens

Names describe usage or intent rather than raw values.

**`core.json`**

```json
"medium": {
  "$type": "fontWeights",
  "$value": "500"
}
```

`fontWeights.medium` is more useful than `fontWeights.500`. The name conveys meaning, the value is just implementation detail.

### Naming strategy summary

| Strategy      | Example                   | When to use                       |
| ------------- | ------------------------- | --------------------------------- |
| Value-based   | `dimension.12px`          | Raw primitive values              |
| Numeric scale | `color.brand.primary.500` | Ordered systems (color ramps)     |
| Semantic      | `fontWeights.medium`      | Human-readable descriptive values |

> **💡 Core token rule**
>
> All core tokens contain raw values. All other tokens reference core tokens via aliases. Naming differences across types are intentional, they reflect different kinds of primitives, each with the naming approach that makes most sense for that domain.

## Common questions

<details markdown="1">
<summary>Why is the same font weight property sometimes fontWeights and sometimes fontWeight?</summary>

Tokens Studio writes the plural `fontWeights` for a standalone property token, and the singular `fontWeight` for that property inside a Typography composite. SD-Transforms normalizes the plural to the singular DTCG type during the export to code, so both forms are expected.
</details>

<details markdown="1">
<summary>Why does a numeric scale step like 500 not match the value?</summary>

Scale numbers are positions, not values. A ramp runs from light to dark (`50` to `950`) and the step number tells you where a color sits in that order. The resolved value is always the hex code stored on the token.
</details>

<details markdown="1">
<summary>Can a composite token mix aliases and primitives?</summary>

Yes. Each property inside a composite is independent, so some can reference other tokens while others hold a literal value. Our typography tokens do exactly this, aliasing font family, weight, and size while keeping line height as a primitive.
</details>
