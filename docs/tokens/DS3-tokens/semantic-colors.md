---
title: Semantic colors tokens (Light & Dark)
group: DS3 Tokens
nav_order: 4
---

Mode-specific color tokens. Each row shows the alias (reference) and the resolved hex for **Light** and **Dark** modes. Sources: `tokens/mode/light.json`, `tokens/mode/dark.json`.

## action

Interactive element colors (buttons, controls) by intent and state.

| Token                                       | Light alias                                 | Light     | Dark alias                                 | Dark      |
| ------------------------------------------- | ------------------------------------------- | --------- | ------------------------------------------ | --------- |
| action.brand.background.default             | `{color.brand.primary.500}`                 | `#3d3e9f` | `{color.brand.primary.400}`                | `#4647b1` |
| action.brand.background.hover               | `{color.brand.primary.600}`                 | `#32348c` | `{color.brand.primary.500}`                | `#3d3e9f` |
| action.brand.background.pressed             | `{color.brand.primary.700}`                 | `#292b79` | `{color.brand.primary.600}`                | `#32348c` |
| action.brand.background.disabled            | `{color.brand.primary.200}`                 | `#a8a9e3` | `{color.brand.primary.800}`                | `#202266` |
| action.brand.border.default                 | `{color.action.brand.background.default}`   | `#3d3e9f` | `{color.action.brand.background.default}`  | `#4647b1` |
| action.brand.border.hover                   | `{color.action.brand.background.hover}`     | `#32348c` | `{color.action.brand.background.hover}`    | `#3d3e9f` |
| action.brand.border.pressed                 | `{color.action.brand.background.pressed}`   | `#292b79` | `{color.action.brand.background.pressed}`  | `#32348c` |
| action.brand.border.disabled                | `{color.action.brand.background.disabled}`  | `#a8a9e3` | `{color.action.brand.background.disabled}` | `#202266` |
| action.brand.foreground.default             | `{color.text.neutral.onDark.default}`       | `#f9fafb` | `{color.text.neutral.onLight.default}`     | `#f3f4f6` |
| action.brand.foreground.hover               | `{color.text.neutral.onDark.default}`       | `#f9fafb` | `{color.text.neutral.onLight.default}`     | `#f3f4f6` |
| action.brand.foreground.pressed             | `{color.text.neutral.onDark.default}`       | `#f9fafb` | `{color.text.neutral.onLight.default}`     | `#f3f4f6` |
| action.brand.foreground.disabled            | `{color.text.neutral.onDark.default}`       | `#f9fafb` | `{color.text.neutral.onLight.muted}`       | `#6b7280` |
| action.neutral.default.background.default   | `{color.global.neutral.white}`              | `#ffffff` | `{color.global.gray.900}`                  | `#111827` |
| action.neutral.default.background.hover     | `{color.global.gray.100}`                   | `#f3f4f6` | `{color.global.gray.800}`                  | `#1f2937` |
| action.neutral.default.background.pressed   | `{color.global.gray.200}`                   | `#dfe2e7` | `{color.global.gray.700}`                  | `#374151` |
| action.neutral.default.background.disabled  | `{color.global.gray.100}`                   | `#f3f4f6` | `{color.global.gray.800}`                  | `#1f2937` |
| action.neutral.default.border.default       | `{color.global.gray.200}`                   | `#dfe2e7` | `{color.global.gray.700}`                  | `#374151` |
| action.neutral.default.border.hover         | `{color.global.gray.300}`                   | `#d1d5db` | `{color.global.gray.700}`                  | `#374151` |
| action.neutral.default.border.pressed       | `{color.global.gray.400}`                   | `#9ca3af` | `{color.global.gray.600}`                  | `#4b5563` |
| action.neutral.default.border.disabled      | `{color.global.gray.200}`                   | `#dfe2e7` | `{color.global.gray.700}`                  | `#374151` |
| action.neutral.default.foreground.default   | `{color.text.neutral.onLight.default}`      | `#1f2937` | `{color.text.neutral.onLight.default}`     | `#f3f4f6` |
| action.neutral.default.foreground.hover     | `{color.text.neutral.onLight.default}`      | `#1f2937` | `{color.text.neutral.onLight.default}`     | `#f3f4f6` |
| action.neutral.default.foreground.pressed   | `{color.text.neutral.onLight.default}`      | `#1f2937` | `{color.text.neutral.onLight.default}`     | `#f3f4f6` |
| action.neutral.default.foreground.disabled  | `{color.text.neutral.onLight.muted}`        | `#9ca3af` | `{color.text.neutral.onLight.muted}`       | `#6b7280` |
| action.neutral.elevated.background.default  | `{color.global.gray.100}`                   | `#f3f4f6` | `{color.global.gray.800}`                  | `#1f2937` |
| action.neutral.elevated.background.hover    | `{color.global.gray.200}`                   | `#dfe2e7` | `{color.global.gray.700}`                  | `#374151` |
| action.neutral.elevated.background.pressed  | `{color.global.gray.300}`                   | `#d1d5db` | `{color.global.gray.600}`                  | `#4b5563` |
| action.neutral.elevated.background.disabled | `{color.global.gray.200}`                   | `#dfe2e7` | `{color.global.gray.700}`                  | `#374151` |
| action.neutral.elevated.border.default      | `{color.global.gray.300}`                   | `#d1d5db` | `{color.global.gray.600}`                  | `#4b5563` |
| action.neutral.elevated.border.hover        | `{color.global.gray.400}`                   | `#9ca3af` | `{color.global.gray.600}`                  | `#4b5563` |
| action.neutral.elevated.border.pressed      | `{color.global.gray.500}`                   | `#6b7280` | `{color.global.gray.500}`                  | `#6b7280` |
| action.neutral.elevated.border.disabled     | `{color.global.gray.300}`                   | `#d1d5db` | `{color.global.gray.600}`                  | `#4b5563` |
| action.neutral.selected.background.default  | `{color.global.gray.700}`                   | `#374151` | `{color.global.gray.200}`                  | `#dfe2e7` |
| action.neutral.selected.background.hover    | `{color.global.gray.800}`                   | `#1f2937` | `{color.global.gray.100}`                  | `#f3f4f6` |
| action.neutral.selected.background.pressed  | `{color.global.gray.900}`                   | `#111827` | `{color.global.gray.50}`                   | `#f9fafb` |
| action.neutral.selected.background.disabled | `{color.global.gray.300}`                   | `#d1d5db` | `{color.global.gray.600}`                  | `#4b5563` |
| action.neutral.selected.border.default      | `{color.global.gray.700}`                   | `#374151` | `{color.global.gray.200}`                  | `#dfe2e7` |
| action.neutral.selected.border.hover        | `{color.global.gray.800}`                   | `#1f2937` | `{color.global.gray.100}`                  | `#f3f4f6` |
| action.neutral.selected.border.pressed      | `{color.global.gray.900}`                   | `#111827` | `{color.global.gray.50}`                   | `#f9fafb` |
| action.neutral.selected.border.disabled     | `{color.global.gray.300}`                   | `#d1d5db` | `{color.global.gray.600}`                  | `#4b5563` |
| action.danger.background.default            | `{color.global.red.600}`                    | `#dc2626` | `{color.global.red.600}`                   | `#dc2626` |
| action.danger.background.hover              | `{color.global.red.700}`                    | `#b91c1c` | `{color.global.red.700}`                   | `#b91c1c` |
| action.danger.background.pressed            | `{color.global.red.800}`                    | `#991b1b` | `{color.global.red.800}`                   | `#991b1b` |
| action.danger.background.disabled           | `{color.global.gray.100}`                   | `#f3f4f6` | `{color.global.gray.800}`                  | `#1f2937` |
| action.danger.border.default                | `{color.action.danger.background.default}`  | `#dc2626` | `{color.action.danger.background.default}` | `#dc2626` |
| action.danger.border.hover                  | `{color.action.danger.background.hover}`    | `#b91c1c` | `{color.action.danger.background.hover}`   | `#b91c1c` |
| action.danger.border.pressed                | `{color.action.danger.background.pressed}`  | `#991b1b` | `{color.action.danger.background.pressed}` | `#991b1b` |
| action.danger.border.disabled               | `{color.action.danger.background.disabled}` | `#f3f4f6` | `{color.global.gray.700}`                  | `#374151` |
| action.danger.foreground.default            | `{color.text.neutral.onDark.default}`       | `#f9fafb` | `{color.text.neutral.onLight.default}`     | `#f3f4f6` |
| action.danger.foreground.hover              | `{color.text.neutral.onDark.default}`       | `#f9fafb` | `{color.text.neutral.onLight.default}`     | `#f3f4f6` |
| action.danger.foreground.pressed            | `{color.text.neutral.onDark.default}`       | `#f9fafb` | `{color.text.neutral.onLight.default}`     | `#f3f4f6` |
| action.danger.foreground.disabled           | `{color.text.neutral.onDark.muted}`         | `#9ca3af` | `{color.text.neutral.onLight.muted}`       | `#6b7280` |

