---
title: Component tokens
group: DS3 Tokens
nav_order: 5
---

Per-component tokens. Color tokens are mode-dependent — resolved hex shown for both **Light** and **Dark**. Dimension/radius/typography are mode-independent. Source: `tokens/base/component.json`.

## button

**Dimensions / radius / width**

| Token                 | Alias                           | Value   |
| --------------------- | ------------------------------- | ------- |
| borderRadius.default  | `{borderRadius.round}`          | `999px` |
| borderRadius.hover    | `{button.borderRadius.default}` | `999px` |
| borderRadius.pressed  | `{button.borderRadius.default}` | `999px` |
| borderRadius.disabled | `{button.borderRadius.default}` | `999px` |
| borderWidth.default   | `{borderWidth.sm}`              | `1px`   |

**Typography**

| Token              | Family | Weight | Size | Line height |
| ------------------ | ------ | ------ | ---- | ----------- |
| typography.default | Inter  | 500    | 16   | 24px        |
| typography.small   | Inter  | 500    | 14   | 20px        |

**Colors**

| Token                                    | Alias                                                | Light             | Dark              |
| ---------------------------------------- | ---------------------------------------------------- | ----------------- | ----------------- |
| color.primary.background.default         | `{color.action.brand.background.default}`            | `#3d3e9f`         | `#4647b1`         |
| color.primary.background.hover           | `{color.action.brand.background.hover}`              | `#32348c`         | `#3d3e9f`         |
| color.primary.background.pressed         | `{color.action.brand.background.pressed}`            | `#292b79`         | `#32348c`         |
| color.primary.background.disabled        | `{color.action.brand.background.disabled}`           | `#a8a9e3`         | `#202266`         |
| color.primary.border.default             | `{button.color.primary.background.default}`          | `#3d3e9f`         | `#4647b1`         |
| color.primary.border.hover               | `{button.color.primary.background.hover}`            | `#32348c`         | `#3d3e9f`         |
| color.primary.border.pressed             | `{button.color.primary.background.pressed}`          | `#292b79`         | `#32348c`         |
| color.primary.border.disabled            | `{color.action.brand.border.disabled}`               | `#a8a9e3`         | `#202266`         |
| color.primary.foreground.default         | `{color.action.brand.foreground.default}`            | `#f9fafb`         | `#f3f4f6`         |
| color.primary.foreground.hover           | `{color.action.brand.foreground.hover}`              | `#f9fafb`         | `#f3f4f6`         |
| color.primary.foreground.pressed         | `{color.action.brand.foreground.pressed}`            | `#f9fafb`         | `#f3f4f6`         |
| color.primary.foreground.disabled        | `{color.action.brand.foreground.disabled}`           | `#f9fafb`         | `#6b7280`         |
| color.secondary.background.default       | `{color.action.neutral.default.background.default}`  | `#ffffff`         | `#111827`         |
| color.secondary.background.hover         | `{color.action.neutral.default.background.hover}`    | `#f3f4f6`         | `#1f2937`         |
| color.secondary.background.pressed       | `{color.action.neutral.default.background.pressed}`  | `#dfe2e7`         | `#374151`         |
| color.secondary.background.disabled      | `{color.action.neutral.default.background.disabled}` | `#f3f4f6`         | `#1f2937`         |
| color.secondary.border.default           | `{color.action.neutral.default.border.default}`      | `#dfe2e7`         | `#374151`         |
| color.secondary.border.hover             | `{color.action.neutral.default.border.hover}`        | `#d1d5db`         | `#374151`         |
| color.secondary.border.pressed           | `{color.action.neutral.default.border.pressed}`      | `#9ca3af`         | `#4b5563`         |
| color.secondary.border.disabled          | `{color.action.neutral.default.border.disabled}`     | `#dfe2e7`         | `#374151`         |
| color.secondary.foreground.default       | `{color.action.neutral.default.foreground.default}`  | `#1f2937`         | `#f3f4f6`         |
| color.secondary.foreground.hover         | `{color.action.neutral.default.foreground.hover}`    | `#1f2937`         | `#f3f4f6`         |
| color.secondary.foreground.pressed       | `{color.action.neutral.default.foreground.pressed}`  | `#1f2937`         | `#f3f4f6`         |
| color.secondary.foreground.disabled      | `{color.action.neutral.default.foreground.disabled}` | `#9ca3af`         | `#6b7280`         |
| color.elevated.background.default        | `{color.action.neutral.elevated.background.default}` | `#f3f4f6`         | `#1f2937`         |
| color.elevated.background.hover          | `{color.action.neutral.elevated.background.hover}`   | `#dfe2e7`         | `#374151`         |
| color.elevated.background.pressed        | `{color.action.neutral.elevated.background.pressed}` | `#d1d5db`         | `#4b5563`         |
| color.elevated.background.disabled       | `{button.color.secondary.background.disabled}`       | `#f3f4f6`         | `#1f2937`         |
| color.elevated.border.default            | `{color.action.neutral.elevated.border.default}`     | `#d1d5db`         | `#4b5563`         |
| color.elevated.border.hover              | `{color.action.neutral.elevated.border.hover}`       | `#9ca3af`         | `#4b5563`         |
| color.elevated.border.pressed            | `{color.action.neutral.elevated.border.pressed}`     | `#6b7280`         | `#6b7280`         |
| color.elevated.border.disabled           | `{button.color.secondary.border.disabled}`           | `#dfe2e7`         | `#374151`         |
| color.elevated.foreground.default        | `{color.action.neutral.default.foreground.default}`  | `#1f2937`         | `#f3f4f6`         |
| color.elevated.foreground.hover          | `{color.action.neutral.default.foreground.hover}`    | `#1f2937`         | `#f3f4f6`         |
| color.elevated.foreground.pressed        | `{color.action.neutral.default.foreground.pressed}`  | `#1f2937`         | `#f3f4f6`         |
| color.elevated.foreground.disabled       | `{button.color.secondary.foreground.disabled}`       | `#9ca3af`         | `#6b7280`         |
| color.ghost.background.default           | `{color.global.transparent.0}`                       | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.background.hover             | `{button.color.secondary.background.hover}`          | `#f3f4f6`         | `#1f2937`         |
| color.ghost.background.pressed           | `{button.color.secondary.background.pressed}`        | `#dfe2e7`         | `#374151`         |
| color.ghost.background.disabled          | `{button.color.ghost.background.default}`            | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.border.default               | `{button.color.ghost.background.default}`            | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.border.hover                 | `{button.color.secondary.background.hover}`          | `#f3f4f6`         | `#1f2937`         |
| color.ghost.border.pressed               | `{button.color.secondary.background.pressed}`        | `#dfe2e7`         | `#374151`         |
| color.ghost.border.disabled              | `{button.color.ghost.background.disabled}`           | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.foreground.default           | `{color.action.neutral.default.foreground.default}`  | `#1f2937`         | `#f3f4f6`         |
| color.ghost.foreground.hover             | `{color.action.neutral.default.foreground.hover}`    | `#1f2937`         | `#f3f4f6`         |
| color.ghost.foreground.pressed           | `{color.action.neutral.default.foreground.pressed}`  | `#1f2937`         | `#f3f4f6`         |
| color.ghost.foreground.disabled          | `{button.color.secondary.foreground.disabled}`       | `#9ca3af`         | `#6b7280`         |
| color.danger-primary.background.default  | `{color.action.danger.background.default}`           | `#dc2626`         | `#dc2626`         |
| color.danger-primary.background.hover    | `{color.action.danger.background.hover}`             | `#b91c1c`         | `#b91c1c`         |
| color.danger-primary.background.pressed  | `{color.action.danger.background.pressed}`           | `#991b1b`         | `#991b1b`         |
| color.danger-primary.background.disabled | `{color.action.danger.background.disabled}`          | `#f3f4f6`         | `#1f2937`         |
| color.danger-primary.border.default      | `{button.color.danger-primary.background.default}`   | `#dc2626`         | `#dc2626`         |
| color.danger-primary.border.hover        | `{button.color.danger-primary.background.hover}`     | `#b91c1c`         | `#b91c1c`         |
| color.danger-primary.border.pressed      | `{button.color.danger-primary.background.pressed}`   | `#991b1b`         | `#991b1b`         |
| color.danger-primary.border.disabled     | `{color.action.danger.border.disabled}`              | `#f3f4f6`         | `#374151`         |
| color.danger-primary.foreground.default  | `{color.action.danger.foreground.default}`           | `#f9fafb`         | `#f3f4f6`         |
| color.danger-primary.foreground.hover    | `{color.action.danger.foreground.hover}`             | `#f9fafb`         | `#f3f4f6`         |
| color.danger-primary.foreground.pressed  | `{color.action.danger.foreground.pressed}`           | `#f9fafb`         | `#f3f4f6`         |
| color.danger-primary.foreground.disabled | `{color.action.danger.foreground.disabled}`          | `#9ca3af`         | `#6b7280`         |
| color.danger-ghost.background.default    | `{color.global.transparent.0}`                       | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.danger-ghost.background.hover      | `{button.color.danger-primary.background.hover}`     | `#b91c1c`         | `#b91c1c`         |
| color.danger-ghost.background.pressed    | `{button.color.danger-primary.background.pressed}`   | `#991b1b`         | `#991b1b`         |
| color.danger-ghost.background.disabled   | `{button.color.danger-ghost.background.default}`     | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.danger-ghost.border.default        | `{button.color.danger-ghost.background.default}`     | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.danger-ghost.border.hover          | `{button.color.danger-ghost.background.hover}`       | `#b91c1c`         | `#b91c1c`         |
| color.danger-ghost.border.pressed        | `{button.color.danger-ghost.background.pressed}`     | `#991b1b`         | `#991b1b`         |
| color.danger-ghost.border.disabled       | `{button.color.danger-ghost.background.disabled}`    | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.danger-ghost.foreground.default    | `{color.text.utility.danger.subtle}`                 | `#dc2626`         | `#ef4444`         |
| color.danger-ghost.foreground.hover      | `{button.color.danger-primary.foreground.hover}`     | `#f9fafb`         | `#f3f4f6`         |
| color.danger-ghost.foreground.pressed    | `{button.color.danger-primary.foreground.pressed}`   | `#f9fafb`         | `#f3f4f6`         |
| color.danger-ghost.foreground.disabled   | `{button.color.secondary.foreground.disabled}`       | `#9ca3af`         | `#6b7280`         |

