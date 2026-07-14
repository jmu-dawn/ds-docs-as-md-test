---
title: Web tokens
group: DS3 Tokens
nav_order: 6
---

Tokens that override the base set for the **web** platform. Where web redefines a token, these values win on web. Sources: `tokens/web/core-web.json`, `tokens/web/semantic-web.json`, `tokens/web/component-web.json`.

## Font sizes (core-web)

| Token | Size |
| ----- | ---- |
| title | `34` |
| h1    | `24` |
| h2    | `20` |
| h3    | `16` |
| body  | `16` |
| sm    | `14` |
| xs    | `12` |
| xxs   | `10` |

## Border radius (semantic-web)

| Token | Alias               | Value   |
| ----- | ------------------- | ------- |
| none  | `{dimension.0px}`   | `0px`   |
| xs    | `{dimension.4px}`   | `4px`   |
| sm    | `{dimension.8px}`   | `8px`   |
| md    | `{dimension.12px}`  | `12px`  |
| lg    | `{dimension.16px}`  | `16px`  |
| xl    | `{dimension.20px}`  | `20px`  |
| xxl   | `{dimension.24px}`  | `24px`  |
| round | `{dimension.999px}` | `999px` |

## Component overrides (component-web)

### button

**Dimensions / radius**

| Token                 | Alias               | Value |
| --------------------- | ------------------- | ----- |
| borderRadius.default  | `{borderRadius.sm}` | `8px` |
| borderRadius.hover    | `{borderRadius.sm}` | `8px` |
| borderRadius.pressed  | `{borderRadius.sm}` | `8px` |
| borderRadius.disabled | `{borderRadius.sm}` | `8px` |

### chip

**Dimensions / radius**

| Token                | Alias               | Value |
| -------------------- | ------------------- | ----- |
| borderRadius.default | `{borderRadius.sm}` | `8px` |
| gap.default          | `{gap.sm}`          | `8px` |

**Typography**

| Token              | Family | Weight | Size | Line height |
| ------------------ | ------ | ------ | ---- | ----------- |
| typography.label   | Inter  | 500    | 12px | 100%        |
| typography.counter | Inter  | 500    | 12px | 100%        |

**Colors**