## text

Text colors by context (onDark/onLight) and emphasis.

| Token                        | Light alias                    | Light     | Dark alias                     | Dark      |
| ---------------------------- | ------------------------------ | --------- | ------------------------------ | --------- |
| text.brand.onDark.strong     | `{color.global.neutral.white}` | `#ffffff` | `{color.brand.primary.900}`    | `#181952` |
| text.brand.onDark.default    | `{color.brand.primary.100}`    | `#d6d7f5` | `{color.brand.primary.700}`    | `#292b79` |
| text.brand.onDark.subtle     | `{color.brand.primary.200}`    | `#a8a9e3` | `{color.brand.primary.600}`    | `#32348c` |
| text.brand.onDark.muted      | `{color.brand.primary.300}`    | `#7879cc` | `{color.brand.primary.300}`    | `#7879cc` |
| text.brand.onLight.strong    | `{color.brand.primary.900}`    | `#181952` | `{color.global.neutral.white}` | `#ffffff` |
| text.brand.onLight.default   | `{color.brand.primary.700}`    | `#292b79` | `{color.brand.primary.100}`    | `#d6d7f5` |
| text.brand.onLight.subtle    | `{color.brand.primary.600}`    | `#32348c` | `{color.brand.primary.200}`    | `#a8a9e3` |
| text.brand.onLight.muted     | `{color.brand.primary.300}`    | `#7879cc` | `{color.brand.primary.300}`    | `#7879cc` |
| text.neutral.onDark.strong   | `{color.global.neutral.white}` | `#ffffff` | `{color.global.neutral.black}` | `#000000` |
| text.neutral.onDark.default  | `{color.global.gray.50}`       | `#f9fafb` | `{color.global.gray.800}`      | `#1f2937` |
| text.neutral.onDark.subtle   | `{color.global.gray.300}`      | `#d1d5db` | `{color.global.gray.700}`      | `#374151` |
| text.neutral.onDark.muted    | `{color.global.gray.400}`      | `#9ca3af` | `{color.global.gray.500}`      | `#6b7280` |
| text.neutral.onLight.strong  | `{color.global.neutral.black}` | `#000000` | `{color.global.neutral.white}` | `#ffffff` |
| text.neutral.onLight.default | `{color.global.gray.800}`      | `#1f2937` | `{color.global.gray.100}`      | `#f3f4f6` |
| text.neutral.onLight.subtle  | `{color.global.gray.500}`      | `#6b7280` | `{color.global.gray.400}`      | `#9ca3af` |
| text.neutral.onLight.muted   | `{color.global.gray.400}`      | `#9ca3af` | `{color.global.gray.500}`      | `#6b7280` |
| text.utility.danger.strong   | `{color.global.red.800}`       | `#991b1b` | `{color.global.red.400}`       | `#f87171` |
| text.utility.danger.default  | `{color.global.red.700}`       | `#b91c1c` | `{color.global.red.400}`       | `#f87171` |
| text.utility.danger.subtle   | `{color.global.red.600}`       | `#dc2626` | `{color.global.red.500}`       | `#ef4444` |
| text.utility.danger.muted    | `{color.global.red.400}`       | `#f87171` | `{color.global.red.700}`       | `#b91c1c` |
| text.utility.warning.strong  | `{color.global.orange.800}`    | `#9a3412` | `{color.global.orange.400}`    | `#fb923c` |
| text.utility.warning.default | `{color.global.orange.700}`    | `#c2410c` | `{color.global.orange.400}`    | `#fb923c` |
| text.utility.warning.subtle  | `{color.global.orange.600}`    | `#ea580c` | `{color.global.orange.500}`    | `#f97316` |
| text.utility.warning.muted   | `{color.global.orange.400}`    | `#fb923c` | `{color.global.orange.700}`    | `#c2410c` |
| text.utility.success.strong  | `{color.global.green.800}`     | `#166534` | `{color.global.green.400}`     | `#4ade80` |
| text.utility.success.default | `{color.global.green.700}`     | `#15803d` | `{color.global.green.400}`     | `#4ade80` |
| text.utility.success.subtle  | `{color.global.green.600}`     | `#16a34a` | `{color.global.green.500}`     | `#22c55e` |
| text.utility.success.muted   | `{color.global.green.400}`     | `#4ade80` | `{color.global.green.700}`     | `#15803d` |
| text.utility.info.strong     | `{color.global.blue.800}`      | `#1e40af` | `{color.global.blue.400}`      | `#60a5fa` |
| text.utility.info.default    | `{color.global.blue.700}`      | `#1d4ed8` | `{color.global.blue.400}`      | `#60a5fa` |
| text.utility.info.subtle     | `{color.global.blue.600}`      | `#2563eb` | `{color.global.blue.500}`      | `#3b82f6` |
| text.utility.info.muted      | `{color.global.blue.400}`      | `#60a5fa` | `{color.global.blue.700}`      | `#1d4ed8` |

