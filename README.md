---
title: README
description: how this vault connects to the site build
unlisted: true
---
This repo [(paramt/notes)](https://github.com/paramt/notes) is the Obsidian vault — the source of truth for [param.me/notes](https://www.param.me/notes). It has no build of its own; it just holds markdown notes plus `images/`, and `.obsidian`/`templates` (both gitignored, editor-only).

## Frontmatter

Every note starts with YAML frontmatter, matching the Templater default template at `templates/default.md`:

```yaml
---
title:
date: 2026-07-16
description:
unlisted: false
tags:
---
```

- `title` — the page `<h1>` and `<title>`.
- `date` — auto-filled on file creation (`YYYY-MM-DD`). Drives sort order on `/notes`, the sitemap `lastmod`, and `datePublished`/`dateModified` in the note's structured data.
- `description` — meta description, Open Graph/Twitter description, and the subtitle shown under the title.
- `unlisted` — `false` by default. Set `true` to keep the permalink working (like this note) while hiding it from the `/notes` listing, injecting `noindex`, and excluding it from `sitemap.xml`.
- `tags` — optional, as a block list:
  ```yaml
  tags:
    - poker
    - puzzles
  ```
  Rendered as badges on the note and listing. The frontmatter parser is a small hand-rolled one (not full YAML) — only this block-list form works; inline arrays like `tags: [poker, puzzles]` won't parse.

## How a note becomes a page

The site repo, [paramt/paramt.github.io](https://github.com/paramt/paramt.github.io), does the actual building. Its `scripts/sync-notes.js` copies everything from this repo into `src/data/notes/` there, automatically, before every `npm run dev` and `npm run build` That copy is disposable and gitignored on the site side — this vault is the only place to actually edit a note.

Only what's committed **and pushed** here ever reaches the live site. Uncommitted drafts sync into local/dev builds same as everything else, but CI only ever checks out pushed commits, so drafts stay private until you commit and push them.

## CI: pushing here redeploys the site

Pushing to `main` here triggers `.github/workflows/notify-site.yml`, which sends a `repository_dispatch` (`notes-updated`) to [paramt.github.io](https://github.com/paramt/paramt.github.io). That fires `.github/workflows/deploy.yml` over there, which checks out both repos as siblings, runs the sync + full build, and deploys to GitHub Pages — same as pushing to the site repo directly.

This requires a `SITE_DISPATCH_TOKEN` secret here (a PAT with write access to `paramt.github.io`), since triggering a dispatch needs write auth on the target even though both repos are public.
