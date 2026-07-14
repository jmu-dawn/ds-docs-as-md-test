---
title: Create a release in GitHub
description: A step-by-step guide to publishing a new DS3 release on GitHub, written for designers who are new to GitHub.
status: stable
group: GitHub
nav_order: 4
---

Releases are how DS3 changes get formally published. Each release has a version number, a changelog, and a snapshot of the token files at that point in time. Downstream teams use releases to know when to pull updates into their own repos.

This guide walks through creating a release using the GitHub web UI, no terminal required.

> **⚠️ Committing changes is not enough**
>
> Pushing or committing changes to the `master` branch **does not** make them available to developers on its own. Devs pull design token updates from a release, not from the branch directly. So even if your changes are already on `master`, you still need to create a new release and send the developers the release name or link. Without that, they have no way to pull the latest tokens.

> **ℹ️ Do you need new a release?**
>
> When you commit design token changes from Tokens Studio to GitHub, they're available in Figma immediately. A new release on the design repo is only needed when developers want to pull the latest token changes into code.

## What you'll need

- Access to the `-design` repo you're working on.
- The version number for this release (follow semantic versioning, see below)
- A written changelog summarizing what changed

## Versioning

### Core DS3 versioning

DS3 uses `MAJOR.MINOR.PATCH` version numbers, for example `v3.2.1`.

| Change type                                     | Version bump | Example             |
| ----------------------------------------------- | ------------ | ------------------- |
| New system architecture or structure. Breaking. | `MAJOR`      | `v3.0.0` → `v4.0.0` |
| Large updates. Could be breaking.               | `MINOR`      | `v3.2.0` → `v3.3.0` |
| Fixes additions. Not breaking.                  | `PATCH`      | `v3.2.0` → `v3.2.1` |

When in doubt, ask a developer before bumping the version. A `MAJOR` bump signals breaking changes to dev teams.

### Project design repo versioning

Project design repos use a combined version name:  
The DS3 base version they last synced from, followed by the project's own version. The two parts are joined with a hyphen.

```
[DS3 base version]-[project version]
```

For example, say a project last synced with DS3 at `v3.3.5`. The project then makes local changes to its forked design repo, bumping its own version to `v1.0.3`. The resulting project design repo version would be:

```
Example:
v3.3.5-1.0.3
```

This makes it clear at a glance which version of DS3 the project is built on, and how far it has diverged with local changes since.

> **💡 Why two version numbers**
>
> The DS3 base version tells you which upstream version the project forked from, so you can tell whether it's behind on DS3 updates. The project version tracks the local changes made on top of that base.

### Syncing a new DS3 version into a project repo

When a new version of DS3 ships, for example a bump from `v3.3.5` to `v3.3.6`, project repos can pull it in by clicking the **Sync** button on their repo in GitHub.

After syncing, create a new release with the updated DS3 base version. If the sync is the only change, you don't bump the project version, just the base version.

So a project sitting at `v3.3.5-1.0.3` that syncs to DS3 `v3.3.6` (and makes no other changes) would become:

```
v3.3.6-1.0.3
```

The project version only moves when the project itself makes local changes. A pure DS3 sync moves the base version only.

## Creating the release

#### Open the Releases page

Go to the `*-design` repo on GitHub. In the right-hand sidebar, find the **Releases** section and click it. If you don't see the sidebar, scroll down on the repo homepage until you find the Releases section.

On the Releases page, click **Draft a new release** in the top-right corner.

#### Create a new tag

At the top of the draft page, there's a field labeled **Choose a tag**. Click it and type the new version number, prefixed with a `v`, for example `v3.3.5-1.0.3`.

GitHub will show a prompt that says **Create new tag: v3.3.5-1.0.3 on publish**. Click that option to confirm.

> ℹ️ Tags are permanent markers on the codebase. Once published, a tag cannot be reused for a different release.

#### Set the target branch

Below the tag field, there's a **Target** dropdown. Make sure it is set to `main` or `master`. This ensures the release is built from the latest merged changes.

#### Set the release title

In the **Release title** field, enter the version number again, for example `v3.3.5-1.0.3`. You can also add a short descriptor after it if the release has a specific indicator, like `v3.3.5-1.0.3 - Brand tokens`. The descriptor is optional, and not necessary in any way.

#### Write the release notes

> ℹ️ Release notes are optional on project teams.

This is the changelog. Write it in the large text area below the title. A good release note tells downstream teams exactly what changed and whether they need to do anything.

A changelog structure could look like this:

```markdown
## What's new

Brief summary of the release in 1-2 sentences.

## Changes

### Added

- nothing

### Updated

- `color.global.brand.primary.100–900`
- `color.neutralPalette.pure`
```

> **💡 Writing good release notes**
>
> Token names go in backticks. Keep descriptions short and factual. If downstream teams need to rename or update anything, say so clearly under Migration notes.

#### Publish the release

Click **Publish release**. The release is now live.

GitHub will automatically attach a zip of the full repo at the time of the tag. Downstream teams can reference the release tag to pull a specific version of the design repo.

## After publishing

Let the team know in Slack. Include the version number, a one-line summary of what changed, and a link to the release. If any downstream repos need to act on the changes, tag the relevant developers.

> **✅ Done**
>
> The release is published and tagged. Downstream teams can now reference it when pulling design updates into their own repos.