## icon

Icon colors, mostly aliasing text colors.

| Token                        | Light alias                            | Light     | Dark alias                             | Dark      |
| ---------------------------- | -------------------------------------- | --------- | -------------------------------------- | --------- |
| icon.neutral.onDark.strong   | `{color.text.neutral.onDark.strong}`   | `#ffffff` | `{color.text.neutral.onDark.strong}`   | `#000000` |
| icon.neutral.onDark.default  | `{color.text.neutral.onDark.default}`  | `#f9fafb` | `{color.text.neutral.onDark.default}`  | `#1f2937` |
| icon.neutral.onDark.subtle   | `{color.text.neutral.onDark.subtle}`   | `#d1d5db` | `{color.text.neutral.onDark.subtle}`   | `#374151` |
| icon.neutral.onDark.muted    | `{color.text.neutral.onDark.muted}`    | `#9ca3af` | `{color.text.neutral.onDark.muted}`    | `#6b7280` |
| icon.neutral.onLight.strong  | `{color.text.neutral.onLight.strong}`  | `#000000` | `{color.text.neutral.onLight.strong}`  | `#ffffff` |
| icon.neutral.onLight.default | `{color.text.neutral.onLight.default}` | `#1f2937` | `{color.text.neutral.onLight.default}` | `#f3f4f6` |
| icon.neutral.onLight.subtle  | `{color.text.neutral.onLight.subtle}`  | `#6b7280` | `{color.text.neutral.onLight.subtle}`  | `#9ca3af` |
| icon.neutral.onLight.muted   | `{color.text.neutral.onLight.muted}`   | `#9ca3af` | `{color.text.neutral.onLight.muted}`   | `#6b7280` |
| icon.brand.onDark.strong     | `{color.text.brand.onDark.strong}`     | `#ffffff` | `{color.text.brand.onDark.strong}`     | `#181952` |
| icon.brand.onDark.default    | `{color.text.brand.onDark.default}`    | `#d6d7f5` | `{color.text.brand.onDark.default}`    | `#292b79` |
| icon.brand.onDark.subtle     | `{color.text.brand.onDark.subtle}`     | `#a8a9e3` | `{color.text.brand.onDark.subtle}`     | `#32348c` |
| icon.brand.onDark.muted      | `{color.text.brand.onDark.muted}`      | `#7879cc` | `{color.text.brand.onDark.muted}`      | `#7879cc` |
| icon.brand.onLight.strong    | `{color.text.brand.onLight.strong}`    | `#181952` | `{color.text.brand.onLight.strong}`    | `#ffffff` |
| icon.brand.onLight.default   | `{color.text.brand.onLight.default}`   | `#292b79` | `{color.text.brand.onLight.default}`   | `#d6d7f5` |
| icon.brand.onLight.subtle    | `{color.text.brand.onLight.subtle}`    | `#32348c` | `{color.text.brand.onLight.subtle}`    | `#a8a9e3` |
| icon.brand.onLight.muted     | `{color.text.brand.onLight.muted}`     | `#7879cc` | `{color.text.brand.onLight.muted}`     | `#7879cc` |
| icon.utility.danger.strong   | `{color.global.red.800}`               | `#991b1b` | `{color.global.red.400}`               | `#f87171` |
| icon.utility.danger.default  | `{color.global.red.700}`               | `#b91c1c` | `{color.global.red.400}`               | `#f87171` |
| icon.utility.danger.subtle   | `{color.global.red.600}`               | `#dc2626` | `{color.global.red.500}`               | `#ef4444` |
| icon.utility.danger.muted    | `{color.global.red.400}`               | `#f87171` | `{color.global.red.700}`               | `#b91c1c` |
| icon.utility.warning.strong  | `{color.global.orange.800}`            | `#9a3412` | `{color.global.orange.400}`            | `#fb923c` |
| icon.utility.warning.default | `{color.global.orange.700}`            | `#c2410c` | `{color.global.orange.400}`            | `#fb923c` |
| icon.utility.warning.subtle  | `{color.global.orange.600}`            | `#ea580c` | `{color.global.orange.500}`            | `#f97316` |
| icon.utility.warning.muted   | `{color.global.orange.400}`            | `#fb923c` | `{color.global.orange.700}`            | `#c2410c` |
| icon.utility.success.strong  | `{color.global.green.800}`             | `#166534` | `{color.global.green.400}`             | `#4ade80` |
| icon.utility.success.default | `{color.global.green.700}`             | `#15803d` | `{color.global.green.400}`             | `#4ade80` |
| icon.utility.success.subtle  | `{color.global.green.600}`             | `#16a34a` | `{color.global.green.500}`             | `#22c55e` |
| icon.utility.success.muted   | `{color.global.green.400}`             | `#4ade80` | `{color.global.green.700}`             | `#15803d` |
| icon.utility.info.strong     | `{color.global.blue.800}`              | `#1e40af` | `{color.global.blue.400}`              | `#60a5fa` |
| icon.utility.info.default    | `{color.global.blue.700}`              | `#1d4ed8` | `{color.global.blue.400}`              | `#60a5fa` |
| icon.utility.info.subtle     | `{color.global.blue.600}`              | `#2563eb` | `{color.global.blue.500}`              | `#3b82f6` |
| icon.utility.info.muted      | `{color.global.blue.400}`              | `#60a5fa` | `{color.global.blue.700}`              | `#1d4ed8` |

