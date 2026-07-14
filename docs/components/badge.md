---
title: Badge
nav_order: 3
---

Extracted via Token Extractor plugin in Figma and based on node mappings from Tokens Studio on `sharedPluginData`.

## Shared tokens (all variants)

| Property       | Token                        |
| -------------- | ---------------------------- |
| `borderRadius` | `badge.borderRadius.default` |
| `itemSpacing`  | `gap.xs`                     |

## Tokens by Color

| Color    | `fill (background)`                          |
| -------- | -------------------------------------------- |
| Danger   | `badge.color.negative.background.default`    |
| Ghost    | `badge.color.ghost.background.default`       |
| Info     | `badge.color.informative.background.default` |
| Neutral  | `badge.color.neutral.background.default`     |
| Positive | `badge.color.positive.background.default`    |
| Warning  | `badge.color.warning.background.default`     |

## Tokens by Type × Color

| Type   | Color    | `fill (foreground)`                          |
| ------ | -------- | -------------------------------------------- |
| Dot    | Danger   | —                                            |
| Dot    | Info     | —                                            |
| Dot    | Positive | —                                            |
| Dot    | Warning  | —                                            |
| Number | Danger   | `badge.color.negative.foreground.default`    |
| Number | Info     | `badge.color.informative.foreground.default` |
| Number | Positive | `badge.color.positive.foreground.default`    |
| Number | Warning  | `badge.color.warning.foreground.default`     |
| Pill   | Danger   | `badge.color.negative.foreground.default`    |
| Pill   | Ghost    | `badge.color.ghost.foreground.default`       |
| Pill   | Info     | `badge.color.informative.foreground.default` |
| Pill   | Neutral  | `badge.color.neutral.foreground.default`     |
| Pill   | Positive | `badge.color.positive.foreground.default`    |
| Pill   | Warning  | `badge.color.warning.foreground.default`     |

## Tokens by Type × Icon

| Type   | Icon     | `horizontalPadding` | `verticalPadding` | `typography`                       |
| ------ | -------- | ------------------- | ----------------- | ---------------------------------- |
| Dot    | None     | —                   | —                 | —                                  |
| Number | None     | `padding.sm`        | `padding.xs`      | `typography.labelSmall.emphasized` |
| Number | Only     | —                   | —                 | —                                  |
| Pill   | Leading  | `padding.sm`        | `padding.xs`      | `typography.labelSmall.emphasized` |
| Pill   | None     | `padding.sm`        | `padding.xs`      | `typography.labelSmall.emphasized` |
| Pill   | Trailing | `padding.sm`        | `padding.xs`      | `typography.labelSmall.emphasized` |

## All 30 instances

| Node   | Type   | Color    | Icon     | Background token                             | Foreground token                             |
| ------ | ------ | -------- | -------- | -------------------------------------------- | -------------------------------------------- |
| `1:11` | Pill   | Info     | Leading  | `badge.color.informative.background.default` | `badge.color.informative.foreground.default` |
| `1:14` | Pill   | Positive | Leading  | `badge.color.positive.background.default`    | `badge.color.positive.foreground.default`    |
| `1:17` | Pill   | Warning  | Leading  | `badge.color.warning.background.default`     | `badge.color.warning.foreground.default`     |
| `1:20` | Pill   | Danger   | Leading  | `badge.color.negative.background.default`    | `badge.color.negative.foreground.default`    |
| `1:23` | Pill   | Neutral  | Leading  | `badge.color.neutral.background.default`     | `badge.color.neutral.foreground.default`     |
| `1:26` | Pill   | Ghost    | Leading  | `badge.color.ghost.background.default`       | `badge.color.ghost.foreground.default`       |
| `1:29` | Pill   | Info     | Trailing | `badge.color.informative.background.default` | `badge.color.informative.foreground.default` |
| `1:32` | Pill   | Positive | Trailing | `badge.color.positive.background.default`    | `badge.color.positive.foreground.default`    |
| `1:35` | Pill   | Warning  | Trailing | `badge.color.warning.background.default`     | `badge.color.warning.foreground.default`     |
| `1:38` | Pill   | Danger   | Trailing | `badge.color.negative.background.default`    | `badge.color.negative.foreground.default`    |
| `1:41` | Pill   | Neutral  | Trailing | `badge.color.neutral.background.default`     | `badge.color.neutral.foreground.default`     |
| `1:44` | Pill   | Ghost    | Trailing | `badge.color.ghost.background.default`       | `badge.color.ghost.foreground.default`       |
| `1:47` | Pill   | Info     | None     | `badge.color.informative.background.default` | `badge.color.informative.foreground.default` |
| `1:49` | Pill   | Positive | None     | `badge.color.positive.background.default`    | `badge.color.positive.foreground.default`    |
| `1:51` | Pill   | Warning  | None     | `badge.color.warning.background.default`     | `badge.color.warning.foreground.default`     |
| `1:53` | Pill   | Danger   | None     | `badge.color.negative.background.default`    | `badge.color.negative.foreground.default`    |
| `1:55` | Pill   | Neutral  | None     | `badge.color.neutral.background.default`     | `badge.color.neutral.foreground.default`     |
| `1:57` | Pill   | Ghost    | None     | `badge.color.ghost.background.default`       | `badge.color.ghost.foreground.default`       |
| `1:59` | Dot    | Danger   | None     | `badge.color.negative.background.default`    | —                                            |
| `1:60` | Dot    | Positive | None     | `badge.color.positive.background.default`    | —                                            |
| `1:61` | Dot    | Warning  | None     | `badge.color.warning.background.default`     | —                                            |
| `1:62` | Dot    | Info     | None     | `badge.color.informative.background.default` | —                                            |
| `1:63` | Number | Info     | None     | `badge.color.informative.background.default` | `badge.color.informative.foreground.default` |
| `1:65` | Number | Info     | Only     | `badge.color.informative.background.default` | `badge.color.informative.foreground.default` |
| `1:67` | Number | Positive | None     | `badge.color.positive.background.default`    | `badge.color.positive.foreground.default`    |
| `1:69` | Number | Positive | Only     | `badge.color.positive.background.default`    | `badge.color.positive.foreground.default`    |
| `1:71` | Number | Warning  | None     | `badge.color.warning.background.default`     | `badge.color.warning.foreground.default`     |
| `1:73` | Number | Warning  | Only     | `badge.color.warning.background.default`     | `badge.color.warning.foreground.default`     |
| `1:75` | Number | Danger   | None     | `badge.color.negative.background.default`    | `badge.color.negative.foreground.default`    |
| `1:77` | Number | Danger   | Only     | `badge.color.negative.background.default`    | `badge.color.negative.foreground.default`    |
