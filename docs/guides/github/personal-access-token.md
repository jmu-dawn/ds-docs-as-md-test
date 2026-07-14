---
title: Generate a Personal Access Token
description: How to create a GitHub Personal Access Token for syncing your design tokens with Tokens Studio.
status: stable
group: GitHub
nav_order: 2
---

A Personal Access Token (PAT) is how Tokens Studio authenticates with GitHub. Without one, the plugin cannot read or write token files in the repository. You'll need to generate a new token whenever yours expires.

> **⚠️ Use a classic token**
>
> Tokens Studio does not support fine-grained tokens. When prompted, always choose **Tokens (classic)**.

#### Sign in to GitHub

Go to [github.com](https://github.com) and sign in with your Dawn Health account.

#### Open Developer settings

1. Click your **profile picture** in the top-right corner.
2. Select **Settings** from the dropdown.
3. In the left sidebar, scroll to the bottom and click **Developer settings**.

#### Navigate to Personal Access Tokens

1. In the left sidebar, click **Personal access tokens**.
2. Select **Tokens (classic)**.

#### Create a new token

1. Click **Generate new token**, then select **Generate new token (classic)**.
2. Confirm your identity using your authenticator app when prompted.
3. In the **Note** field, give your token a recognisable name so you can identify it later. For example: `DS3 Tokens Studio`
4. Set an expiration date. **90 days** is recommended — shorter is more secure, but you'll need to regenerate more often.
5. Under **Select scopes**, check the `repo` box. This is the only permission Tokens Studio needs to read and write token files.

#### Copy and save the token

1. Scroll to the bottom and click **Generate token**.
2. Copy the token that appears.

> **🚫 Save this now**
>
> GitHub only shows the token once. If you leave this page without copying it, you'll need to generate a new one. Store it somewhere secure, such as 1Password.

#### Add the token to Tokens Studio

Open the **Tokens Studio** plugin in Figma, then follow the path that applies to you.

**If you already have a GitHub sync set up:**

1. Go to **Settings** then **Sync providers**.
2. Find your GitHub entry and click the **three dots** icon, then **Edit**.
3. Paste your token into the **Personal Access Token** field.
4. Click **Save**.

**If you're setting up sync for the first time:**

Follow the [Connect Tokens Studio to GitHub]({{ '/docs/guides/tokens-studio/set-up-github-sync/' | relative_url }}) guide.

#### Confirm the connection

After saving, Tokens Studio will prompt you to **Pull from GitHub?**. Click **Yes** to load your tokens.

Open the **Tokens** panel and check that your token sets are visible. If they are, the connection is working correctly.

> **✅ You're connected**
>
> Your tokens are now synced with GitHub. Any changes you push or pull in Tokens Studio will be reflected in the repository.

## Token maintenance

- **Treat your token like a password.** Do not share it or commit it to any file in the repository.
- **Tokens expire.** When yours expires, repeat this guide to generate a new one and update Tokens Studio.
- **Revoke old tokens** anytime from **GitHub** > **Developer settings** > **Personal access tokens**.