## tag

**Dimensions / radius / width**

| Token                | Alias               | Value |
| -------------------- | ------------------- | ----- |
| borderRadius.default | `{borderRadius.xs}` | `4px` |
| borderWidth.default  | `{borderWidth.sm}`  | `1px` |

**Colors**

| Token                                | Alias                                       | Light             | Dark              |
| ------------------------------------ | ------------------------------------------- | ----------------- | ----------------- |
| color.filled.cat1.background.default | `{color.global.gray.200}`                   | `#dfe2e7`         | `#dfe2e7`         |
| color.filled.cat1.background.pressed | `{color.global.gray.300}`                   | `#d1d5db`         | `#d1d5db`         |
| color.filled.cat1.foreground.default | `{color.global.gray.600}`                   | `#4b5563`         | `#4b5563`         |
| color.filled.cat1.foreground.pressed | `{color.global.gray.700}`                   | `#374151`         | `#374151`         |
| color.filled.cat1.border.default     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat1.border.pressed     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat2.background.default | `{color.global.blue.100}`                   | `#dbeafe`         | `#dbeafe`         |
| color.filled.cat2.background.pressed | `{color.global.blue.200}`                   | `#bfdbfe`         | `#bfdbfe`         |
| color.filled.cat2.foreground.default | `{color.global.blue.700}`                   | `#1d4ed8`         | `#1d4ed8`         |
| color.filled.cat2.foreground.pressed | `{color.global.blue.800}`                   | `#1e40af`         | `#1e40af`         |
| color.filled.cat2.border.default     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat2.border.pressed     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat3.background.default | `{color.global.green.100}`                  | `#dcfce7`         | `#dcfce7`         |
| color.filled.cat3.background.pressed | `{color.global.green.200}`                  | `#bbf7d0`         | `#bbf7d0`         |
| color.filled.cat3.foreground.default | `{color.global.green.700}`                  | `#15803d`         | `#15803d`         |
| color.filled.cat3.foreground.pressed | `{color.global.green.800}`                  | `#166534`         | `#166534`         |
| color.filled.cat3.border.default     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat3.border.pressed     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat4.background.default | `{color.global.red.100}`                    | `#fee2e2`         | `#fee2e2`         |
| color.filled.cat4.background.pressed | `{color.global.red.200}`                    | `#fecaca`         | `#fecaca`         |
| color.filled.cat4.foreground.default | `{color.global.red.700}`                    | `#b91c1c`         | `#b91c1c`         |
| color.filled.cat4.foreground.pressed | `{color.global.red.800}`                    | `#991b1b`         | `#991b1b`         |
| color.filled.cat4.border.default     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat4.border.pressed     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat5.background.default | `{color.global.orange.100}`                 | `#ffedd5`         | `#ffedd5`         |
| color.filled.cat5.background.pressed | `{color.global.orange.200}`                 | `#fed7aa`         | `#fed7aa`         |
| color.filled.cat5.foreground.default | `{color.global.orange.700}`                 | `#c2410c`         | `#c2410c`         |
| color.filled.cat5.foreground.pressed | `{color.global.orange.800}`                 | `#9a3412`         | `#9a3412`         |
| color.filled.cat5.border.default     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.filled.cat5.border.pressed     | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.cat1.background.default  | `{color.global.transparent.0}`              | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.cat1.background.pressed  | `{color.global.gray.200}`                   | `#dfe2e7`         | `#dfe2e7`         |
| color.ghost.cat1.foreground.default  | `{color.global.gray.600}`                   | `#4b5563`         | `#4b5563`         |
| color.ghost.cat1.foreground.pressed  | `{color.global.gray.700}`                   | `#374151`         | `#374151`         |
| color.ghost.cat1.border.default      | `{tag.color.ghost.cat1.background.default}` | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.cat1.border.pressed      | `{tag.color.ghost.cat1.background.pressed}` | `#dfe2e7`         | `#dfe2e7`         |

