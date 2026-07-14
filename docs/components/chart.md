---
title: Chart
nav_order: 6
---

Source: Figma file "DS3 - Mobile" (`—`). Extracted via the Token Extractor plugin (Tokens Studio `sharedPluginData`).

> **Note:** This export captured the interior of a **single chart variant** (`Chart type=lineChart, Size=Default`) — only leaf nodes (ellipses, vectors, text, lines), no `COMPONENT`/`INSTANCE` variant nodes. So this is a flat layer→token reference for one line-chart instance, not a per-variant table. Re-run the extractor on the Chart **component set** for variant coverage.

## Grid & axes

| Layer             | Property      | Token                                    |
| ----------------- | ------------- | ---------------------------------------- |
| `yAxisGridLine`   | `borderColor` | `chart.color.grid.line.horizontal`       |
| `yAxisGridLine`   | `borderWidth` | `chart.borderWidth.grid.line.horizontal` |
| `xAxisGridLine`   | `borderColor` | `chart.color.grid.line.vertical`         |
| `xAxisGridLine`   | `borderWidth` | `chart.borderWidth.grid.line.vertical`   |
| `xAxisTick`       | `borderColor` | `chart.color.grid.line.vertical`         |
| `xAxisTick`       | `borderWidth` | `chart.borderWidth.grid.line.vertical`   |
| `yAxisValueLabel` | `fill`        | `chart.color.axis.label.default`         |
| `yAxisValueLabel` | `typography`  | `chart.typography.axis.label.default`    |
| `xAxisValueLabel` | `fill`        | `chart.color.axis.label.default`         |
| `xAxisValueLabel` | `typography`  | `chart.typography.axis.label.default`    |

## Line series

| Property      | Token                                      |
| ------------- | ------------------------------------------ |
| `borderWidth` | `chart.borderWidth.lineChart.line.default` |

`borderColor` cycles through the full series palette (one line per series):

| Series   | Token                                 |
| -------- | ------------------------------------- |
| 1        | `chart.color.series.1.default`        |
| 2        | `chart.color.series.2.default`        |
| 3        | `chart.color.series.3.default`        |
| 4        | `chart.color.series.4.default`        |
| 5        | `chart.color.series.5.default`        |
| neutral  | `chart.color.series.neutral.default`  |
| positive | `chart.color.series.positive.default` |
| negative | `chart.color.series.negative.default` |
| warning  | `chart.color.series.warning.default`  |

## Point markers

| Property      | Token                                             |
| ------------- | ------------------------------------------------- |
| `fill`        | `chart.color.lineChart.marker.fill.default`       |
| `borderWidth` | `chart.borderWidth.lineChart.pointMarker.default` |
| `width`       | `chart.size.lineChart.pointMarker.default`        |
| `height`      | `chart.size.lineChart.pointMarker.default`        |

`borderColor` matches the series palette above (same 9 series tokens), so each marker inherits its line's color.