| Token                                | Alias                                                | Light     | Dark      |
| ------------------------------------ | ---------------------------------------------------- | --------- | --------- |
| color.inputChip.background.default   | `{color.action.neutral.default.background.default}`  | `#ffffff` | `#111827` |
| color.inputChip.background.hover     | `{color.action.neutral.default.background.hover}`    | `#f3f4f6` | `#1f2937` |
| color.inputChip.background.pressed   | `{color.action.neutral.default.background.pressed}`  | `#dfe2e7` | `#374151` |
| color.inputChip.background.selected  | `{color.surface.brand.border.base}`                  | `#d6d7f5` | `#202266` |
| color.inputChip.background.disabled  | `{color.action.neutral.default.background.disabled}` | `#f3f4f6` | `#1f2937` |
| color.inputChip.border.default       | `{color.neutralPalette.subtle}`                      | `#d1d5db` | `#374151` |
| color.inputChip.border.hover         | `{color.action.neutral.default.border.hover}`        | `#d1d5db` | `#374151` |
| color.inputChip.border.pressed       | `{color.action.neutral.default.border.pressed}`      | `#9ca3af` | `#4b5563` |
| color.inputChip.border.selected      | `{chip.color.inputChip.background.selected}`         | `#d6d7f5` | `#202266` |
| color.inputChip.border.disabled      | `{color.action.neutral.default.border.disabled}`     | `#dfe2e7` | `#374151` |
| color.inputChip.foreground.default   | `{color.text.neutral.onLight.default}`               | `#1f2937` | `#f3f4f6` |
| color.inputChip.foreground.hover     | `{color.text.neutral.onLight.default}`               | `#1f2937` | `#f3f4f6` |
| color.inputChip.foreground.pressed   | `{color.text.neutral.onLight.default}`               | `#1f2937` | `#f3f4f6` |
| color.inputChip.foreground.selected  | `{color.text.utility.info.default}`                  | `#1d4ed8` | `#60a5fa` |
| color.inputChip.foreground.disabled  | `{color.text.neutral.onLight.muted}`                 | `#9ca3af` | `#6b7280` |
| color.filterChip.background.default  | `{color.action.neutral.default.background.default}`  | `#ffffff` | `#111827` |
| color.filterChip.background.hover    | `{color.action.neutral.default.background.hover}`    | `#f3f4f6` | `#1f2937` |
| color.filterChip.background.pressed  | `{color.action.neutral.default.background.pressed}`  | `#dfe2e7` | `#374151` |
| color.filterChip.background.selected | `{color.action.brand.background.default}`            | `#3d3e9f` | `#4647b1` |
| color.filterChip.background.disabled | `{color.action.neutral.default.background.disabled}` | `#f3f4f6` | `#1f2937` |
| color.filterChip.border.default      | `{color.neutralPalette.subtle}`                      | `#d1d5db` | `#374151` |
| color.filterChip.border.hover        | `{color.action.neutral.default.border.hover}`        | `#d1d5db` | `#374151` |
| color.filterChip.border.pressed      | `{color.action.neutral.default.border.pressed}`      | `#9ca3af` | `#4b5563` |
| color.filterChip.border.selected     | `{chip.color.inputChip.background.selected}`         | `#d6d7f5` | `#202266` |
| color.filterChip.border.disabled     | `{color.action.neutral.default.border.disabled}`     | `#dfe2e7` | `#374151` |
| color.filterChip.foreground.default  | `{color.text.neutral.onLight.default}`               | `#1f2937` | `#f3f4f6` |
| color.filterChip.foreground.hover    | `{color.text.neutral.onLight.default}`               | `#1f2937` | `#f3f4f6` |
| color.filterChip.foreground.pressed  | `{color.text.neutral.onLight.default}`               | `#1f2937` | `#f3f4f6` |
| color.filterChip.foreground.selected | `{color.text.neutral.onDark.default}`                | `#f9fafb` | `#1f2937` |
| color.filterChip.foreground.disabled | `{color.text.neutral.onLight.muted}`                 | `#9ca3af` | `#6b7280` |
| color.actionChip.background.default  | `{color.action.neutral.default.background.default}`  | `#ffffff` | `#111827` |
| color.actionChip.background.hover    | `{color.action.neutral.default.background.hover}`    | `#f3f4f6` | `#1f2937` |
| color.actionChip.background.pressed  | `{color.action.neutral.default.background.pressed}`  | `#dfe2e7` | `#374151` |
| color.actionChip.background.selected | `{color.action.brand.background.default}`            | `#3d3e9f` | `#4647b1` |
| color.actionChip.background.disabled | `{color.action.neutral.default.background.disabled}` | `#f3f4f6` | `#1f2937` |
| color.actionChip.border.default      | `{color.neutralPalette.subtle}`                      | `#d1d5db` | `#374151` |
| color.actionChip.border.hover        | `{color.action.neutral.default.border.hover}`        | `#d1d5db` | `#374151` |
| color.actionChip.border.pressed      | `{color.action.neutral.default.border.pressed}`      | `#9ca3af` | `#4b5563` |
| color.actionChip.border.selected     | `{chip.color.inputChip.background.selected}`         | `#d6d7f5` | `#202266` |
| color.actionChip.border.disabled     | `{color.action.neutral.default.border.disabled}`     | `#dfe2e7` | `#374151` |
| color.actionChip.foreground.default  | `{color.text.neutral.onLight.default}`               | `#1f2937` | `#f3f4f6` |
| color.actionChip.foreground.hover    | `{color.text.neutral.onLight.default}`               | `#1f2937` | `#f3f4f6` |
| color.actionChip.foreground.pressed  | `{color.text.neutral.onLight.default}`               | `#1f2937` | `#f3f4f6` |
| color.actionChip.foreground.selected | `{color.text.neutral.onDark.default}`                | `#f9fafb` | `#1f2937` |
| color.actionChip.foreground.disabled | `{color.text.neutral.onLight.muted}`                 | `#9ca3af` | `#6b7280` |

### badge

**Dimensions / radius**

| Token                | Alias               | Value |
| -------------------- | ------------------- | ----- |
| borderRadius.default | `{borderRadius.xs}` | `4px` |

### tag

**Colors**

