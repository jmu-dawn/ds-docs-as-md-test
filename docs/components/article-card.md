---
title: Article Card
nav_order: 2
---

Source: Figma file "DS3 - Mobile", component `State=Default` (`6388:13003`). Extracted via the Token Extractor plugin (Tokens Studio `sharedPluginData`).

This is a single-variant component (`State=Default`), so there are no variant dimensions to compare. Tokens below are grouped by layer anatomy rather than by variant.

## Card root (`6388:13003`)

| Property            | Token                                             |
| ------------------- | ------------------------------------------------- |
| `fill` (background) | `color.action.neutral.default.background.default` |
| `borderColor`       | `color.action.neutral.default.border.default`     |
| `borderRadius`      | `borderRadius.md`                                 |
| `padding`           | `padding.lg`                                      |
| `itemSpacing` (gap) | `gap.lg`                                          |

## Layout frame gaps

Every structural frame inside the card uses the same `gap.sm` spacing token.

| Frame        | `itemSpacing` |
| ------------ | ------------- |
| Content left | `gap.sm`      |
| Category tag | `gap.sm`      |
| Info         | `gap.sm`      |
| Title        | `gap.sm`      |
| Meta info    | `gap.sm`      |
| Reading time | `gap.sm`      |

## Category tag → Tag badge (nested instance)

The category tag is a nested `Tag` instance using the `filled / cat2` color set.

| Property                  | Token                                      |
| ------------------------- | ------------------------------------------ |
| `fill` (background)       | `tag.color.filled.cat2.background.default` |
| `borderColor`             | `tag.color.filled.cat2.border.default`     |
| `borderWidth`             | `tag.borderWidth.default`                  |
| `borderRadius`            | `tag.borderRadius.default`                 |
| `horizontalPadding`       | `padding.sm`                               |
| `verticalPadding`         | `padding.xs`                               |
| `itemSpacing` (gap)       | `gap.xs`                                   |
| Label `typography`        | `typography.labelSmall.emphasized`         |
| Label `fill` (foreground) | `tag.color.filled.cat2.foreground.default` |
| Sparkle icon `fill`       | `tag.color.filled.cat2.foreground.default` |

## Title

| Property     | Token                                |
| ------------ | ------------------------------------ |
| `typography` | `typography.labelMedium.emphasized`  |
| `fill`       | `color.text.neutral.onLight.default` |

## Meta info

| Layer              | Property     | Token                               |
| ------------------ | ------------ | ----------------------------------- |
| Date               | `typography` | `typography.labelSmall.regular`     |
| Date               | `fill`       | `color.text.neutral.onLight.subtle` |
| Divider dot        | `fill`       | `color.icon.neutral.onLight.subtle` |
| Reading time label | `typography` | `typography.labelSmall.regular`     |
| Reading time label | `fill`       | `color.text.neutral.onLight.subtle` |

## Media placeholder (nested instance)

| Property       | Token               |
| -------------- | ------------------- |
| `borderRadius` | `borderRadius.none` |

## Notes

- **Card surface uses an `action` token.** The root `fill` and `borderColor` resolve to `color.action.neutral.default.*` — an _interactive action_ semantic. For a static content card a surface/container token would normally be expected; worth confirming this is intentional and not a borrowed swatch.
- **Border color without a border width.** The card root carries `borderColor` but no `borderWidth` token (only the nested Tag has `tag.borderWidth.default`). If the card is meant to render a visible 1px outline, the width is currently un-tokenized.
- **`cat2` category slot.** The tag maps to `tag.color.filled.cat2.*`. That's a category-color slot rather than a semantic name, so the rendered hue depends on the cat2 assignment — fine, just not self-describing.
