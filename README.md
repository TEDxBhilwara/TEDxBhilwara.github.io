# TEDxBhilwara

Official website for [TEDxBhilwara](https://tedxbhilwara.com) — a locally organized TEDx event in Bhilwara, India.

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Main landing page with about, speakers, participate, salon, partners, and contact sections |
| Media | `media.html` | Media coverage and press logos |
| Speaker Registration | `speaker-reg.html` | Speaker nomination form (Google Form embed) |
| Blog | `blog.html` | Blog (currently empty) |

## Tech Stack

- **Framework:** [Materialize CSS](https://materializecss.com/) (v0.x)
- **Fonts:** Self-hosted Roboto + Material Design Icons (`font/`)
- **Lightbox:** Magnific Popup
- **No build step** — plain HTML/CSS/JS, served directly by GitHub Pages

## Project Structure

```
/
├── index.html
├── blog.html
├── media.html
├── speaker-reg.html
├── favicon.ico
├── CNAME               # Points tedxbhilwara.com to this repo
├── css/
│   ├── materialize.min.css
│   ├── magnific-popup.css
│   └── style.css       # Custom overrides
├── js/
│   ├── materialize.min.js
│   ├── magnific-popup.js
│   └── init.js
├── font/
│   ├── roboto/
│   └── material-design-icons/
└── images/
    ├── background/
    ├── icons/
    ├── media/
    ├── partners/
    └── speakers2015/
```

## Development

No build process required. Edit files directly and open in a browser.

```bash
# Clone the repo
git clone https://github.com/tedxbhilwara/tedxbhilwara.github.io.git
cd tedxbhilwara.github.io

# Open locally
open index.html
```

## Deployment

Pushing to `master` deploys automatically via GitHub Pages to [tedxbhilwara.com](https://tedxbhilwara.com). There is no staging environment.

## License

MIT — see [LICENSE](LICENSE).
