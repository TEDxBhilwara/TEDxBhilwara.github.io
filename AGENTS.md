# AGENTS.md

## Project Overview

Static GitHub Pages site for TEDxBhilwara — a locally organized TEDx event in Bhilwara, India.
No build step. No package manager. Pure HTML/CSS/JS served directly by GitHub Pages.

## Structure

```
/
├── index.html          # Homepage
├── blog.html           # Blog (currently empty)
├── media.html          # Media coverage
├── speaker-reg.html    # Speaker registration (embeds a Google Form)
├── favicon.ico
├── css/                # Stylesheets
│   ├── materialize.min.css
│   ├── magnific-popup.css
│   └── style.css       # Custom overrides
├── js/                 # Scripts
│   ├── materialize.min.js
│   ├── magnific-popup.js
│   └── init.js         # Materialize initialization
├── font/               # Self-hosted fonts (Roboto + Material Design Icons)
└── images/             # Site images
    ├── background/
    ├── icons/
    ├── media/
    ├── partners/
    └── speakers2015/
```

## Key Constraints

- **HTML files must stay at the repository root.** GitHub Pages serves the site from root; moving HTML files will break the domain.
- **Do not move `css/`, `js/`, `font/`, or `images/`.** Asset paths are hardcoded in HTML files and the font paths in `materialize.min.css` use relative references (`../font/...`). Moving these directories requires updating all references carefully.
- **No build process.** There is no npm, webpack, or any compilation step. Edit files directly.

## Conventions

- Use only the minified versions of third-party libraries (`materialize.min.css`, `materialize.min.js`). The unminified versions are not included.
- CSS framework: [Materialize](https://materializecss.com/) (v0.x).
- `style.css` is for custom overrides only — do not edit framework files.
- Images are committed directly to the repo (no CDN or Git LFS currently in use).

## Deployment

Pushing to `master` deploys automatically via GitHub Pages. There is no staging environment.