## badge

**Dimensions / radius / width**

| Token                | Alias                  | Value   |
| -------------------- | ---------------------- | ------- |
| borderRadius.default | `{borderRadius.round}` | `999px` |

**Colors**

| Token                                | Alias                              | Light             | Dark              |
| ------------------------------------ | ---------------------------------- | ----------------- | ----------------- |
| color.informative.background.default | `{color.utility.info.subtle}`      | `#dbeafe`         | `#172554`         |
| color.informative.foreground.default | `{color.text.utility.info.strong}` | `#1e40af`         | `#60a5fa`         |
| color.positive.background.default    | `{color.utility.success.subtle}`   | `#dcfce7`         | `#052e16`         |
| color.positive.foreground.default    | `{color.utility.success.strong}`   | `#166534`         | `#bbf7d0`         |
| color.warning.background.default     | `{color.utility.warning.subtle}`   | `#ffedd5`         | `#431407`         |
| color.warning.foreground.default     | `{color.utility.warning.strong}`   | `#9a3412`         | `#fed7aa`         |
| color.negative.background.default    | `{color.utility.danger.subtle}`    | `#fee2e2`         | `#450a0a`         |
| color.negative.foreground.default    | `{color.utility.danger.strong}`    | `#991b1b`         | `#fecaca`         |
| color.neutral.background.default     | `{color.neutralPalette.muted}`     | `#f3f4f6`         | `#1f2937`         |
| color.neutral.foreground.default     | `{color.neutralPalette.heavy}`     | `#1f2937`         | `#f3f4f6`         |
| color.ghost.background.default       | `{color.global.transparent.0}`     | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.foreground.default       | `{color.neutralPalette.heavy}`     | `#1f2937`         | `#f3f4f6`         |

## chip

**Dimensions / radius / width**

| Token                | Alias                  | Value   |
| -------------------- | ---------------------- | ------- |
| borderRadius.default | `{borderRadius.round}` | `999px` |
| borderWidth.default  | `{borderWidth.sm}`     | `1px`   |
| gap.default          | `{gap.sm}`             | `8px`   |

**Typography**

| Token              | Family | Weight | Size | Line height |
| ------------------ | ------ | ------ | ---- | ----------- |
| typography.label   | Inter  | 500    | 14   | 14px        |
| typography.counter | Inter  | 500    | 12   | 12px        |

**Colors**

