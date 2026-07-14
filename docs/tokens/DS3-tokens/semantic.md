---
title: Semantic tokens
group: DS3 Tokens
nav_order: 3
---

Purpose-based tokens that alias core primitives. Source: `tokens/base/semantic.json`. The `Alias` column is the reference; `Value` is the resolved primitive.

## Border radius

| Token | Alias               | Value   |
| ----- | ------------------- | ------- |
| none  | `{dimension.0px}`   | `0px`   |
| xxs   | `{dimension.2px}`   | `2px`   |
| xs    | `{dimension.4px}`   | `4px`   |
| sm    | `{dimension.8px}`   | `8px`   |
| md    | `{dimension.12px}`  | `12px`  |
| lg    | `{dimension.16px}`  | `16px`  |
| xl    | `{dimension.20px}`  | `20px`  |
| xxl   | `{dimension.24px}`  | `24px`  |
| xxxl  | `{dimension.32px}`  | `32px`  |
| round | `{dimension.999px}` | `999px` |

## Border width

| Token | Alias             | Value |
| ----- | ----------------- | ----- |
| sm    | `{dimension.1px}` | `1px` |
| md    | `{dimension.2px}` | `2px` |
| lg    | `{dimension.4px}` | `4px` |

## Gap

| Token  | Alias              | Value  |
| ------ | ------------------ | ------ |
| none   | `{dimension.0px}`  | `0px`  |
| xxs    | `{dimension.2px}`  | `2px`  |
| xs     | `{dimension.4px}`  | `4px`  |
| sm     | `{dimension.8px}`  | `8px`  |
| md     | `{dimension.12px}` | `12px` |
| lg     | `{dimension.16px}` | `16px` |
| lgPlus | `{dimension.20px}` | `20px` |
| xl     | `{dimension.24px}` | `24px` |
| xxl    | `{dimension.32px}` | `32px` |
| xxxl   | `{dimension.40px}` | `40px` |

## Padding

| Token  | Alias              | Value  |
| ------ | ------------------ | ------ |
| none   | `{dimension.0px}`  | `0px`  |
| xxs    | `{dimension.2px}`  | `2px`  |
| xs     | `{dimension.4px}`  | `4px`  |
| sm     | `{dimension.8px}`  | `8px`  |
| md     | `{dimension.12px}` | `12px` |
| lg     | `{dimension.16px}` | `16px` |
| lgPlus | `{dimension.20px}` | `20px` |
| xl     | `{dimension.24px}` | `24px` |
| xxl    | `{dimension.32px}` | `32px` |
| xxxl   | `{dimension.40px}` | `40px` |

## Typography

Composite text styles. Values resolved to primitives (font size is unitless px).

| Style                   | Family      | Weight | Size | Line height |
| ----------------------- | ----------- | ------ | ---- | ----------- |
| title.regular           | Inter       | 500    | 34   | 44px        |
| title.emphasized        | Inter       | 600    | 34   | 44px        |
| heading1.regular        | Inter       | 400    | 24   | 32px        |
| heading1.emphasized     | Inter       | 600    | 24   | 32px        |
| heading2.regular        | Inter       | 400    | 20   | 26px        |
| heading2.emphasized     | Inter       | 600    | 20   | 26px        |
| heading3.regular        | Inter       | 400    | 16   | 20px        |
| heading3.emphasized     | Inter       | 600    | 16   | 20px        |
| body.regular            | Inter       | 400    | 16   | 24px        |
| body.emphasized         | Inter       | 600    | 16   | 24px        |
| labelLarge.regular      | Inter       | 400    | 16   | 20px        |
| labelLarge.emphasized   | Inter       | 500    | 16   | 20px        |
| labelLarge.monoRegular  | Roboto Mono | 400    | 16   | 20px        |
| labelMedium.regular     | Inter       | 400    | 14   | 18px        |
| labelMedium.emphasized  | Inter       | 500    | 14   | 18px        |
| labelMedium.monoRegular | Roboto Mono | 400    | 14   | 18px        |
| labelSmall.regular      | Inter       | 400    | 12   | 16px        |
| labelSmall.emphasized   | Inter       | 500    | 12   | 16px        |
| labelSmall.monoRegular  | Roboto Mono | 400    | 12   | 16px        |
| labelMini.regular       | Inter       | 400    | 10   | 14px        |
| labelMini.emphasized    | Inter       | 500    | 10   | 14px        |
| labelMini.monoRegular   | Roboto Mono | 400    | 10   | 14px        |

## Font weight aliases

| Token              | Alias                    | Value |
| ------------------ | ------------------------ | ----- |
| heading.emphasized | `{fontWeights.semiBold}` | `600` |
| body.emphasized    | `{fontWeights.semiBold}` | `600` |
| label.emphasized   | `{fontWeights.medium}`   | `500` |
