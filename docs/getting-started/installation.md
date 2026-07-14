---
title: Installation
nav_order: 2
description: Add the design system to your project.
---

Install the package from your registry:

```bash
npm install @your-org/design-system
```

Import the base styles once at the root of your app:

```js
import "@your-org/design-system/styles.css";
```

Then use components:

```jsx
import { Button } from "@your-org/design-system";

export default function Example() {
  return <Button variant="primary">Save</Button>;
}
```
