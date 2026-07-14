---
title: Setting up GitHub sync in Tokens Studio
description: Connect Tokens Studio to a design repository so your design tokens stay in sync with the source of truth.
status: stable
group: Tokens Studio
nav_order: 1
---

GitHub holds the source of truth for design tokens. This guide connects Tokens Studio to a repository so you can pull the latest tokens into Figma and push your changes back to the repo. If you want to understand how the sync works or what each credential field means, see the [GitHub sync reference]({{ '/docs/guides/tokens-studio/github-sync-reference/' | relative_url }}).

## Before you start

You need three things ready before you connect the sync. If any are missing, the setup will fail.

<div class="card-grid">
  <a class="card" href="{{ '/docs/guides/github/create-github-account/' | relative_url }}">
    <h3>👤 GitHub account</h3>
    <p>Set up your Dawn Health GitHub account.</p>
  </a>
  <a class="card" href="{{ '/docs/guides/github/forking-dawn-design/' | relative_url }}">
    <h3>📁 Design repository</h3>
    <p>The repo that stores the token files. Ask your Design System Designer if you do not know which repo to use.</p>
  </a>
  <a class="card" href="{{ '/docs/guides/github/personal-access-token/' | relative_url }}">
    <h3>🔑 Personal Access Token in GitHub</h3>
    <p>Create the PAT that lets the plugin authenticate with GitHub.</p>
  </a>
</div>

> **⚠️ All three are required**
>
> You need the repository and a Personal Access Token in hand before you begin. The plugin cannot connect without them.

## Connect the sync

#### Open Tokens Studio

Open Figma and launch the Tokens Studio plugin. On the start screen, choose **New empty file**. You will pull the real tokens from GitHub in a moment, so there is no need to create anything locally first.

#### Add GitHub as a sync provider

Go to the **Settings** tab.  
Under **Sync providers**, select **Add new** and choose **GitHub** from the list.

#### Fill in your credentials

Complete the form with the values below. Leave **Base URL** empty, we do not use it at Dawn.

| Field                  | What to enter                                                                      |
| ---------------------- | ---------------------------------------------------------------------------------- |
| Name                   | The name of the repo you're connecting to. For example: `dawn-design`              |
| Personal Access Token  | The PAT from your Dawn GitHub account                                              |
| Repository             | The `owner/repo` portion of the repo URL. For example: `DawnHealthGit/dawn-design` |
| Branch                 | The branch to sync against. Usually `master`                                       |
| Token storage location | The token folder: `tokens`                                                         |

Every field is explained in detail, including why we use folder storage and the Pro licence requirement, in the GitHub sync reference:

<div class="card-grid">
  <a class="card" href="{{ '/docs/guides/tokens-studio/github-sync-reference/' | relative_url }}">
    <h3>📖 GitHub sync reference</h3>
    <p>Field-by-field reference for every credential, plus how GitHub sync works.</p>
  </a>
</div>

#### Run the initial sync

Save your credentials. The plugin compares your local tokens with the repository and prompts you to push or pull. Choose **Pull** to bring the design tokens into your file.

#### Confirm it worked

Open the **Tokens** tab. You should see every token set loaded from the repository.

Then check that the **Push to GitHub** button in the bottom left of the window is disabled. You should sit in a read-only state until you intentionally make a change, which confirms your local tokens match the remote. After you've made a change, the **Push to GitHub** button should switch to an active state, indicating that you have local changes ready to be pushed to the remote GitHub repo.

> **✅ You're all set**
>
> GitHub sync is active. Changes you push from Tokens Studio update the repository, and you can pull updates from the repo at any time.

## Keeping in sync

As you work, the plugin shows push and pull indicators that remind you to keep your local tokens aligned with GitHub. Sync regularly so design and development stay on the same set of tokens.

<div class="card-grid">
  <a class="card" href="#">
    <h3>📖 Sync changes</h3>
    <p>How to push and pull tokens once your sync is connected. (Coming soon!)</p>
  </a>
  <a class="card" href="{{ '/docs/guides/github/create-new-release/' | relative_url }}">
    <h3>📖 Creating releases</h3>
    <p>How to create a new release so developers can pull the latest token updates.</p>
  </a>
</div>