## surface

Background and border colors for surfaces/containers by elevation.

| Token                             | Light alias                                     | Light     | Dark alias                                | Dark      |
| --------------------------------- | ----------------------------------------------- | --------- | ----------------------------------------- | --------- |
| surface.neutral.background.base   | `{color.global.gray.50}`                        | `#f9fafb` | `{color.global.gray.950}`                 | `#0e121b` |
| surface.neutral.background.level1 | `{color.global.neutral.white}`                  | `#ffffff` | `{color.global.gray.900}`                 | `#111827` |
| surface.neutral.background.level2 | `{color.global.neutral.white}`                  | `#ffffff` | `{color.global.gray.900}`                 | `#111827` |
| surface.neutral.border.base       | `{color.global.gray.200}`                       | `#dfe2e7` | `{color.global.gray.700}`                 | `#374151` |
| surface.neutral.border.level1     | `{color.action.neutral.default.border.default}` | `#dfe2e7` | `{color.surface.neutral.border.base}`     | `#374151` |
| surface.neutral.border.level2     | `{color.action.neutral.default.border.default}` | `#dfe2e7` | `{color.surface.neutral.border.base}`     | `#374151` |
| surface.brand.background.base     | `{color.brand.primary.50}`                      | `#fbfbfe` | `{color.brand.primary.900}`               | `#181952` |
| surface.brand.background.level1   | `{color.global.neutral.white}`                  | `#ffffff` | `{color.brand.primary.800}`               | `#202266` |
| surface.brand.background.level2   | `{color.surface.neutral.background.level1}`     | `#ffffff` | `{color.surface.brand.background.level1}` | `#202266` |
| surface.brand.border.base         | `{color.brand.primary.100}`                     | `#d6d7f5` | `{color.brand.primary.800}`               | `#202266` |
| surface.brand.border.level1       | `{color.brand.primary.100}`                     | `#d6d7f5` | `{color.brand.primary.100}`               | `#d6d7f5` |
| surface.brand.border.level2       | `{color.brand.primary.100}`                     | `#d6d7f5` | `{color.brand.primary.100}`               | `#d6d7f5` |

