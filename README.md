# minimdm-site

Marketing and landing page for [miniMDM](https://github.com/planemarlin/minimdm) — a minimal, lightweight, open-source Master Data Management application.

## About

This is a static HTML/CSS site that serves as the public-facing front page for the miniMDM project. It covers features, screenshots, a comparison table, and links to the documentation in the main repo.

## Structure

```
index.html           # Main page
site.css             # Stylesheet (extends the app's design language)
assets/
  screens/           # Application screenshots used in the page
```

## Local development

No build step required. Serve the directory with any static file server:

```bash
# Python (built-in)
python3 -m http.server 8181

# Node (if available)
npx serve .
```

Then open [http://localhost:8181](http://localhost:8181).

## Deployment

Drop the files on any static hosting provider (GitHub Pages, Netlify, Vercel, Cloudflare Pages, or a plain web server). No server-side processing is needed.

The latest release version is fetched at runtime from the GitHub API and cached in `localStorage` for one hour, so the version badge stays current without a rebuild.

## Contributing

This site tracks the main miniMDM repo. If a feature is added, removed, or renamed there, please open a PR here to keep the page accurate.

For contributions to miniMDM itself, see [CONTRIBUTING.md](https://github.com/planemarlin/minimdm/blob/main/CONTRIBUTING.md) in the main repo.

## License

MIT — same as the main miniMDM project.
