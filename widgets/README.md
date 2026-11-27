# Widgets

Interactive React components that notes embed with a fenced block:

````md
```widget mac-studio-resale
some-prop: value
```
````

Each widget is a folder here. The folder name is the widget name, and `index.jsx` default-exports the component. Its `key: value` lines arrive as string props.

These files are only built by the site repo (paramt.github.io). Its sync copies this folder to `src/data/notes/widgets/`, which auto-registers every `widgets/*/index.jsx`. Imports such as `react` and `d3` resolve from the site's `node_modules`, so a new npm dependency gets added there.

## Rules

- **Must work on mobile.** Notes are read on phones (~320–430px wide). Size to the container (never a fixed width), and make labels shorter, stacked or right-aligned at small widths so nothing overlaps, clips or causes horizontal page scroll. Check every widget change at 320px, 390px and desktop width before shipping (see below).
- No `window`/`document` during render. Pages are prerendered, so do DOM work in `useEffect`.
- Dark mode is `html[data-theme="dark"]`, not `prefers-color-scheme`. Check both themes.

## Checking a widget

From the site repo (with this repo checked out next to it as `../notes`): `npm run build && npx vite preview`, then open a note that uses the widget. Screenshot it at 320px, 390px (or Playwright's `iPhone 13` device) and ~1100px wide, in light and dark. Confirm that labels don't overlap or clip, that `document.documentElement.scrollWidth <= window.innerWidth`, and that the console has no errors.
