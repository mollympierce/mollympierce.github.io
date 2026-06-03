# mollypiercedesign.com

Astro static-site rebuild scaffold for the archived `mollypiercedesign.com` website.

## Recovery policy

Use the most recent archive capture as the canonical source. Defer to older captures only when pages or assets are missing from the latest capture.

## Local development

```bash
npm install
npm run dev
```

## Production build

```bash
npm run build
npm run preview
```

## GitHub Pages deployment

This repository includes `.github/workflows/deploy.yml`, which builds Astro and deploys `dist/` to GitHub Pages on pushes to `main`.

The `public/CNAME` file is set to:

```text
mollypiercedesign.com
```

After the repo exists, configure GitHub Pages to use GitHub Actions, then point DNS for `mollypiercedesign.com` at GitHub Pages.

## Archive migration notes

The current files are a clean scaffold. The actual archive scrape still needs to be added once the Wayback capture URLs and assets are obtainable from the runtime or manually exported.
