---
title: Button
nav_order: 1
description: Triggers an action or event.
---

Buttons let users take actions with a single tap or click.

## Variants

| Variant | When to use |
| --- | --- |
| `primary` | The main action on a screen |
| `secondary` | Alternative, lower-emphasis actions |
| `danger` | Destructive actions |

## Example

```jsx
<Button variant="primary">Save changes</Button>
<Button variant="secondary">Cancel</Button>
<Button variant="danger">Delete</Button>
```

## Guidelines

- Use one primary button per view.
- Keep labels short and action-oriented ("Save", not "Click here to save").
- Don't use a button when a link is more appropriate.