## utility

Status/feedback colors (danger, warning, info, success, focus).

| Token                      | Light alias                     | Light             | Dark alias                      | Dark              |
| -------------------------- | ------------------------------- | ----------------- | ------------------------------- | ----------------- |
| utility.danger.subtle      | `{color.global.red.100}`        | `#fee2e2`         | `{color.global.red.950}`        | `#450a0a`         |
| utility.danger.medium      | `{color.global.red.500}`        | `#ef4444`         | `{color.global.red.600}`        | `#dc2626`         |
| utility.danger.strong      | `{color.global.red.800}`        | `#991b1b`         | `{color.global.red.200}`        | `#fecaca`         |
| utility.warning.subtle     | `{color.global.orange.100}`     | `#ffedd5`         | `{color.global.orange.950}`     | `#431407`         |
| utility.warning.medium     | `{color.global.orange.500}`     | `#f97316`         | `{color.global.orange.600}`     | `#ea580c`         |
| utility.warning.strong     | `{color.global.orange.800}`     | `#9a3412`         | `{color.global.orange.200}`     | `#fed7aa`         |
| utility.info.subtle        | `{color.global.blue.100}`       | `#dbeafe`         | `{color.global.blue.950}`       | `#172554`         |
| utility.info.medium        | `{color.global.blue.500}`       | `#3b82f6`         | `{color.global.blue.600}`       | `#2563eb`         |
| utility.info.strong        | `{color.global.blue.800}`       | `#1e40af`         | `{color.global.blue.200}`       | `#bfdbfe`         |
| utility.success.subtle     | `{color.global.green.100}`      | `#dcfce7`         | `{color.global.green.950}`      | `#052e16`         |
| utility.success.medium     | `{color.global.green.500}`      | `#22c55e`         | `{color.global.green.600}`      | `#16a34a`         |
| utility.success.strong     | `{color.global.green.800}`      | `#166534`         | `{color.global.green.200}`      | `#bbf7d0`         |
| utility.focus.default      | `{color.global.blue.500}`       | `#3b82f6`         | `{color.global.blue.500}`       | `#3b82f6`         |
| utility.transparent.subtle | `{color.global.transparent.20}` | `rgba(0,0,0,0.2)` | `{color.global.transparent.20}` | `rgba(0,0,0,0.2)` |
| utility.transparent.medium | `{color.global.transparent.50}` | `rgba(0,0,0,0.5)` | `{color.global.transparent.50}` | `rgba(0,0,0,0.5)` |
| utility.transparent.strong | `{color.global.transparent.70}` | `rgba(0,0,0,0.7)` | `{color.global.transparent.70}` | `rgba(0,0,0,0.7)` |

