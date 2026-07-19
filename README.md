# paulinavl.github.io

My personal site — a live, story-driven CV. Studies, teaching, research, and the projects I keep building on the side, in English, Spanish, and Traditional Chinese.

**Live:** [paulinavl.github.io](https://https://github.com/Poln4/paulinavl.github.io)

## What's here

A single static page (`index.html`) — no build step, no dependencies to install. Everything lives in one file on purpose, so it's easy to edit directly on GitHub or drop into any static host.

- **Two visual themes** — a light "marker on whiteboard" mode and a dark "chalk on chalkboard" mode, toggled top-right. The choice is remembered between visits.
- **Three languages** — English, Spanish, and 中文 (繁體), toggled top-right next to the theme switch. Also remembered between visits.
- **A CEFR-level rail** — the vertical stamp trail on the left lights up as you scroll, mapping the page's sections (origins → teaching → research → projects → the honest stuff → what's next) to reading levels A1–C2, since that's literally what my research measures.
- Sections: origins, a full teaching timeline, doctoral + master's research (the CARLA model, Study 1 & 2), projects (ZebraUp, Reading Club, leehzn, NAS Project, the Carla Model), publications, the honest "messy middle," toolkit, and a support/contact section.

## Editing content

Everything is in `index.html`. Text that appears in more than one language is wrapped like this:

```html
<div class="i18n" data-lang="en"> ... English ... </div>
<div class="i18n" data-lang="es" style="display:none"> ... Español ... </div>
<div class="i18n" data-lang="zh" style="display:none"> ... 中文 ... </div>
```

To edit a section, find all three `data-lang` blocks for it and update each — the JavaScript at the bottom just toggles which one is visible (`style.display`) based on the selected language, saved to `localStorage`.

Elements that don't need translating (proper nouns, tech tags, the teaching ledger) aren't wrapped and appear the same in every language.

## Adding a new project

Copy one of the existing `.card` blocks inside `<section id="projects">`, keeping the three `.i18n` paragraphs, and drop it into the `.grid.two` container. For something bigger, copy the `.spotlight` block (used for ZebraUp) instead — it gets full-width treatment with its own link row.

## Local preview

No build tools needed — open `index.html` directly in a browser, or serve it locally:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deployment

This repo is a GitHub Pages user site (`<username>.github.io`), so anything pushed to `main` at the repo root goes live automatically — no Actions or build config required.

```bash
git add index.html
git commit -m "update site"
git push
```

Changes are typically live within a minute or two.

## Stack

Plain HTML, CSS (custom properties for theming), and vanilla JavaScript. Fonts via Google Fonts (Kalam, Caveat, Source Serif 4, IBM Plex Mono, Noto Sans TC). No frameworks, no npm install.

## Contact

[paoo.ss@gmail.com](mailto:paoo.ss@gmail.com) · [LinkedIn](https://linkedin.com/in/paulina-valenzuela-lagos) · [ORCID](https://orcid.org/0009-0006-1635-7823)
