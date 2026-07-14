---
title: Colors
nav_order: 1
description: The color tokens that everything is built on.
---

Colors are exposed as tokens. Always reference the token, never a raw hex value.

## Core palette

| Token | Value | Usage |
| --- | --- | --- |
| `color.accent` | `#0969da` | Primary actions, links |
| `color.fg` | `#1b1f24` | Body text |
| `color.muted` | `#656d76` | Secondary text |
| `color.border` | `#d8dee4` | Dividers, outlines |
| `color.bg` | `#ffffff` | Surfaces |

## Usage

```css
.button-primary {
  background: var(--color-accent);
  color: #fff;
}
```
