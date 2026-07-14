---
title: Checkbox
nav_order: 7
---

Source: Figma file "DS3 - Mobile" (`—`). Extracted via the Token Extractor plugin (Tokens Studio `sharedPluginData`). Covers both platform variants of the checkbox.

## iOS

### Shared tokens (all variants)

| Property       | Token                            |
| -------------- | -------------------------------- |
| `borderRadius` | `borderRadius.xs`                |
| `itemSpacing`  | `gap.md`                         |
| `typography`   | `typography.labelMedium.regular` |

### Tokens by Selected

| Selected | `horizontalPadding` | `verticalPadding` |
| -------- | ------------------- | ----------------- |
| False    | —                   | —                 |
| True     | `padding.xxs`       | `padding.xxs`     |

### Tokens by State

| State    | `borderColor (misc/.Focus ring)` | `fill (Label)`                       |
| -------- | -------------------------------- | ------------------------------------ |
| Default  | —                                | `color.text.neutral.onLight.default` |
| Disabled | —                                | `color.text.neutral.onLight.muted`   |
| Focus    | `color.utility.focus.default`    | `color.text.neutral.onLight.default` |
| Hover    | —                                | `color.text.neutral.onLight.default` |
| Pressed  | —                                | `color.text.neutral.onLight.default` |

### Tokens by Selected × State × Type

| Selected | State    | Type     | `borderColor`                                   | `borderColor (Checkbox)`                     | `fill (Checkbox)`                                  | `fill (Vector)`                     |
| -------- | -------- | -------- | ----------------------------------------------- | -------------------------------------------- | -------------------------------------------------- | ----------------------------------- |
| False    | Default  | Default  | `color.action.neutral.elevated.border.default`  | —                                            | `color.action.neutral.default.background.default`  | —                                   |
| False    | Default  | Emphasis | `color.action.neutral.elevated.border.default`  | —                                            | `color.action.neutral.default.background.default`  | —                                   |
| False    | Default  | Error    | `color.action.danger.border.default`            | —                                            | `color.action.neutral.default.background.default`  | —                                   |
| False    | Disabled | Default  | `color.action.neutral.elevated.border.disabled` | —                                            | `color.action.neutral.default.background.disabled` | —                                   |
| False    | Disabled | Emphasis | `color.action.neutral.elevated.border.disabled` | —                                            | `color.action.neutral.default.background.disabled` | —                                   |
| False    | Disabled | Error    | `color.action.neutral.elevated.border.disabled` | —                                            | `color.action.neutral.default.background.disabled` | —                                   |
| False    | Focus    | Default  | —                                               | `color.action.neutral.elevated.border.hover` | `color.action.neutral.default.background.hover`    | —                                   |
| False    | Focus    | Emphasis | —                                               | `color.action.neutral.elevated.border.hover` | `color.action.neutral.default.background.hover`    | —                                   |
| False    | Focus    | Error    | —                                               | `color.action.danger.border.hover`           | `color.action.neutral.default.background.hover`    | —                                   |
| False    | Hover    | Default  | `color.action.neutral.elevated.border.hover`    | —                                            | `color.action.neutral.default.background.hover`    | —                                   |
| False    | Hover    | Emphasis | `color.action.neutral.elevated.border.hover`    | —                                            | `color.action.neutral.default.background.hover`    | —                                   |
| False    | Hover    | Error    | `color.action.danger.border.hover`              | —                                            | `color.action.neutral.default.background.hover`    | —                                   |
| False    | Pressed  | Default  | `color.action.neutral.elevated.border.pressed`  | —                                            | `color.action.neutral.default.background.pressed`  | —                                   |
| False    | Pressed  | Emphasis | `color.action.neutral.elevated.border.pressed`  | —                                            | `color.action.neutral.default.background.pressed`  | —                                   |
| False    | Pressed  | Error    | `color.action.danger.border.pressed`            | —                                            | `color.action.neutral.default.background.pressed`  | —                                   |
| True     | Default  | Default  | `color.action.neutral.selected.border.default`  | —                                            | `color.action.neutral.selected.background.default` | `color.icon.neutral.onDark.default` |
| True     | Default  | Emphasis | `color.action.brand.border.default`             | —                                            | `color.action.brand.background.default`            | `color.icon.neutral.onDark.strong`  |
| True     | Default  | Error    | `color.action.danger.border.default`            | —                                            | `color.action.danger.background.default`           | `color.icon.neutral.onDark.strong`  |
| True     | Disabled | Default  | —                                               | —                                            | `color.action.neutral.selected.border.disabled`    | `color.icon.neutral.onDark.default` |
| True     | Disabled | Emphasis | —                                               | —                                            | `color.action.neutral.selected.border.disabled`    | `color.icon.neutral.onDark.default` |
| True     | Disabled | Error    | —                                               | —                                            | `color.action.neutral.selected.border.disabled`    | `color.icon.neutral.onDark.default` |
| True     | Focus    | Default  | —                                               | `color.action.neutral.selected.border.hover` | `color.action.neutral.selected.background.hover`   | `color.icon.neutral.onDark.default` |
| True     | Focus    | Emphasis | —                                               | `color.action.brand.border.hover`            | `color.action.brand.background.hover`              | `color.icon.neutral.onDark.strong`  |
| True     | Focus    | Error    | —                                               | `color.action.danger.border.hover`           | `color.action.danger.background.hover`             | `color.icon.neutral.onDark.strong`  |
| True     | Hover    | Default  | `color.action.neutral.selected.border.hover`    | —                                            | `color.action.neutral.selected.background.hover`   | `color.icon.neutral.onDark.default` |
| True     | Hover    | Emphasis | `color.action.brand.border.hover`               | —                                            | `color.action.brand.background.hover`              | `color.icon.neutral.onDark.strong`  |
| True     | Hover    | Error    | `color.action.danger.border.hover`              | —                                            | `color.action.danger.background.hover`             | `color.icon.neutral.onDark.strong`  |
| True     | Pressed  | Default  | `color.action.neutral.selected.border.pressed`  | —                                            | `color.action.neutral.selected.background.pressed` | `color.icon.neutral.onDark.default` |
| True     | Pressed  | Emphasis | `color.action.brand.border.pressed`             | —                                            | `color.action.brand.background.pressed`            | `color.icon.neutral.onDark.strong`  |
| True     | Pressed  | Error    | `color.action.danger.border.pressed`            | —                                            | `color.action.danger.background.pressed`           | `color.icon.neutral.onDark.strong`  |