| Token                                | Alias                                       | Light             | Dark              |
| ------------------------------------ | ------------------------------------------- | ----------------- | ----------------- |
| color.filled.cat1.background.default | `{color.global.gray.200}`                   | `#dfe2e7`         | `#dfe2e7`         |
| color.filled.cat1.background.hover   | `{color.global.gray.300}`                   | `#d1d5db`         | `#d1d5db`         |
| color.filled.cat1.background.pressed | `{color.global.gray.400}`                   | `#9ca3af`         | `#9ca3af`         |
| color.filled.cat1.foreground.default | `{color.global.gray.600}`                   | `#4b5563`         | `#4b5563`         |
| color.filled.cat1.foreground.pressed | `{color.global.gray.700}`                   | `#374151`         | `#374151`         |
| color.filled.cat1.border.default     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat1.border.pressed     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat2.background.default | `{color.global.blue.100}`                   | `#dbeafe`         | `#dbeafe`         |
| color.filled.cat2.background.hover   | `{color.global.blue.200}`                   | `#bfdbfe`         | `#bfdbfe`         |
| color.filled.cat2.background.pressed | `{color.global.blue.300}`                   | `#93c5fd`         | `#93c5fd`         |
| color.filled.cat2.foreground.default | `{color.global.blue.700}`                   | `#1d4ed8`         | `#1d4ed8`         |
| color.filled.cat2.foreground.pressed | `{color.global.blue.800}`                   | `#1e40af`         | `#1e40af`         |
| color.filled.cat2.border.default     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat2.border.pressed     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat3.background.default | `{color.global.green.100}`                  | `#dcfce7`         | `#dcfce7`         |
| color.filled.cat3.background.hover   | `{color.global.green.200}`                  | `#bbf7d0`         | `#bbf7d0`         |
| color.filled.cat3.background.pressed | `{color.global.green.300}`                  | `#86efac`         | `#86efac`         |
| color.filled.cat3.foreground.default | `{color.global.green.700}`                  | `#15803d`         | `#15803d`         |
| color.filled.cat3.foreground.pressed | `{color.global.green.800}`                  | `#166534`         | `#166534`         |
| color.filled.cat3.border.default     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat3.border.pressed     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat4.background.default | `{color.global.red.100}`                    | `#fee2e2`         | `#fee2e2`         |
| color.filled.cat4.background.hover   | `{color.global.red.200}`                    | `#fecaca`         | `#fecaca`         |
| color.filled.cat4.background.pressed | `{color.global.red.300}`                    | `#fca5a5`         | `#fca5a5`         |
| color.filled.cat4.foreground.default | `{color.global.red.700}`                    | `#b91c1c`         | `#b91c1c`         |
| color.filled.cat4.foreground.pressed | `{color.global.red.800}`                    | `#991b1b`         | `#991b1b`         |
| color.filled.cat4.border.default     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat4.border.pressed     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat5.background.default | `{color.global.orange.100}`                 | `#ffedd5`         | `#ffedd5`         |
| color.filled.cat5.background.hover   | `{color.global.orange.200}`                 | `#fed7aa`         | `#fed7aa`         |
| color.filled.cat5.background.pressed | `{color.global.orange.300}`                 | `#fdba74`         | `#fdba74`         |
| color.filled.cat5.foreground.default | `{color.global.orange.700}`                 | `#c2410c`         | `#c2410c`         |
| color.filled.cat5.foreground.pressed | `{color.global.orange.800}`                 | `#9a3412`         | `#9a3412`         |
| color.filled.cat5.border.default     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat5.border.pressed     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.cat1.background.default  | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.cat1.background.hover    | `{color.global.transparent.10}`             | `rgba(0,0,0,0.1)` | `rgba(0,0,0,0.1)` |
| color.ghost.cat1.background.pressed  | `{color.global.transparent.20}`             | `rgba(0,0,0,0.2)` | `rgba(0,0,0,0.2)` |
| color.ghost.cat1.foreground.default  | `{color.global.gray.600}`                   | `#4b5563`         | `#4b5563`         |
| color.ghost.cat1.foreground.pressed  | `{color.global.gray.700}`                   | `#374151`         | `#374151`         |
| color.ghost.cat1.border.default      | `{tag.color.ghost.cat1.background.default}` | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.cat1.border.pressed      | `{tag.color.ghost.cat1.background.pressed}` | `rgba(0,0,0,0.2)` | `rgba(0,0,0,0.2)` |