| Token                                | Alias                                                | Light     | Dark      |
| ------------------------------------ | ---------------------------------------------------- | --------- | --------- |
| color.inputChip.background.default   | `{color.action.neutral.default.background.default}`  | `#ffffff` | `#111827` |
| color.inputChip.background.hover     | `{color.action.neutral.default.background.hover}`    | `#f3f4f6` | `#1f2937` |
| color.inputChip.background.pressed   | `{color.action.neutral.default.background.pressed}`  | `#dfe2e7` | `#374151` |
| color.inputChip.background.selected  | `{color.action.brand.background.default}`            | `#3d3e9f` | `#4647b1` |
| color.inputChip.background.disabled  | `{color.action.neutral.default.background.disabled}` | `#f3f4f6` | `#1f2937` |
| color.inputChip.border.default       | `{color.neutralPalette.subtle}`                      | `#d1d5db` | `#374151` |
| color.inputChip.border.hover         | `{color.action.neutral.default.border.hover}`        | `#d1d5db` | `#374151` |
| color.inputChip.border.pressed       | `{color.action.neutral.default.border.pressed}`      | `#9ca3af` | `#4b5563` |
| color.inputChip.border.selected      | `{chip.color.inputChip.background.selected}`         | `#3d3e9f` | `#4647b1` |
| color.inputChip.border.disabled      | `{color.action.neutral.default.border.disabled}`     | `#dfe2e7` | `#374151` |
| color.inputChip.foreground.default   | `{color.action.neutral.default.foreground.default}`  | `#1f2937` | `#f3f4f6` |
| color.inputChip.foreground.hover     | `{color.action.neutral.default.foreground.hover}`    | `#1f2937` | `#f3f4f6` |
| color.inputChip.foreground.pressed   | `{color.action.neutral.default.foreground.pressed}`  | `#1f2937` | `#f3f4f6` |
| color.inputChip.foreground.selected  | `{color.action.brand.foreground.default}`            | `#f9fafb` | `#f3f4f6` |
| color.inputChip.foreground.disabled  | `{color.action.neutral.default.foreground.disabled}` | `#9ca3af` | `#6b7280` |
| color.filterChip.background.default  | `{color.action.neutral.default.background.default}`  | `#ffffff` | `#111827` |
| color.filterChip.background.hover    | `{color.action.neutral.default.background.hover}`    | `#f3f4f6` | `#1f2937` |
| color.filterChip.background.pressed  | `{color.action.neutral.default.background.pressed}`  | `#dfe2e7` | `#374151` |
| color.filterChip.background.selected | `{color.action.brand.background.default}`            | `#3d3e9f` | `#4647b1` |
| color.filterChip.background.disabled | `{color.action.neutral.default.background.disabled}` | `#f3f4f6` | `#1f2937` |
| color.filterChip.border.default      | `{color.neutralPalette.subtle}`                      | `#d1d5db` | `#374151` |
| color.filterChip.border.hover        | `{color.action.neutral.default.border.hover}`        | `#d1d5db` | `#374151` |
| color.filterChip.border.pressed      | `{color.action.neutral.default.border.pressed}`      | `#9ca3af` | `#4b5563` |
| color.filterChip.border.selected     | `{chip.color.inputChip.background.selected}`         | `#3d3e9f` | `#4647b1` |
| color.filterChip.border.disabled     | `{color.action.neutral.default.border.disabled}`     | `#dfe2e7` | `#374151` |
| color.filterChip.foreground.default  | `{color.action.neutral.default.foreground.default}`  | `#1f2937` | `#f3f4f6` |
| color.filterChip.foreground.hover    | `{color.action.neutral.default.foreground.hover}`    | `#1f2937` | `#f3f4f6` |
| color.filterChip.foreground.pressed  | `{color.action.neutral.default.foreground.pressed}`  | `#1f2937` | `#f3f4f6` |
| color.filterChip.foreground.selected | `{color.action.brand.foreground.default}`            | `#f9fafb` | `#f3f4f6` |
| color.filterChip.foreground.disabled | `{color.action.neutral.default.foreground.disabled}` | `#9ca3af` | `#6b7280` |
| color.actionChip.background.default  | `{color.action.neutral.default.background.default}`  | `#ffffff` | `#111827` |
| color.actionChip.background.hover    | `{color.action.neutral.default.background.hover}`    | `#f3f4f6` | `#1f2937` |
| color.actionChip.background.pressed  | `{color.action.neutral.default.background.pressed}`  | `#dfe2e7` | `#374151` |
| color.actionChip.background.selected | `{color.action.brand.background.default}`            | `#3d3e9f` | `#4647b1` |
| color.actionChip.background.disabled | `{color.action.neutral.default.background.disabled}` | `#f3f4f6` | `#1f2937` |
| color.actionChip.border.default      | `{color.neutralPalette.subtle}`                      | `#d1d5db` | `#374151` |
| color.actionChip.border.hover        | `{color.action.neutral.default.border.hover}`        | `#d1d5db` | `#374151` |
| color.actionChip.border.pressed      | `{color.action.neutral.default.border.pressed}`      | `#9ca3af` | `#4b5563` |
| color.actionChip.border.selected     | `{chip.color.inputChip.background.selected}`         | `#3d3e9f` | `#4647b1` |
| color.actionChip.border.disabled     | `{color.action.neutral.default.border.disabled}`     | `#dfe2e7` | `#374151` |
| color.actionChip.foreground.default  | `{color.action.neutral.default.foreground.default}`  | `#1f2937` | `#f3f4f6` |
| color.actionChip.foreground.hover    | `{color.action.neutral.default.foreground.hover}`    | `#1f2937` | `#f3f4f6` |
| color.actionChip.foreground.pressed  | `{color.action.neutral.default.foreground.pressed}`  | `#1f2937` | `#f3f4f6` |
| color.actionChip.foreground.selected | `{color.action.brand.foreground.default}`            | `#f9fafb` | `#f3f4f6` |
| color.actionChip.foreground.disabled | `{color.action.neutral.default.foreground.disabled}` | `#9ca3af` | `#6b7280` |

## chart

**Dimensions / radius / width**

| Token                                       | Alias               | Value  |
| ------------------------------------------- | ------------------- | ------ |
| size.lineChart.pointMarker.default          | `{dimension.8px}`   | `8px`  |
| size.lineChart.pointMarker.highlight        | `{dimension.10px}`  | `10px` |
| borderRadius.barChart.default               | `{borderRadius.sm}` | `8px`  |
| borderWidth.grid.line.horizontal            | `{borderWidth.sm}`  | `1px`  |
| borderWidth.grid.line.vertical              | `{borderWidth.sm}`  | `1px`  |
| borderWidth.lineChart.line.default          | `{borderWidth.md}`  | `2px`  |
| borderWidth.lineChart.line.highlight        | `{borderWidth.lg}`  | `4px`  |
| borderWidth.lineChart.pointMarker.default   | `{borderWidth.md}`  | `2px`  |
| borderWidth.lineChart.pointMarker.highlight | `{borderWidth.md}`  | `2px`  |

**Typography**

| Token                         | Family | Weight | Size | Line height |
| ----------------------------- | ------ | ------ | ---- | ----------- |
| typography.axis.label.default | Inter  | 400    | 10   | 14px        |

**Colors**