### All 45 instances

| Node        | Selected | Indeterminate | State    | Type     |
| ----------- | -------- | ------------- | -------- | -------- |
| `5369:1652` | False    | False         | Default  | Default  |
| `6978:832`  | False    | False         | Default  | Emphasis |
| `5369:1655` | False    | False         | Hover    | Default  |
| `6978:835`  | False    | False         | Hover    | Emphasis |
| `5369:1658` | False    | False         | Pressed  | Default  |
| `6978:838`  | False    | False         | Pressed  | Emphasis |
| `5369:1661` | False    | False         | Disabled | Default  |
| `6978:841`  | False    | False         | Disabled | Emphasis |
| `5369:1664` | False    | False         | Focus    | Default  |
| `6978:844`  | False    | False         | Focus    | Emphasis |
| `5369:1667` | True     | False         | Default  | Default  |
| `5369:1670` | True     | False         | Hover    | Default  |
| `5369:1673` | True     | False         | Pressed  | Default  |
| `5369:1676` | True     | False         | Disabled | Default  |
| `5369:1679` | True     | False         | Focus    | Default  |
| `5369:1682` | True     | True          | Default  | Default  |
| `5369:1685` | True     | True          | Hover    | Default  |
| `5369:1688` | True     | True          | Pressed  | Default  |
| `5369:1691` | True     | True          | Disabled | Default  |
| `5369:1694` | True     | True          | Focus    | Default  |
| `5369:1697` | True     | False         | Default  | Emphasis |
| `5369:1700` | True     | False         | Hover    | Emphasis |
| `5369:1703` | True     | False         | Pressed  | Emphasis |
| `5369:1706` | True     | False         | Disabled | Emphasis |
| `5369:1709` | True     | False         | Focus    | Emphasis |
| `5369:1712` | True     | True          | Default  | Emphasis |
| `5369:1715` | True     | True          | Hover    | Emphasis |
| `5369:1718` | True     | True          | Pressed  | Emphasis |
| `5369:1721` | True     | True          | Disabled | Emphasis |
| `5369:1724` | True     | True          | Focus    | Emphasis |
| `5369:1727` | False    | False         | Default  | Error    |
| `5369:1730` | False    | False         | Hover    | Error    |
| `5369:1733` | False    | False         | Pressed  | Error    |
| `5369:1736` | False    | False         | Disabled | Error    |
| `5369:1739` | False    | False         | Focus    | Error    |
| `5369:1742` | True     | False         | Default  | Error    |
| `5369:1745` | True     | False         | Hover    | Error    |
| `5369:1748` | True     | False         | Pressed  | Error    |
| `5369:1751` | True     | False         | Disabled | Error    |
| `5369:1754` | True     | False         | Focus    | Error    |
| `5369:1757` | True     | True          | Default  | Error    |
| `5369:1760` | True     | True          | Hover    | Error    |
| `5369:1763` | True     | True          | Pressed  | Error    |
| `5369:1766` | True     | True          | Disabled | Error    |
| `5369:1769` | True     | True          | Focus    | Error    |

