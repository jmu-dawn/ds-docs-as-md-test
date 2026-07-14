---
title: Token Architecture
description: How DS3 organizes design tokens into three tiers, and why the semantic layer splits into separate files for color theming.
status: stable
nav_order: 1
---

DS3 uses a strict three-tier token architecture. Each tier has a defined role and a set of rules about what it can and cannot reference. Understanding the structure is essential before creating or modifying tokens.

## The three tiers

**The three token tiers of DS3**

```text
┌── Tier 3 — Component
│   └── component.json
│       Aliases semantic + other component tokens
│
│       ↑ aliases
│
├── Tier 2 — Semantic
│   ├── semantic.json
│   │   Spacing, border radius, typography
│   │   No color tokens
│   │
│   ├── light.json
│   │   Light theme color tokens
│   │
│   └── dark.json
│       Dark theme color tokens
│
│   light.json and dark.json are structurally identical.
│   Same token names, same hierarchy — only values differ.
│
│       ↑ aliases
│
└── Tier 1 — Core
    └── core.json
        Resolved values only (hex, px, rem)
        Never aliases anything
```

### Tier 1: Core

Core tokens hold every raw value in the system. Hex codes, pixel values, font sizes, numeric scales. Nothing in `core.json` references another token. It is the resolved source of truth.

**`tokens/base/core.json`**

```json
{
  "color": {
    "brand": {
      "primary": {
        "500": { "$type": "color", "$value": "#3d3e9f" }
      }
    },
    "global": {
      "gray": {
        "200": { "$type": "color", "$value": "#dfe2e7" }
      }
    }
  },
  "fontSizes": {
    "body": { "$type": "fontSizes", "$value": "16" }
  }
}
```

> **⚠️ Core tokens never alias**
>
> A core token that aliases another token is a hard violation. Core tokens must always contain resolved values.

### Tier 2: Semantic

Semantic tokens give meaning to raw values. They translate "gray 200" into "this is what a default border looks like." This is also where theming happens.

The semantic tier is split into three token sets:

| File            | Purpose                                                        |
| --------------- | -------------------------------------------------------------- |
| `semantic.json` | Spacing, border radius, typography, and other non-color tokens |
| `light.json`    | All color tokens for the light theme                           |
| `dark.json`     | All color tokens for the dark theme                            |

Semantic tokens can alias core tokens and other semantic tokens. They must never alias component tokens.

> **⚠️ No color tokens in semantic.json**
>
> Color tokens belong exclusively in `light.json` and `dark.json`. Putting a color token in `semantic.json` breaks the theming model.

### Tier 3: Component

Component tokens describe how specific UI components are styled. They primarily alias semantic tokens, and can also alias other component tokens. Direct references to core tokens are allowed only in rare, documented cases.

**`tokens/base/component.json`**

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

## The aliasing matrix

| Token tier    | Resolved values | Can alias Core | Can alias Semantic | Can alias Component |
| ------------- | --------------- | -------------- | ------------------ | ------------------- |
| **Core**      | Always          | Never          | Never              | Never               |
| **Semantic**  | Never           | Yes            | Yes                | Never               |
| **Component** | Rarely          | Rarely         | Yes                | Yes                 |

> **💡 Names are what get mapped, not values**
>
> Token names are what engineers map in code. Values can change freely without any dev work. Renaming a token breaks the mapping and costs engineering time. Always add tokens, never rename existing ones without a coordinated migration.

## The light and dark split

`light.json` and `dark.json` are structurally identical. They use the same token names and the same hierarchy. Only the values differ.

**`light.json`**

```json
{
  "color": {
    "action": {
      "brand": {
        "background": {
          "default": {
            "$type": "color",
            "$value": "{color.brand.primary.500}"
          },
          "hover": { "$type": "color", "$value": "{color.brand.primary.600}" },
          "pressed": { "$type": "color", "$value": "{color.brand.primary.700}" }
        }
      }
    },
    "neutralPalette": {
      "pure": { "$type": "color", "$value": "{color.global.neutral.white}" },
      "solid": { "$type": "color", "$value": "{color.global.neutral.black}" }
    }
  }
}
```

**`dark.json`**

```json
{
  "color": {
    "action": {
      "brand": {
        "background": {
          "default": {
            "$type": "color",
            "$value": "{color.brand.primary.400}"
          },
          "hover": { "$type": "color", "$value": "{color.brand.primary.500}" },
          "pressed": { "$type": "color", "$value": "{color.brand.primary.600}" }
        }
      }
    },
    "neutralPalette": {
      "pure": { "$type": "color", "$value": "{color.global.neutral.black}" },
      "solid": { "$type": "color", "$value": "{color.global.neutral.white}" }
    }
  }
}
```

Because the names match exactly, the build system can swap the entire color layer simply by activating a different theme file. Component tokens never need to change to support dark mode. They reference semantic names, and the semantic layer handles the rest.

## Token files and folders in the repository

Tokens Studio manages these files as token sets. The `$themes.json` file controls which sets are active per theme.

```text
tokens/
├── base/
│   ├── core.json
│   ├── semantic.json
│   └── component.json
├── mode/
│   ├── light.json
│   └── dark.json
├── web/
│   ├── core-web.json
│   ├── semantic-web.json
│   └── component-web.json
├── $themes.json
└── $metadata.json
```

The `web/` folder holds platform overrides for the web theme. These are layered on top of the base sets and can override values where web-specific behavior is needed, for example adjusted border radius scales or font size overrides.

## Themes and token set activation

`$themes.json` defines which token sets are active for each named theme. The `light` and `dark` themes each use the full base stack plus their respective mode file. The `web` theme uses base plus all three web sets.

**`tokens/$themes.json`**

```json
[
  {
    "name": "light",
    "selectedTokenSets": {
      "base/core": "source",
      "base/semantic": "enabled",
      "base/component": "enabled",
      "mode/light": "enabled"
    },
    "group": "mode"
  },
  {
    "name": "dark",
    "selectedTokenSets": {
      "base/core": "source",
      "base/semantic": "enabled",
      "base/component": "enabled",
      "mode/dark": "enabled"
    },
    "group": "mode"
  }
]
```

`source` means the set contributes tokens and can be referenced. `enabled` means the set is active and its tokens override earlier sets with the same name.

## Frequently asked questions

<details markdown="1">
<summary>Why can't semantic tokens alias component tokens?</summary>

The tier hierarchy is one-directional by design. Semantic tokens describe abstract meaning (surfaces, actions, states). Component tokens apply that meaning to specific UI elements. If semantic tokens could reference component tokens, the dependency graph would become circular, and changing a component token could break semantic tokens used across the entire system.
</details>

<details markdown="1">
<summary>When is it acceptable for a component token to alias core directly?</summary>

Rarely, and only when there is no semantic token that accurately represents the intent. When this happens, it must be documented in the token's `$description` field so the reasoning is visible in Tokens Studio. If you find yourself doing this often, it is a signal that the semantic layer is missing a token, not that direct core references are appropriate.
</details>

<details markdown="1">
<summary>Why are light and dark in separate files rather than a single semantic file?</summary>

A single file would require a mechanism to conditionally resolve values based on the active theme. Separate files let Tokens Studio and the build pipeline handle theming through set activation, which is simpler, less error-prone, and easier to audit. It also means the two themes can be diffed directly as files.
</details>

<details markdown="1">
<summary>What happens if I rename a token?</summary>

Any engineer who has mapped that token name in code will get a broken reference the next time they pull the updated token file. Token names are the contract between design and engineering. Adding new tokens is always safe. Renaming or removing existing ones requires a coordinated migration with engineering.
</details>