| Token                               | Alias                                  | Light     | Dark      |
| ----------------------------------- | -------------------------------------- | --------- | --------- |
| color.axis.label.default            | `{color.text.neutral.onLight.muted}`   | `#9ca3af` | `#6b7280` |
| color.axis.label.highlight          | `{color.text.neutral.onLight.default}` | `#1f2937` | `#f3f4f6` |
| color.grid.line.horizontal          | `{color.surface.neutral.border.base}`  | `#dfe2e7` | `#374151` |
| color.grid.line.vertical            | `{color.surface.neutral.border.base}`  | `#dfe2e7` | `#374151` |
| color.series.1.default              | `{color.dataviz.blue.medium}`          | `#60a5fa` | `#60a5fa` |
| color.series.1.highlight            | `{color.dataviz.blue.strong}`          | `#3b82f6` | `#93c5fd` |
| color.series.1.dimmed               | `{color.dataviz.blue.subtle}`          | `#93c5fd` | `#3b82f6` |
| color.series.2.default              | `{color.dataviz.red.medium}`           | `#f87171` | `#f87171` |
| color.series.2.highlight            | `{color.dataviz.red.strong}`           | `#ef4444` | `#fca5a5` |
| color.series.2.dimmed               | `{color.dataviz.red.subtle}`           | `#fca5a5` | `#ef4444` |
| color.series.3.default              | `{color.dataviz.green.medium}`         | `#4ade80` | `#4ade80` |
| color.series.3.highlight            | `{color.dataviz.green.strong}`         | `#22c55e` | `#86efac` |
| color.series.3.dimmed               | `{color.dataviz.green.subtle}`         | `#86efac` | `#22c55e` |
| color.series.4.default              | `{color.dataviz.yellow.medium}`        | `#facc15` | `#facc15` |
| color.series.4.highlight            | `{color.dataviz.yellow.strong}`        | `#eab308` | `#fde047` |
| color.series.4.dimmed               | `{color.dataviz.yellow.subtle}`        | `#fde047` | `#eab308` |
| color.series.5.default              | `{color.dataviz.pink.medium}`          | `#f472b6` | `#f472b6` |
| color.series.5.highlight            | `{color.dataviz.pink.strong}`          | `#ec4899` | `#f9a8d4` |
| color.series.5.dimmed               | `{color.dataviz.pink.subtle}`          | `#f9a8d4` | `#ec4899` |
| color.series.positive.default       | `{color.dataviz.green.medium}`         | `#4ade80` | `#4ade80` |
| color.series.positive.highlight     | `{color.dataviz.green.strong}`         | `#22c55e` | `#86efac` |
| color.series.positive.dimmed        | `{color.dataviz.green.subtle}`         | `#86efac` | `#22c55e` |
| color.series.negative.default       | `{color.dataviz.red.medium}`           | `#f87171` | `#f87171` |
| color.series.negative.highlight     | `{color.dataviz.red.strong}`           | `#ef4444` | `#fca5a5` |
| color.series.negative.dimmed        | `{color.dataviz.red.subtle}`           | `#fca5a5` | `#ef4444` |
| color.series.warning.default        | `{color.dataviz.orange.medium}`        | `#fb923c` | `#fb923c` |
| color.series.warning.highlight      | `{color.dataviz.orange.strong}`        | `#f97316` | `#fdba74` |
| color.series.warning.dimmed         | `{color.dataviz.orange.subtle}`        | `#fdba74` | `#f97316` |
| color.series.neutral.default        | `{color.dataviz.blue.medium}`          | `#60a5fa` | `#60a5fa` |
| color.series.neutral.highlight      | `{color.dataviz.blue.strong}`          | `#3b82f6` | `#93c5fd` |
| color.series.neutral.dimmed         | `{color.dataviz.blue.subtle}`          | `#93c5fd` | `#3b82f6` |
| color.lineChart.marker.fill.default | `{color.neutralPalette.pure}`          | `#ffffff` | `#000000` |

## iconButton

**Dimensions / radius / width**

| Token                 | Alias                               | Value   |
| --------------------- | ----------------------------------- | ------- |
| borderRadius.default  | `{borderRadius.round}`              | `999px` |
| borderRadius.hover    | `{iconButton.borderRadius.default}` | `999px` |
| borderRadius.pressed  | `{iconButton.borderRadius.default}` | `999px` |
| borderRadius.disabled | `{iconButton.borderRadius.default}` | `999px` |
| borderWidth.default   | `{borderWidth.sm}`                  | `1px`   |

**Colors**