## Android

### Shared tokens (all variants)

| Property            | Token        |
| ------------------- | ------------ |
| `horizontalPadding` | `padding.xs` |
| `verticalPadding`   | `padding.xs` |

### Tokens by Type

| Type                | `fill (icon)`                       |
| ------------------- | ----------------------------------- |
| Error indeterminate | `color.icon.neutral.onDark.default` |
| Error selected      | `color.icon.neutral.onDark.default` |
| Error unselected    | —                                   |
| Indeterminate       | `color.icon.neutral.onDark.default` |
| Selected            | `color.icon.neutral.onDark.default` |
| Unselected          | —                                   |

### Tokens by Type × State

| Type                | State    | `fill (foreground)`           | `borderColor`                                   | `fill (Ripple)`               | `fill (container)`                                 | `fill (state-layer)`          |
| ------------------- | -------- | ----------------------------- | ----------------------------------------------- | ----------------------------- | -------------------------------------------------- | ----------------------------- |
| Error indeterminate | Disabled | —                             | —                                               | —                             | `color.action.neutral.selected.border.disabled`    | —                             |
| Error indeterminate | Enabled  | —                             | —                                               | —                             | `color.action.danger.background.default`           | —                             |
| Error indeterminate | Focused  | —                             | —                                               | —                             | `color.action.danger.background.hover`             | `color.global.transparent.10` |
| Error indeterminate | Hovered  | —                             | —                                               | —                             | `color.action.danger.background.hover`             | `color.global.transparent.10` |
| Error indeterminate | Pressed  | —                             | —                                               | `color.utility.danger.strong` | `color.action.danger.background.pressed`           | `color.global.transparent.10` |
| Error selected      | Disabled | —                             | —                                               | —                             | `color.action.neutral.selected.border.disabled`    | —                             |
| Error selected      | Enabled  | —                             | —                                               | —                             | `color.action.danger.background.default`           | —                             |
| Error selected      | Focused  | —                             | —                                               | —                             | `color.action.danger.background.hover`             | `color.global.transparent.10` |
| Error selected      | Hovered  | —                             | —                                               | —                             | `color.action.danger.background.hover`             | `color.global.transparent.10` |
| Error selected      | Pressed  | —                             | —                                               | `color.utility.danger.strong` | `color.action.danger.background.pressed`           | `color.global.transparent.10` |
| Error unselected    | Disabled | —                             | `color.action.neutral.selected.border.disabled` | —                             | —                                                  | —                             |
| Error unselected    | Enabled  | —                             | `color.action.danger.border.default`            | —                             | —                                                  | —                             |
| Error unselected    | Focused  | `color.global.transparent.10` | `color.action.danger.border.hover`              | —                             | —                                                  | —                             |
| Error unselected    | Hovered  | `color.global.transparent.10` | `color.action.danger.border.hover`              | —                             | —                                                  | —                             |
| Error unselected    | Pressed  | —                             | `color.action.danger.border.pressed`            | `color.utility.danger.strong` | —                                                  | `color.global.transparent.10` |
| Indeterminate       | Disabled | —                             | —                                               | —                             | `color.action.neutral.selected.border.disabled`    | —                             |
| Indeterminate       | Enabled  | —                             | —                                               | —                             | `color.action.neutral.selected.background.default` | —                             |
| Indeterminate       | Focused  | —                             | —                                               | —                             | `color.action.neutral.selected.background.default` | `color.global.transparent.10` |
| Indeterminate       | Hovered  | —                             | —                                               | —                             | `color.action.neutral.selected.background.default` | `color.global.transparent.10` |
| Indeterminate       | Pressed  | —                             | —                                               | `color.neutralPalette.heavy`  | `color.action.neutral.selected.background.default` | `color.global.transparent.10` |
| Selected            | Disabled | —                             | —                                               | —                             | `color.action.neutral.selected.border.disabled`    | —                             |
| Selected            | Enabled  | —                             | —                                               | —                             | `color.action.neutral.selected.background.default` | —                             |
| Selected            | Focused  | —                             | —                                               | —                             | `color.action.neutral.selected.background.default` | `color.global.transparent.10` |
| Selected            | Hovered  | —                             | —                                               | —                             | `color.action.neutral.selected.background.default` | `color.global.transparent.10` |
| Selected            | Pressed  | —                             | —                                               | `color.neutralPalette.heavy`  | `color.action.neutral.selected.background.default` | `color.global.transparent.10` |
| Unselected          | Disabled | —                             | `color.action.neutral.selected.border.disabled` | —                             | —                                                  | —                             |
| Unselected          | Enabled  | —                             | `color.action.neutral.elevated.border.pressed`  | —                             | —                                                  | —                             |
| Unselected          | Focused  | `color.global.transparent.10` | `color.action.neutral.elevated.border.pressed`  | —                             | —                                                  | —                             |
| Unselected          | Hovered  | `color.global.transparent.10` | `color.action.neutral.elevated.border.pressed`  | —                             | —                                                  | —                             |
| Unselected          | Pressed  | —                             | `color.action.neutral.elevated.border.pressed`  | `color.neutralPalette.heavy`  | —                                                  | `color.global.transparent.10` |