## dataviz

Data-visualization palette.

| Token                          | Light alias                   | Light     | Dark alias                    | Dark      |
| ------------------------------ | ----------------------------- | --------- | ----------------------------- | --------- |
| dataviz.brand.primary.muted    | `{color.brand.primary.100}`   | `#d6d7f5` | `{color.brand.primary.500}`   | `#3d3e9f` |
| dataviz.brand.primary.subtle   | `{color.brand.primary.200}`   | `#a8a9e3` | `{color.brand.primary.400}`   | `#4647b1` |
| dataviz.brand.primary.medium   | `{color.brand.primary.300}`   | `#7879cc` | `{color.brand.primary.300}`   | `#7879cc` |
| dataviz.brand.primary.strong   | `{color.brand.primary.400}`   | `#4647b1` | `{color.brand.primary.200}`   | `#a8a9e3` |
| dataviz.brand.primary.heavy    | `{color.brand.primary.500}`   | `#3d3e9f` | `{color.brand.primary.100}`   | `#d6d7f5` |
| dataviz.brand.secondary.muted  | `{color.brand.secondary.100}` | `#fdf4cc` | `{color.brand.secondary.500}` | `#d7ac03` |
| dataviz.brand.secondary.subtle | `{color.brand.secondary.200}` | `#fbe899` | `{color.brand.secondary.400}` | `#efc103` |
| dataviz.brand.secondary.medium | `{color.brand.secondary.300}` | `#f9dc66` | `{color.brand.secondary.300}` | `#f9dc66` |
| dataviz.brand.secondary.strong | `{color.brand.secondary.400}` | `#efc103` | `{color.brand.secondary.200}` | `#fbe899` |
| dataviz.brand.secondary.heavy  | `{color.brand.secondary.500}` | `#d7ac03` | `{color.brand.secondary.100}` | `#fdf4cc` |
| dataviz.brand.tertiary.muted   | `{color.brand.tertiary.100}`  | `#dbeade` | `{color.brand.tertiary.500}`  | `#77a284` |
| dataviz.brand.tertiary.subtle  | `{color.brand.tertiary.200}`  | `#b7d5be` | `{color.brand.tertiary.400}`  | `#86b593` |
| dataviz.brand.tertiary.medium  | `{color.brand.tertiary.300}`  | `#92c19e` | `{color.brand.tertiary.300}`  | `#92c19e` |
| dataviz.brand.tertiary.strong  | `{color.brand.tertiary.400}`  | `#86b593` | `{color.brand.tertiary.200}`  | `#b7d5be` |
| dataviz.brand.tertiary.heavy   | `{color.brand.tertiary.500}`  | `#77a284` | `{color.brand.tertiary.100}`  | `#dbeade` |
| dataviz.blue.muted             | `{color.global.blue.200}`     | `#bfdbfe` | `{color.global.blue.600}`     | `#2563eb` |
| dataviz.blue.subtle            | `{color.global.blue.300}`     | `#93c5fd` | `{color.global.blue.500}`     | `#3b82f6` |
| dataviz.blue.medium            | `{color.global.blue.400}`     | `#60a5fa` | `{color.global.blue.400}`     | `#60a5fa` |
| dataviz.blue.strong            | `{color.global.blue.500}`     | `#3b82f6` | `{color.global.blue.300}`     | `#93c5fd` |
| dataviz.blue.heavy             | `{color.global.blue.600}`     | `#2563eb` | `{color.global.blue.200}`     | `#bfdbfe` |
| dataviz.green.muted            | `{color.global.green.200}`    | `#bbf7d0` | `{color.global.green.600}`    | `#16a34a` |
| dataviz.green.subtle           | `{color.global.green.300}`    | `#86efac` | `{color.global.green.500}`    | `#22c55e` |
| dataviz.green.medium           | `{color.global.green.400}`    | `#4ade80` | `{color.global.green.400}`    | `#4ade80` |
| dataviz.green.strong           | `{color.global.green.500}`    | `#22c55e` | `{color.global.green.300}`    | `#86efac` |
| dataviz.green.heavy            | `{color.global.green.600}`    | `#16a34a` | `{color.global.green.200}`    | `#bbf7d0` |
| dataviz.orange.muted           | `{color.global.orange.200}`   | `#fed7aa` | `{color.global.orange.600}`   | `#ea580c` |
| dataviz.orange.subtle          | `{color.global.orange.300}`   | `#fdba74` | `{color.global.orange.500}`   | `#f97316` |
| dataviz.orange.medium          | `{color.global.orange.400}`   | `#fb923c` | `{color.global.orange.400}`   | `#fb923c` |
| dataviz.orange.strong          | `{color.global.orange.500}`   | `#f97316` | `{color.global.orange.300}`   | `#fdba74` |
| dataviz.orange.heavy           | `{color.global.orange.600}`   | `#ea580c` | `{color.global.orange.200}`   | `#fed7aa` |
| dataviz.pink.muted             | `{color.global.pink.200}`     | `#fbcfe8` | `{color.global.pink.600}`     | `#db2777` |
| dataviz.pink.subtle            | `{color.global.pink.300}`     | `#f9a8d4` | `{color.global.pink.500}`     | `#ec4899` |
| dataviz.pink.medium            | `{color.global.pink.400}`     | `#f472b6` | `{color.global.pink.400}`     | `#f472b6` |
| dataviz.pink.strong            | `{color.global.pink.500}`     | `#ec4899` | `{color.global.pink.300}`     | `#f9a8d4` |
| dataviz.pink.heavy             | `{color.global.pink.600}`     | `#db2777` | `{color.global.pink.200}`     | `#fbcfe8` |
| dataviz.red.muted              | `{color.global.red.200}`      | `#fecaca` | `{color.global.red.600}`      | `#dc2626` |
| dataviz.red.subtle             | `{color.global.red.300}`      | `#fca5a5` | `{color.global.red.500}`      | `#ef4444` |
| dataviz.red.medium             | `{color.global.red.400}`      | `#f87171` | `{color.global.red.400}`      | `#f87171` |
| dataviz.red.strong             | `{color.global.red.500}`      | `#ef4444` | `{color.global.red.300}`      | `#fca5a5` |
| dataviz.red.heavy              | `{color.global.red.600}`      | `#dc2626` | `{color.global.red.200}`      | `#fecaca` |
| dataviz.yellow.muted           | `{color.global.yellow.200}`   | `#fef08a` | `{color.global.yellow.600}`   | `#ca8a04` |
| dataviz.yellow.subtle          | `{color.global.yellow.300}`   | `#fde047` | `{color.global.yellow.500}`   | `#eab308` |
| dataviz.yellow.medium          | `{color.global.yellow.400}`   | `#facc15` | `{color.global.yellow.400}`   | `#facc15` |
| dataviz.yellow.strong          | `{color.global.yellow.500}`   | `#eab308` | `{color.global.yellow.300}`   | `#fde047` |
| dataviz.yellow.heavy           | `{color.global.yellow.600}`   | `#ca8a04` | `{color.global.yellow.200}`   | `#fef08a` |

