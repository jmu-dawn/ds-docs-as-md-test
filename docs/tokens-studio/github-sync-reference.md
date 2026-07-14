---
title: GitHub sync reference
description: How GitHub sync works in Tokens Studio, with a field-by-field reference for the credentials form.
status: stable
group: Tokens Studio
nav_order: 2
---

This page explains how GitHub sync works and documents every field in the Tokens Studio credentials form. If you just want to get connected, follow the [setup guide]({{ '/docs/tokens-studio/set-up-github-sync/' | relative_url }}).

## How GitHub sync works

[GitHub](https://github.com/) is a Git-based repository hosting service and the source of truth for DS3 design tokens as well as the project's design tokens. The Tokens Studio plugin connects to the repos through a native two-way sync, so the same token files power both design and development.

Once connected you can:

- **Push** token JSON files from Figma to GitHub
- **Pull** tokens stored in GitHub into any Figma file

Because the tokens live in GitHub, the repository (not any individual Figma file) holds the source of truth for design decisions. Everyone pulls from the same place, and changes flow back through the same place.

<div class="card-grid">
  <a class="card" href="{{ '/docs/tokens-studio/set-up-github-sync/' | relative_url }}">
    <h3>🚀 Set up GitHub sync</h3>
    <p>The step-by-step guide to connecting Tokens Studio to GitHub.</p>
  </a>
</div>

## Credentials reference

These are the fields in the **Add new sync provider** form when you choose GitHub. You fill them in once per Figma file.

### Name

A nickname for this sync configuration, shown in the plugin settings so you can identify it later. Use the same name as the repository. For example `dawn-design` for the DS3 design repo, or `[product]-design` for a product design repo.

### Personal Access Token

The PAT generated for your personal Dawn GitHub account. It lets the plugin authenticate on your behalf, so treat it like a password: do not share it!

> **💡 Generating a PAT**
>
> See [Generate a Personal Access Token]({{ '/docs/github/personal-access-token/' | relative_url }}) for how to create one with the right scope.

### Repository

The `owner/repo` portion of the repository URL, taken from everything after `github.com/`. For the URL `https://github.com/DawnHealthGit/dawn-design`, you would enter:

```
DawnHealthGit/dawn-design
```

### Branch

The branch that tokens are pushed to and pulled from. At Dawn this is usually:

```
master
```

If you are unsure which branch to target, ask your Design System Designer or the engineers who consume the tokens.

### Token storage location

Tokens Studio can store token JSON two ways: as a single combined file, or as a folder of multiple files. At Dawn we use **folder storage** so that engineers can consume tokens directly from GitHub and so the Themes feature works. Enter the folder name:

```
tokens
```

> **⚠️ Pro licence required**
>
> Multi-file sync to remote storage needs a Tokens Studio Pro licence. Without one, you have read-only access to the tokens. Request a licence through ServiceDesk or your manager if you need to push changes.

### Base URL

Not used at Dawn. Leave this field empty.

## Common questions

<details markdown="1">
<summary>Why folder storage instead of a single file?</summary>

Folder storage writes one JSON file per token set, which is what lets engineers pull tokens straight from the repo and keeps the Themes feature working. A single combined file would break both of those.
</details>

<details markdown="1">
<summary>Why is Push to GitHub disabled right after I connect?</summary>

A disabled Push button means your local tokens match the remote, so there is nothing to send. You stay in this read-only state until you intentionally make a change. Note that pushing also requires a Pro licence.
</details>

<details markdown="1">
<summary>Which branch should I target?</summary>

At Dawn the token branch is usually `master`. If you are working against a product design repo or are unsure, confirm the branch with your Design System Designer before syncing so you do not push to the wrong place.
</details>