| Token                                    | Alias                                                  | Light             | Dark              |
| ---------------------------------------- | ------------------------------------------------------ | ----------------- | ----------------- |
| color.primary.background.default         | `{color.action.brand.background.default}`              | `#3d3e9f`         | `#4647b1`         |
| color.primary.background.hover           | `{color.action.brand.background.hover}`                | `#32348c`         | `#3d3e9f`         |
| color.primary.background.pressed         | `{color.action.brand.background.pressed}`              | `#292b79`         | `#32348c`         |
| color.primary.background.disabled        | `{color.action.brand.background.disabled}`             | `#a8a9e3`         | `#202266`         |
| color.primary.border.default             | `{iconButton.color.primary.background.default}`        | `#3d3e9f`         | `#4647b1`         |
| color.primary.border.hover               | `{iconButton.color.primary.background.hover}`          | `#32348c`         | `#3d3e9f`         |
| color.primary.border.pressed             | `{iconButton.color.primary.background.pressed}`        | `#292b79`         | `#32348c`         |
| color.primary.border.disabled            | `{color.action.brand.border.disabled}`                 | `#a8a9e3`         | `#202266`         |
| color.primary.foreground.default         | `{color.action.brand.foreground.default}`              | `#f9fafb`         | `#f3f4f6`         |
| color.primary.foreground.hover           | `{color.action.brand.foreground.hover}`                | `#f9fafb`         | `#f3f4f6`         |
| color.primary.foreground.pressed         | `{color.action.brand.foreground.pressed}`              | `#f9fafb`         | `#f3f4f6`         |
| color.primary.foreground.disabled        | `{color.action.brand.foreground.disabled}`             | `#f9fafb`         | `#6b7280`         |
| color.secondary.background.default       | `{color.action.neutral.default.background.default}`    | `#ffffff`         | `#111827`         |
| color.secondary.background.hover         | `{color.action.neutral.default.background.hover}`      | `#f3f4f6`         | `#1f2937`         |
| color.secondary.background.pressed       | `{color.action.neutral.default.background.pressed}`    | `#dfe2e7`         | `#374151`         |
| color.secondary.background.disabled      | `{color.action.neutral.default.background.disabled}`   | `#f3f4f6`         | `#1f2937`         |
| color.secondary.border.default           | `{color.action.neutral.default.border.default}`        | `#dfe2e7`         | `#374151`         |
| color.secondary.border.hover             | `{color.action.neutral.default.border.hover}`          | `#d1d5db`         | `#374151`         |
| color.secondary.border.pressed           | `{color.action.neutral.default.border.pressed}`        | `#9ca3af`         | `#4b5563`         |
| color.secondary.border.disabled          | `{color.action.neutral.default.border.disabled}`       | `#dfe2e7`         | `#374151`         |
| color.secondary.foreground.default       | `{color.action.neutral.default.foreground.default}`    | `#1f2937`         | `#f3f4f6`         |
| color.secondary.foreground.hover         | `{color.action.neutral.default.foreground.hover}`      | `#1f2937`         | `#f3f4f6`         |
| color.secondary.foreground.pressed       | `{color.action.neutral.default.foreground.pressed}`    | `#1f2937`         | `#f3f4f6`         |
| color.secondary.foreground.disabled      | `{color.action.neutral.default.foreground.disabled}`   | `#9ca3af`         | `#6b7280`         |
| color.elevated.background.default        | `{color.action.neutral.elevated.background.default}`   | `#f3f4f6`         | `#1f2937`         |
| color.elevated.background.hover          | `{color.action.neutral.elevated.background.hover}`     | `#dfe2e7`         | `#374151`         |
| color.elevated.background.pressed        | `{color.action.neutral.elevated.background.pressed}`   | `#d1d5db`         | `#4b5563`         |
| color.elevated.background.disabled       | `{iconButton.color.secondary.background.disabled}`     | `#f3f4f6`         | `#1f2937`         |
| color.elevated.border.default            | `{color.action.neutral.elevated.border.default}`       | `#d1d5db`         | `#4b5563`         |
| color.elevated.border.hover              | `{color.action.neutral.elevated.border.hover}`         | `#9ca3af`         | `#4b5563`         |
| color.elevated.border.pressed            | `{color.action.neutral.elevated.border.pressed}`       | `#6b7280`         | `#6b7280`         |
| color.elevated.border.disabled           | `{iconButton.color.secondary.border.disabled}`         | `#dfe2e7`         | `#374151`         |
| color.elevated.foreground.default        | `{color.action.neutral.default.foreground.default}`    | `#1f2937`         | `#f3f4f6`         |
| color.elevated.foreground.hover          | `{color.action.neutral.default.foreground.hover}`      | `#1f2937`         | `#f3f4f6`         |
| color.elevated.foreground.pressed        | `{color.action.neutral.default.foreground.pressed}`    | `#1f2937`         | `#f3f4f6`         |
| color.elevated.foreground.disabled       | `{iconButton.color.secondary.foreground.disabled}`     | `#9ca3af`         | `#6b7280`         |
| color.ghost.background.default           | `{color.global.transparent.0}`                         | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.background.hover             | `{iconButton.color.secondary.background.hover}`        | `#f3f4f6`         | `#1f2937`         |
| color.ghost.background.pressed           | `{iconButton.color.secondary.background.pressed}`      | `#dfe2e7`         | `#374151`         |
| color.ghost.background.disabled          | `{iconButton.color.ghost.background.default}`          | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.border.default               | `{iconButton.color.ghost.background.default}`          | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.border.hover                 | `{iconButton.color.secondary.background.hover}`        | `#f3f4f6`         | `#1f2937`         |
| color.ghost.border.pressed               | `{iconButton.color.secondary.background.pressed}`      | `#dfe2e7`         | `#374151`         |
| color.ghost.border.disabled              | `{iconButton.color.ghost.background.disabled}`         | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.ghost.foreground.default           | `{color.action.neutral.default.foreground.default}`    | `#1f2937`         | `#f3f4f6`         |
| color.ghost.foreground.hover             | `{color.action.neutral.default.foreground.hover}`      | `#1f2937`         | `#f3f4f6`         |
| color.ghost.foreground.pressed           | `{color.action.neutral.default.foreground.pressed}`    | `#1f2937`         | `#f3f4f6`         |
| color.ghost.foreground.disabled          | `{iconButton.color.secondary.foreground.disabled}`     | `#9ca3af`         | `#6b7280`         |
| color.danger-primary.background.default  | `{color.action.danger.background.default}`             | `#dc2626`         | `#dc2626`         |
| color.danger-primary.background.hover    | `{color.action.danger.background.hover}`               | `#b91c1c`         | `#b91c1c`         |
| color.danger-primary.background.pressed  | `{color.action.danger.background.pressed}`             | `#991b1b`         | `#991b1b`         |
| color.danger-primary.background.disabled | `{color.action.danger.background.disabled}`            | `#f3f4f6`         | `#1f2937`         |
| color.danger-primary.border.default      | `{iconButton.color.danger-primary.background.default}` | `#dc2626`         | `#dc2626`         |
| color.danger-primary.border.hover        | `{iconButton.color.danger-primary.background.hover}`   | `#b91c1c`         | `#b91c1c`         |
| color.danger-primary.border.pressed      | `{iconButton.color.danger-primary.background.pressed}` | `#991b1b`         | `#991b1b`         |
| color.danger-primary.border.disabled     | `{color.action.danger.border.disabled}`                | `#f3f4f6`         | `#374151`         |
| color.danger-primary.foreground.default  | `{color.action.danger.foreground.default}`             | `#f9fafb`         | `#f3f4f6`         |
| color.danger-primary.foreground.hover    | `{color.action.danger.foreground.hover}`               | `#f9fafb`         | `#f3f4f6`         |
| color.danger-primary.foreground.pressed  | `{color.action.danger.foreground.pressed}`             | `#f9fafb`         | `#f3f4f6`         |
| color.danger-primary.foreground.disabled | `{color.action.danger.foreground.disabled}`            | `#9ca3af`         | `#6b7280`         |
| color.danger-ghost.background.default    | `{color.global.transparent.0}`                         | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.danger-ghost.background.hover      | `{iconButton.color.danger-primary.background.hover}`   | `#b91c1c`         | `#b91c1c`         |
| color.danger-ghost.background.pressed    | `{iconButton.color.danger-primary.background.pressed}` | `#991b1b`         | `#991b1b`         |
| color.danger-ghost.background.disabled   | `{iconButton.color.danger-ghost.background.default}`   | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.danger-ghost.border.default        | `{iconButton.color.danger-ghost.background.default}`   | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.danger-ghost.border.hover          | `{iconButton.color.danger-ghost.background.hover}`     | `#b91c1c`         | `#b91c1c`         |
| color.danger-ghost.border.pressed        | `{iconButton.color.danger-ghost.background.pressed}`   | `#991b1b`         | `#991b1b`         |
| color.danger-ghost.border.disabled       | `{iconButton.color.danger-ghost.background.disabled}`  | `rgba(0,0,0,0.0)` | `rgba(0,0,0,0.0)` |
| color.danger-ghost.foreground.default    | `{color.text.utility.danger.subtle}`                   | `#dc2626`         | `#ef4444`         |
| color.danger-ghost.foreground.hover      | `{iconButton.color.danger-primary.foreground.hover}`   | `#f9fafb`         | `#f3f4f6`         |
| color.danger-ghost.foreground.pressed    | `{iconButton.color.danger-primary.foreground.pressed}` | `#f9fafb`         | `#f3f4f6`         |
| color.danger-ghost.foreground.disabled   | `{iconButton.color.secondary.foreground.disabled}`     | `#9ca3af`         | `#6b7280`         |