## neutralPalette

Neutral scale from pure (white) to solid (black).

| Token                 | Light alias                    | Light     | Dark alias                     | Dark      |
| --------------------- | ------------------------------ | --------- | ------------------------------ | --------- |
| neutralPalette.pure   | `{color.global.neutral.white}` | `#ffffff` | `{color.global.neutral.black}` | `#000000` |
| neutralPalette.muted  | `{color.global.gray.100}`      | `#f3f4f6` | `{color.global.gray.800}`      | `#1f2937` |
| neutralPalette.subtle | `{color.global.gray.300}`      | `#d1d5db` | `{color.global.gray.700}`      | `#374151` |
| neutralPalette.medium | `{color.global.gray.400}`      | `#9ca3af` | `{color.global.gray.500}`      | `#6b7280` |
| neutralPalette.strong | `{color.global.gray.600}`      | `#4b5563` | `{color.global.gray.300}`      | `#d1d5db` |
| neutralPalette.heavy  | `{color.global.gray.800}`      | `#1f2937` | `{color.global.gray.100}`      | `#f3f4f6` |
| neutralPalette.solid  | `{color.global.neutral.black}` | `#000000` | `{color.global.neutral.white}` | `#ffffff` |

## neutralAbsolute

Absolute white/black, mode-independent.

| Token                 | Light alias                    | Light     | Dark alias                     | Dark      |
| --------------------- | ------------------------------ | --------- | ------------------------------ | --------- |
| neutralAbsolute.white | `{color.global.neutral.white}` | `#ffffff` | `{color.global.neutral.white}` | `#ffffff` |
| neutralAbsolute.black | `{color.global.neutral.black}` | `#000000` | `{color.global.neutral.black}` | `#000000` |
