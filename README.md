# hello-jason

Personal portfolio site of Jason Zhang — a single-file, theme-aware, i18n (zh/en) personal website.

## Features

- **Single-file deliverable** — `index.html` is the whole site. No build step, no bundler, no external runtime dependencies.
- **Dark / Light mode** — Persisted via `localStorage`, follows `prefers-color-scheme` on first visit, no flash on load.
- **i18n (中文 / English)** — Full bilingual content driven by a single `I18N` dictionary, no duplicated HTML.
- **URL-parameter overrides** — `?theme=dark&lang=en` for shareable state.
- **Keyboard shortcuts** — `D` toggles theme, `L` toggles language (guarded against input focus).
- **Colophon** — Versioned change log at the bottom of the page.
- **Performance** — Inter / Noto Sans SC / JetBrains Mono loaded with `preconnect` + `display=swap`; system-font fallbacks everywhere.
- **Responsive & a11y** — Semantic landmarks, reduced-motion respected, keyboard-operable.

## Deployment

Deployed as a GitHub Pages **project site** at:

- Live URL: https://zjszjs007.github.io/hello-jason/

### Local preview

```bash
python -m http.server 8000
# open http://127.0.0.1:8000/
```

### Deploy to GitHub Pages

1. In repo Settings → Pages → **Deploy from a branch** → `main` / `/ (root)`.
2. Wait 1–3 minutes for the first build.
3. The empty `.nojekyll` file prevents Jekyll from processing underscores.

## Structure

```
.
├── index.html     # The entire site (HTML + CSS + JS, inline)
├── .nojekyll      # Disable Jekyll processing on GitHub Pages
└── .gitignore
```

## License

Personal portfolio. © Jason Zhang.
