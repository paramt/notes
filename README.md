---
title: README
description:
unlisted: true
date: 2026-07-15
---
This repo [(paramt/notes)](https://github.com/paramt/notes) is the Obsidian vault -- the source of truth for [param.me/notes](https://www.param.me/notes). 

[This note](https://www.param.me/notes/README/) is itself generated from the repo's [README.md](https://github.com/paramt/notes/blob/main/README.md)  
# How a note becomes a page

The site repo, [paramt/paramt.github.io](https://github.com/paramt/paramt.github.io), does the actual building. Its `scripts/sync-notes.js` copies everything from this repo into `src/data/notes/` there, automatically, before every `npm run dev` and `npm run build` That copy is disposable and gitignored on the site side — this vault is the only place to actually edit a note.

Only what's committed **and pushed** here ever reaches the live site. Uncommitted drafts sync into local/dev builds same as everything else, but CI only ever checks out pushed commits, so drafts stay private until you commit and push them.

# CI: pushing here redeploys the site

Pushing to `main` in this repo triggers `.github/workflows/notify-site.yml`, which sends a `repository_dispatch` (`notes-updated`) to [paramt/paramt.github.io](https://github.com/paramt/paramt.github.io). That fires `.github/workflows/deploy.yml` over there, which checks out both repos as siblings, runs the sync + full build, and deploys to GitHub Pages — same as pushing to the site repo directly.

# Frontmatter

Every note starts with YAML frontmatter that comes from the Templater default template at `templates/default.md`:

```yaml
---
title:
date: 2026-07-16
description:
unlisted: false
tags:
---
```

which is used to fill in metadata on [param.me/notes](https://www.param.me/notes)
