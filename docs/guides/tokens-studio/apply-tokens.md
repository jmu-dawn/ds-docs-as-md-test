---
title: Applying tokens in Figma
description: How to apply design tokens to elements in Figma using the Tokens Studio plugin.
status: stable
group: Tokens Studio
nav_order: 3
---

## Prerequisites

Before applying any tokens, make sure the Tokens Studio plugin is open and connected to the right GitHub repository.

> ℹ️ Working on DS3 components or PACE layouts? -> Connect to the dawn-design repo.  
> Working on a client product? -> Connect to the product-specific repo.

## Token types overview

The token type defines which design property it belongs to and where it can be applied. Most types map directly to a Figma property. For example, a `borderRadius` token can only be applied to corner radius, and a `borderWidth` token can only be applied to stroke weight.

The `dimension` type is more flexible. It covers any property that takes a distance value, including gap, padding, border width, border radius, width, height, and more. In DS3, dimension tokens are used exclusively for gap and padding.

**How to apply tokens in Tokens Studio:**

- Clicking a token applies it to its default property.
- Right-clicking opens a menu with additional application options.

## Color tokens

#### Select an element in Figma

#### Open the Color section in Tokens Studio

#### Right-click a color token and choose Fill or Border

Color tokens apply to Fill by default.

## Border Radius tokens

#### Select an element in Figma

#### Open the Border Radius section in Tokens Studio

#### Right-click a borderRadius token

Choose from: All, Top Right, Top Left, Bottom Right, or Bottom Left.

Border Radius tokens apply to All by default.

## Border Width tokens

#### Select an element in Figma

#### Open the Border Width section in Tokens Studio

#### Right-click a borderWidth token

Choose from: All, Top, Right, Bottom, or Left.

Border Width tokens apply to All by default.

## Typography tokens

Typography tokens are composite tokens. They bundle font family, weight, size, line height, and letter spacing into a single token. Applying one sets all text properties at once.

#### Select a text element in Figma

#### Open the Typography section in Tokens Studio

#### Click a typography token to apply it

> **⚠️ Font Weight tokens are for internal use only**
>
> Font Weight tokens are meant to be used inside Typography tokens, not applied directly to text. If you apply a font weight token to text that already has a Typography token applied, Figma will override the weight visually while Tokens Studio keeps both tokens mapped. This creates a mismatch that can confuse developers.
>
> Rule: only apply Font Weight tokens as part of a Typography token. Never apply them directly to text.

## Gap tokens

#### Select a frame with Auto Layout

#### Open the Dimension section in Tokens Studio

#### Right-click a gap token

Choose **Spacing → Gap** or **Spacing → Row gap**.

Gap tokens apply to the default gap based on Auto Layout direction:

- Vertical layout → vertical gap
- Horizontal layout → horizontal gap
- Horizontal + Wrap → horizontal gap (use Row gap for the gap between rows)

> **🚫 Never use Spacing → All for gap**
>
> Using **Spacing → All** removes the visible gap in Figma while keeping the gap token mapped in Tokens Studio. Developers will export a gap value that does not match what is shown in the design.
>
> Always use **Spacing → Gap** or **Spacing → Row gap** instead.

> ⚠️ If you apply a gap token to a frame before Auto Layout is enabled, you may need to remove and re-apply the token after enabling Auto Layout for the value to apply correctly.

## Padding tokens

#### Select an element in Figma

#### Open the Dimension section in Tokens Studio

#### Right-click a padding token

Choose from: **Spacing → Horizontal**, **Vertical**, **Top**, **Right**, **Bottom**, or **Left**.

> **🚫 Never use Spacing → All for padding**
>
> Using **Spacing → All** removes the visible gap in Figma while keeping the gap token mapped in Tokens Studio. This causes a mismatch between what is shown in the design and what developers export.
>
> Always use directional spacing options instead of Spacing → All.
