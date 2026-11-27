# Notes vault

This repo is the Obsidian vault behind param.me/notes. The site (paramt/paramt.github.io, a sibling checkout at `../paramt.github.io`) syncs this whole repo at build time; pushing to `main` triggers a site rebuild and deploy. Keep all note content and its commits here.

- **Notes** are top-level `*.md` files with frontmatter (`title`, `date`, `description`, `tags`, `unlisted`). Notes are unlisted unless the frontmatter says `unlisted: false`. Rendering details live in the site repo's `.claude/docs/notes.md`.
- **Interactive widgets** live in `widgets/<name>/index.jsx` and are embedded with a ```` ```widget <name> ```` fenced block. Read `widgets/README.md` before adding or changing one. Every widget must work on mobile, and you check it at phone widths before shipping.
- A note that uses a widget must land together with, or after, that widget's folder. An unknown widget name fails the site build.