## listItem

**Dimensions / radius / width**

| Token                 | Alias                             | Value  |
| --------------------- | --------------------------------- | ------ |
| borderRadius.default  | `{borderRadius.md}`               | `12px` |
| borderRadius.hover    | `{listItem.borderRadius.default}` | `12px` |
| borderRadius.pressed  | `{listItem.borderRadius.default}` | `12px` |
| borderRadius.disabled | `{listItem.borderRadius.default}` | `12px` |
| borderWidth.default   | `{borderWidth.sm}`                | `1px`  |
| padding.default       | `{padding.lg}`                    | `16px` |

**Colors**

| Token                              | Alias                                               | Light     | Dark      |
| ---------------------------------- | --------------------------------------------------- | --------- | --------- |
| color.default.background.default   | `{color.action.neutral.default.background.default}` | `#ffffff` | `#111827` |
| color.default.background.hover     | `{color.action.neutral.default.background.hover}`   | `#f3f4f6` | `#1f2937` |
| color.default.background.pressed   | `{color.action.neutral.default.background.pressed}` | `#dfe2e7` | `#374151` |
| color.default.background.disabled  | `{listItem.color.default.background.default}`       | `#ffffff` | `#111827` |
| color.default.border.default       | `{color.action.neutral.default.border.default}`     | `#dfe2e7` | `#374151` |
| color.default.border.hover         | `{color.action.neutral.default.border.hover}`       | `#d1d5db` | `#374151` |
| color.default.border.pressed       | `{color.action.neutral.default.border.pressed}`     | `#9ca3af` | `#4b5563` |
| color.default.border.disabled      | `{listItem.color.default.border.default}`           | `#dfe2e7` | `#374151` |
| color.default.title.default        | `{color.text.neutral.onLight.default}`              | `#1f2937` | `#f3f4f6` |
| color.default.title.hover          | `{color.text.neutral.onLight.default}`              | `#1f2937` | `#f3f4f6` |
| color.default.title.pressed        | `{color.text.neutral.onLight.default}`              | `#1f2937` | `#f3f4f6` |
| color.default.title.disabled       | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.default.subtitle.default     | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.default.subtitle.hover       | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.default.subtitle.pressed     | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.default.subtitle.disabled    | `{color.text.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.default.icon.default         | `{color.icon.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.default.icon.hover           | `{color.icon.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.default.icon.pressed         | `{color.icon.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.default.icon.disabled        | `{color.icon.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.default.iconBg.default       | `{color.neutralPalette.muted}`                      | `#f3f4f6` | `#1f2937` |
| color.default.iconBg.hover         | `{color.neutralPalette.muted}`                      | `#f3f4f6` | `#1f2937` |
| color.default.iconBg.pressed       | `{color.neutralPalette.muted}`                      | `#f3f4f6` | `#1f2937` |
| color.default.iconBg.disabled      | `{color.neutralPalette.muted}`                      | `#f3f4f6` | `#1f2937` |
| color.default.detail.default       | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.default.detail.hover         | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.default.detail.pressed       | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.default.detail.disabled      | `{color.text.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.default.drill-in.default     | `{color.text.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.default.drill-in.hover       | `{color.text.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.default.drill-in.pressed     | `{color.text.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.default.drill-in.disabled    | `{color.neutralPalette.subtle}`                     | `#d1d5db` | `#374151` |
| color.default.iconInfo.default     | `{color.icon.utility.info.subtle}`                  | `#2563eb` | `#3b82f6` |
| color.default.iconInfo.hover       | `{color.icon.utility.info.subtle}`                  | `#2563eb` | `#3b82f6` |
| color.default.iconInfo.pressed     | `{color.icon.utility.info.subtle}`                  | `#2563eb` | `#3b82f6` |
| color.default.iconInfo.disabled    | `{color.icon.utility.info.muted}`                   | `#60a5fa` | `#1d4ed8` |
| color.default.iconDanger.default   | `{color.icon.utility.danger.subtle}`                | `#dc2626` | `#ef4444` |
| color.default.iconDanger.hover     | `{color.icon.utility.danger.subtle}`                | `#dc2626` | `#ef4444` |
| color.default.iconDanger.pressed   | `{color.icon.utility.danger.subtle}`                | `#dc2626` | `#ef4444` |
| color.default.iconDanger.disabled  | `{color.icon.utility.danger.muted}`                 | `#f87171` | `#b91c1c` |
| color.selected.background.default  | `{color.action.neutral.default.background.default}` | `#ffffff` | `#111827` |
| color.selected.background.hover    | `{color.action.neutral.default.background.hover}`   | `#f3f4f6` | `#1f2937` |
| color.selected.background.pressed  | `{color.action.neutral.default.background.pressed}` | `#dfe2e7` | `#374151` |
| color.selected.background.disabled | `{listItem.color.selected.background.default}`      | `#ffffff` | `#111827` |
| color.selected.border.default      | `{color.action.neutral.selected.border.default}`    | `#374151` | `#dfe2e7` |
| color.selected.border.hover        | `{color.action.neutral.selected.border.hover}`      | `#1f2937` | `#f3f4f6` |
| color.selected.border.pressed      | `{color.action.neutral.selected.border.pressed}`    | `#111827` | `#f9fafb` |
| color.selected.border.disabled     | `{color.action.neutral.selected.border.disabled}`   | `#d1d5db` | `#4b5563` |
| color.selected.title.default       | `{color.text.neutral.onLight.default}`              | `#1f2937` | `#f3f4f6` |
| color.selected.title.hover         | `{color.text.neutral.onLight.default}`              | `#1f2937` | `#f3f4f6` |
| color.selected.title.pressed       | `{color.text.neutral.onLight.default}`              | `#1f2937` | `#f3f4f6` |
| color.selected.title.disabled      | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.selected.subtitle.default    | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.selected.subtitle.hover      | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.selected.subtitle.pressed    | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.selected.subtitle.disabled   | `{color.text.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.selected.icon.default        | `{color.icon.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.selected.icon.hover          | `{color.icon.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.selected.icon.pressed        | `{color.icon.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.selected.icon.disabled       | `{color.icon.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.selected.iconBg.default      | `{color.neutralPalette.muted}`                      | `#f3f4f6` | `#1f2937` |
| color.selected.iconBg.hover        | `{color.neutralPalette.muted}`                      | `#f3f4f6` | `#1f2937` |
| color.selected.iconBg.pressed      | `{color.neutralPalette.muted}`                      | `#f3f4f6` | `#1f2937` |
| color.selected.iconBg.disabled     | `{color.neutralPalette.muted}`                      | `#f3f4f6` | `#1f2937` |
| color.selected.detail.default      | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.selected.detail.hover        | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.selected.detail.pressed      | `{color.text.neutral.onLight.subtle}`               | `#6b7280` | `#9ca3af` |
| color.selected.detail.disabled     | `{color.text.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.selected.drill-in.default    | `{color.text.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.selected.drill-in.hover      | `{color.text.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.selected.drill-in.pressed    | `{color.text.neutral.onLight.muted}`                | `#9ca3af` | `#6b7280` |
| color.selected.drill-in.disabled   | `{color.neutralPalette.subtle}`                     | `#d1d5db` | `#374151` |
| color.selected.iconInfo.default    | `{color.icon.utility.info.subtle}`                  | `#2563eb` | `#3b82f6` |
| color.selected.iconInfo.hover      | `{color.icon.utility.info.subtle}`                  | `#2563eb` | `#3b82f6` |
| color.selected.iconInfo.pressed    | `{color.icon.utility.info.subtle}`                  | `#2563eb` | `#3b82f6` |
| color.selected.iconInfo.disabled   | `{color.icon.utility.info.muted}`                   | `#60a5fa` | `#1d4ed8` |
| color.selected.iconDanger.default  | `{color.icon.utility.danger.subtle}`                | `#dc2626` | `#ef4444` |
| color.selected.iconDanger.hover    | `{color.icon.utility.danger.subtle}`                | `#dc2626` | `#ef4444` |
| color.selected.iconDanger.pressed  | `{color.icon.utility.danger.subtle}`                | `#dc2626` | `#ef4444` |
| color.selected.iconDanger.disabled | `{color.icon.utility.danger.muted}`                 | `#f87171` | `#b91c1c` |

## container

**Dimensions / radius / width**

| Token                 | Alias                           | Value   |
| --------------------- | ------------------------------- | ------- |
| borderRadius.default  | `{borderRadius.md}`             | `12px`  |
| borderRadius.hover    | `{button.borderRadius.default}` | `999px` |
| borderRadius.pressed  | `{button.borderRadius.default}` | `999px` |
| borderRadius.disabled | `{button.borderRadius.default}` | `999px` |
| borderWidth.default   | `{borderWidth.sm}`              | `1px`   |
| padding.none          | `{dimension.0px}`               | `0px`   |
| padding.xs            | `{padding.xs}`                  | `4px`   |
| padding.sm            | `{padding.sm}`                  | `8px`   |
| padding.md            | `{padding.md}`                  | `12px`  |
| padding.lg            | `{padding.lg}`                  | `16px`  |
| padding.lgPlus        | `{padding.lgPlus}`              | `20px`  |
| padding.xl            | `{padding.xl}`                  | `24px`  |

**Colors**

| Token                             | Alias                                       | Light     | Dark      |
| --------------------------------- | ------------------------------------------- | --------- | --------- |
| color.default.background.default  | `{color.surface.neutral.background.level1}` | `#ffffff` | `#111827` |
| color.default.background.hover    | `{color.surface.neutral.background.level1}` | `#ffffff` | `#111827` |
| color.default.background.pressed  | `{color.surface.neutral.background.level1}` | `#ffffff` | `#111827` |
| color.default.background.disabled | `{color.surface.neutral.background.level1}` | `#ffffff` | `#111827` |
| color.default.border.default      | `{color.surface.neutral.border.level1}`     | `#dfe2e7` | `#374151` |
| color.default.border.hover        | `{color.surface.neutral.border.level1}`     | `#dfe2e7` | `#374151` |
| color.default.border.pressed      | `{color.surface.neutral.border.level1}`     | `#dfe2e7` | `#374151` |
| color.default.border.disabled     | `{color.surface.neutral.border.level1}`     | `#dfe2e7` | `#374151` |

## recorder

**Colors**

| Token                    | Alias                                 | Light     | Dark      |
| ------------------------ | ------------------------------------- | --------- | --------- |
| color.background.default | `{color.brand.primary.900}`           | `#181952` | `#181952` |
| color.border.default     | `{recorder.color.background.default}` | `#181952` | `#181952` |
| color.waveform.default   | `{color.global.blue.500}`             | `#3b82f6` | `#3b82f6` |
| color.waveform.paused    | `{color.global.blue.500}`             | `#3b82f6` | `#3b82f6` |
