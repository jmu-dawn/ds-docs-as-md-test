# ds-docs-as-md-test

A design system documentation site built with **plain Jekyll** — the engine
GitHub Pages runs natively. No Fumadocs, no third-party doc framework. You write
Markdown; GitHub builds the site.

## Structure

```
.
├── _config.yml              # Site config
├── index.md                 # Landing page
├── docs/                    # All documentation (.md)
│   ├── index.md             # Docs overview
│   ├── getting-started/     # ← a subfolder = a sidebar group
│   ├── foundations/
│   └── components/
├── _layouts/                # HTML templates (default / home / doc)
├── _includes/sidebar.html   # Auto-generated docs nav
└── assets/css/style.css     # Styles
```

## Writing docs

Create a `.md` file anywhere under `docs/`. **Each subfolder becomes a group**
in the sidebar. A page only needs a title:

```markdown
---
title: My Page
nav_order: 2        # optional: order within its group (lower = higher)
description: One-line summary shown under the heading.
group: Custom Label # optional: override the auto folder-name label
---

Your Markdown content here.
```

The `layout: doc` is applied automatically to everything under `docs/`
(see `_config.yml`), so you don't set it per file.

## Publishing on GitHub Pages

1. Push to GitHub.
2. Repo **Settings → Pages**.
3. Under **Build and deployment**, set **Source: Deploy from a branch**,
   branch **main**, folder **/ (root)**. Save.
4. The site builds automatically at `https://<user>.github.io/<repo>/`.

> **Project sites:** because the URL includes `/<repo>/`, open `_config.yml` and
> set `baseurl: "/<repo-name>"`. All internal links use `relative_url`, so they
> resolve correctly once `baseurl` is set. For a user/org site or a custom
> domain, leave `baseurl` empty.

## Local preview (optional)

```bash
bundle install
bundle exec jekyll serve
# → http://localhost:4000
```
