---
title: Introduction
group: DS3 Tokens
nav_order: 1
---

LLM- and human-readable reference for the Dawn design system tokens, converted from the source Tokens Studio JSON (`tokens/`). Aliases are shown alongside their resolved values so you can answer questions without chasing references.

## Token layers

Tokens are layered. Each layer aliases the one(s) below it:

1. **Core** (primitives) — raw hex, px, font values. → [Core tokens]({{ '/docs/tokens/DS3-tokens/core/' | relative_url }})
2. **Semantic** — purpose-based radius/spacing/typography aliasing core. → [Semantic tokens]({{ '/docs/tokens/DS3-tokens/semantic/' | relative_url }})
3. **Semantic colors** — mode-specific colors (action/text/icon/surface/utility/dataviz), defined per Light & Dark. → [Semantic colors]({{ '/docs/tokens/DS3-tokens/semantic-colors/' | relative_url }})
4. **Components** — per-component tokens aliasing semantic + core. → [Component tokens]({{ '/docs/tokens/DS3-tokens/components/' | relative_url }})
5. **Web overrides** — platform-specific overrides for web. → [Web tokens]({{ '/docs/tokens/DS3-tokens/web/' | relative_url }})

## Reading aliases

A value like `{color.brand.primary.500}` is an **alias** — a pointer to another token. In these docs the alias is shown in one column and its fully resolved value (e.g. `#3d3e9f`) in the next. Colors resolve differently per mode, so color tables include both **Light** and **Dark** resolved values.

## Themes & platforms

From `$themes.json`. `source` = referenced but not emitted; `enabled` = active in that theme.

| Theme  | Group    | Token sets                                                                                                                                           |
| ------ | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| light  | mode     | base/core (source), base/semantic (enabled), base/component (enabled), mode/light (enabled)                                                          |
| dark   | mode     | base/core (source), base/semantic (enabled), base/component (enabled), mode/dark (enabled)                                                           |
| mobile | platform | base/core (enabled), base/semantic (enabled), base/component (enabled)                                                                               |
| web    | platform | base/core (source), base/semantic (source), base/component (source), web/core-web (enabled), web/semantic-web (enabled), web/component-web (enabled) |

## Token set order

Resolution order from `$metadata.json` (later sets can override earlier):

1. `base/core`
2. `base/semantic`
3. `base/component`
4. `web/core-web`
5. `web/semantic-web`
6. `web/component-web`
7. `mode/light`
8. `mode/dark`

## At a glance

| Metric                   | Count |
| ------------------------ | ----- |
| Core primitives (colors) | 114   |
| Semantic colors per mode | 198   |
| Components               | 9     |
