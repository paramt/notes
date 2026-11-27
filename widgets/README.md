# Widgets

Interactive React components that notes embed with a fenced block:

````md
```widget mac-studio-resale
some-prop: value
```
````

Each widget is a folder here. The folder name is the widget name, and `index.jsx` default-exports the component. Its `key: value` lines arrive as string props.

These files are only built by the site repo (paramt.github.io). Its sync copies this folder to `src/data/notes/widgets/`, which auto-registers every `widgets/*/index.jsx`. Imports such as `react` and `d3` resolve from the site's `node_modules`, so a new npm dependency gets added there.

Rules: no `window`/`document` during render (pages are prerendered; do DOM work in `useEffect`), and dark mode is `html[data-theme="dark"]`, not `prefers-color-scheme`.