### All 30 instances

| Node         | Type                | State    | Foreground token              |
| ------------ | ------------------- | -------- | ----------------------------- |
| `9847:68425` | Selected            | Enabled  | —                             |
| `9847:68429` | Selected            | Disabled | —                             |
| `9847:68433` | Selected            | Hovered  | —                             |
| `9847:68437` | Selected            | Focused  | —                             |
| `9847:68441` | Selected            | Pressed  | —                             |
| `9847:68446` | Indeterminate       | Enabled  | —                             |
| `9847:68450` | Indeterminate       | Disabled | —                             |
| `9847:68454` | Indeterminate       | Hovered  | —                             |
| `9847:68458` | Indeterminate       | Focused  | —                             |
| `9847:68462` | Indeterminate       | Pressed  | —                             |
| `9847:68467` | Unselected          | Enabled  | —                             |
| `9847:68470` | Unselected          | Disabled | —                             |
| `9847:68473` | Unselected          | Hovered  | `color.global.transparent.10` |
| `9847:68476` | Unselected          | Focused  | `color.global.transparent.10` |
| `9847:68479` | Unselected          | Pressed  | —                             |
| `9847:68483` | Error selected      | Enabled  | —                             |
| `9847:68487` | Error selected      | Disabled | —                             |
| `9847:68491` | Error selected      | Hovered  | —                             |
| `9847:68495` | Error selected      | Focused  | —                             |
| `9847:68499` | Error selected      | Pressed  | —                             |
| `9847:68504` | Error indeterminate | Enabled  | —                             |
| `9847:68508` | Error indeterminate | Disabled | —                             |
| `9847:68512` | Error indeterminate | Hovered  | —                             |
| `9847:68516` | Error indeterminate | Focused  | —                             |
| `9847:68520` | Error indeterminate | Pressed  | —                             |
| `9847:68525` | Error unselected    | Enabled  | —                             |
| `9847:68528` | Error unselected    | Disabled | —                             |
| `9847:68531` | Error unselected    | Hovered  | `color.global.transparent.10` |
| `9847:68534` | Error unselected    | Focused  | `color.global.transparent.10` |
| `9847:68537` | Error unselected    | Pressed  | —                             |
