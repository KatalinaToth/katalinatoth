# katalinatoth.github.io

Personal academic website for Katalina Toth, Pre-Doctoral Research Fellow at the Institute for Quantitative Social Science, Harvard University.

## Tech Stack

- **Hugo** (extended) — static site generator
- **GitHub Pages** — hosting
- **GitHub Actions** — automated deployment

## Local Development

```bash
# Install Hugo (macOS)
brew install hugo

# Run local server
hugo server -D

# Build for production
hugo --gc --minify
```

## Deployment

Push to `main` branch. GitHub Actions builds and deploys automatically.

## Structure

```
├── assets/css/style.css    — all styles
├── content/_index.md       — homepage bio
├── content/blog/           — blog posts
├── data/                   — papers, teaching, awards (YAML)
├── layouts/                — Hugo templates
├── static/files/           — PDFs (CV, papers)
├── static/images/          — photos
└── hugo.yaml               — site configuration
```

## Updating Content

See [UPDATING.md](UPDATING.md) for instructions on adding papers, blog posts, and other content.
