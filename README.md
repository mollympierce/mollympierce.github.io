# mollypiercedesign.com

Static Astro migration of the mirrored Molly Pierce Design Webflow site. The production site uses the real mirrored copy, portfolio pages, Webflow styles, and locally hosted assets.

## Local development

Requires Node.js 22 or newer.

```bash
npm ci
npm run dev
```

Astro serves the site at `http://localhost:4321`.

## Production build

```bash
npm run build
npm run preview
```

`npm run build` runs `astro check` and writes the static site to `dist/`.

## Project structure

The checked-in site is standard Astro route files in [`src/pages`](/Users/jsiler/Development/mollypiercedesign.com/src/pages).

Static assets are hosted locally under `public/assets/`:

- `public/assets/images`
- `public/assets/fonts`
- `public/assets/files`
- `public/assets/css`
- `public/assets/js`

## GitHub Pages deployment

The existing `.github/workflows/deploy.yml` workflow installs dependencies, builds the site, uploads `dist/`, and deploys it to GitHub Pages on pushes to `main`.

GitHub Pages must use **GitHub Actions** as its source. `public/CNAME` preserves the custom domain `mollypiercedesign.com`.
