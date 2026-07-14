---
title: Forking dawn-design
description: How to fork dawn-design for your project, and what counts as a deviation from DS3.
status: draft
group: GitHub
nav_order: 3
---

Every client project starts from a fork of `dawn-design`. The fork keeps DS3's structure and architecture intact while letting you set your own token values. This page covers how forking works and how to tell the difference between an intended customization and an actual deviation from DS3.

## Why forking works this way

DS3 uses a 3-tier token architecture: core, semantic, and component. The names of the tokens are what's mapped in code, not the values. Because of that, you can change a value freely without touching a single line of dev code, as long as the token name and its place in the architecture stay the same.

This is also why forking is safe by design. Your fork can look completely different from another project's fork while both stay fully compatible with the Template App.

> **💡 The rule in one sentence**
>
> Change values freely. Never change names or structure.

## Forking your project repo

#### Fork dawn-design

Fork `DawnHealthGit/dawn-design` into your own repo, named `[project]-design`. This becomes your project's source of truth for token values.

#### Update token values

Open the token files and update the values to match your project's visual direction. Token names, file structure, and the alias chains between tiers stay exactly as they are in `dawn-design`.

#### Keep your fork in sync

`dawn-design` keeps evolving. Pull in updates from the canonical repo regularly so your fork doesn't fall behind on structural changes, new tokens, or fixes.

### What counts as a deviation

Not every difference between your fork and `dawn-design` is a problem. The distinction comes down to what changed.

> **✅ Value changes are not a deviation**
>
> A token keeping its name and position in the architecture, with a different value, is exactly what forking is for. This is expected and never flagged.

> **🚫 Name and structure changes are deviations**
>
> These break the contract between design and code, and are always flagged.

### Name deviations

A token name in your fork doesn't exist in canonical `dawn-design`, or a canonical token name has been renamed in your fork. Since dev code maps to token names, a name change means the Template App can no longer resolve that token correctly without extra dev work.

### Structural deviations

The alias chain between tiers has been broken. Common examples:

- A core token aliases another token, instead of containing a resolved value
- A component token aliases a core token directly, skipping the semantic tier, outside of the rare documented exceptions
- A semantic token aliases a component token
- A color token has been added to `semantic.json` instead of `light.json` or `dark.json`

Any of these break the 3-tier architecture and should be corrected before merging.

## Comparing your fork against the latest DS3

When checking your fork against `dawn-design`, always compare against the latest release on the default branch, not a specific older version you may have started from.

<details markdown="1">
<summary>What if I intentionally renamed a token for my project?</summary>

Don't. Token names are the contract between design and dev. If a name genuinely needs to change across the whole system, that's a DS3-level proposal, not a per-project fork decision.
</details>

<details markdown="1">
<summary>What if my fork is missing a token that exists in canonical?</summary>

That's a name deviation. It usually means your fork hasn't been synced with a recent `dawn-design` update. Pull the latest changes and add the missing token.
</details>

<details markdown="1">
<summary>Can component tokens ever alias core tokens directly?</summary>

On rare, documented occasions, yes. If your fork does this without it being one of those documented exceptions, it's a structural deviation.
</details>
