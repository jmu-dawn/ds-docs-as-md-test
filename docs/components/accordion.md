---
title: Accordion
nav_order: 1
---

Source: Figma file "DS3 - Mobile", component set `5605:11885`. Extracted via the Token Extractor plugin (Tokens Studio `sharedPluginData`).

Four variants across `State` × `Padding content` × `Expanded`:

| Node         | State   | Padding content | Expanded |
| ------------ | ------- | --------------- | -------- |
| `5605:11885` | Default | Default         | True     |
| `12293:4171` | Default | None            | True     |
| `12299:4325` | Default | None            | False    |
| `9564:9056`  | Default | Default         | False    |

**All four variants carry an identical set of token assignments** at the layer level — none of the three variant axes maps to a different _token_. The axes that do differ (`Padding content`, `Expanded`) change layout/visibility rather than token values; see Notes. Tokens are therefore grouped by layer anatomy below rather than by variant.

## Container

| Property                            | Token                                             |
| ----------------------------------- | ------------------------------------------------- |
| `fill` (background)                 | `color.action.neutral.default.background.default` |
| `borderColor`                       | `color.action.neutral.default.border.default`     |
| `borderRadius` (+ all four corners) | `borderRadius.md`                                 |

## Header

| Layer                                  | Property                 | Token                                   |
| -------------------------------------- | ------------------------ | --------------------------------------- |
| Header                                 | `horizontalPadding`      | `padding.lg`                            |
| Header                                 | `verticalPadding`        | `padding.lg`                            |
| Leading                                | `paddingRight`           | `padding.sm`                            |
| Leading Content (instance)             | `fill` (icon background) | `listItem.color.default.iconBg.default` |
| Leading Content → icon `Vector`        | `fill`                   | `listItem.color.default.icon.default`   |
| Title                                  | `typography`             | `typography.heading3.emphasized`        |
| Title                                  | `fill`                   | `color.text.neutral.onLight.default`    |
| Chevron → `Vector` (CaretUp/CaretDown) | `fill`                   | `color.icon.neutral.onLight.muted`      |

## Body (subtitles + divider)

| Layer       | Property     | Token                               |
| ----------- | ------------ | ----------------------------------- |
| Subtitle 1  | `typography` | `typography.labelMedium.regular`    |
| Subtitle 1  | `fill`       | `color.text.neutral.onLight.subtle` |
| Divider dot | `fill`       | `color.text.neutral.onLight.subtle` |
| Subtitle 2  | `typography` | `typography.labelMedium.regular`    |
| Subtitle 2  | `fill`       | `color.text.neutral.onLight.subtle` |

## Content (only when `Padding content=Default`)

Present only in the two `Padding content=Default` variants (`5605:11885`, `9564:9056`). Absent from both `Padding content=None` variants.

| Property            | Token        |
| ------------------- | ------------ |
| `horizontalPadding` | `padding.lg` |
| `verticalPadding`   | `padding.lg` |

## Notes

- **`Padding content=None` is un-tokenized.** In the two `None` variants the Content frame carries no padding tokens at all (the plugin only exports token-bearing nodes, so it doesn't appear). The padding difference is set as a raw `0` rather than via a `padding.none`-style token — a tokenization gap if you want the "no padding" state to be token-driven.
- **`Expanded` maps to no token change.** Both `Expanded=False` variants still carry the full body text tokens (Subtitle 1, Divider dot, Subtitle 2). Collapsing is handled by visibility, not tokens — expected, but worth knowing the collapsed state isn't a distinct token surface. The chevron also swaps glyph (CaretUp ↔ CaretDown) while keeping the same `color.icon.neutral.onLight.muted` fill.
- **Two icons, two color sources.** The leading content icon uses the `listItem.color.default.*` set (`iconBg` for its background, `icon` for the glyph), while the trailing chevron uses `color.icon.neutral.onLight.muted`. Both glyph layers happen to be named `Vector`; if you audit straight from the raw extract, the shared layer name can mask that these are two different tokens.
- **Card surface uses an `action` token.** As with the Article card, the container `fill`/`borderColor` resolve to `color.action.neutral.default.*` (an interactive-action semantic) on a container surface. Consistent between the two components, but worth confirming it's the intended surface token.
