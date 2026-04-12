# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## About This Site

Personal Chinese-language blog ("火箭的博客") built with Hugo v0.147.4 extended and the [dream](https://github.com/g1eny0ung/hugo-theme-dream) theme. Published at https://huojian.tech/.

## Common Commands

```bash
# Local dev server (published posts only)
hugo server

# Local dev server including drafts
hugo server -D

# Build to public/
hugo

# Create a new post (uses archetypes/default.md)
hugo new content posts/my-post-name.md
```

> **Note:** `hugo new content` generates TOML front matter (`+++`). All published posts use YAML (`---`). Manually convert the front matter when creating a new post.

## Content Structure

- `content/posts/` — blog posts; can be flat `.md` files or page bundles (`posts/slug/index.md`)
- `content/about/` — headless bundle; sub-pages (`me.md`, `hobby.md`, etc.) make up the flippable about page
- `content/home/_index.md` — home page content
- `data1/socials.toml` — social icon links shown on the site
- `assets/css/custom.css` — custom CSS overrides (referenced in `hugo.toml`)
- `static/` — files copied as-is to `public/`

## Post Front Matter

Use YAML front matter. A typical post looks like:

```yaml
---
title: Post Title
date: 2026-01-01T10:00:00+08:00
lastmod: 2026-01-01T10:00:00+08:00
author: 火箭
categories:
  - 技术博客
tags:
  - some-tag
cover: https://tuchuang-1258410772.cos.ap-guangzhou.myqcloud.com/image.png
draft: false
slug: "url-friendly-slug"
url: "/url-friendly-slug/"
description: "SEO description"
keywords:
  - keyword1
---
```

`slug` and `url` together control the permalink. Set `draft: true` while writing; remove or set to `false` to publish.

Use a page bundle (`posts/slug/index.md`) when the post includes local images or other assets.

### Categories

Only use the established categories to keep the nav consistent:

| Category | Usage |
|---|---|
| `技术博客` | Technical / programming posts |
| `新概念` | Short explainers on a single concept (used with the `【新概念】` title prefix) |
| `日常分享` | Tooling, workflow, and daily-life sharing |
| `生活` | Personal life and reflection |

### Excerpt separator

Place `<!--more-->` in the post body to control where the summary cuts off on the listing page. Most published posts put it right after the opening paragraph(s).

## Theme Configuration

Theme options live under `[params]` in `hugo.toml`. Key settings:
- `lightTheme` / `darkTheme` — DaisyUI theme names
- `utterancesRepo` — GitHub repo used for comments
- `reorderNavItems` / `collapseNavItems` — control nav bar layout

The dream theme docs are at https://g1en.site/hugo-theme-dream.
