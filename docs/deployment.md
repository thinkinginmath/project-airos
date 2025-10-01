# Project Airos Website Deployment Guide

The Project Airos site lives in the [`site/`](../site) directory and is implemented with the [Astro](https://astro.build/) framework. Astro builds a static bundle (HTML, CSS, and JavaScript) that can be hosted on any CDN or static web platform.

## 1. Install dependencies & build

Run these commands from the repository root when you need to publish an update:

```bash
cd site
npm install          # first time or when dependencies change
npm run build        # generates the production-ready bundle in site/dist
```

Use `npm run dev` for live preview while editing content, and `npm run preview` to sanity-check the optimized build locally.

## 2. Deploy to GitHub Pages

1. Commit the site changes (no need to commit the `dist/` output).
2. Configure a GitHub Action to run `npm install` and `npm run build` inside `site/` on your chosen branch.
3. Use the official [pages deploy action](https://github.com/actions/deploy-pages) (or similar) to publish `site/dist` to GitHub Pages.
4. After the workflow completes, the site is available at `https://<org>.github.io/<repo>/`.

> Tip: You can alternatively target a dedicated `gh-pages` branch by having the workflow upload the build artifacts there.

## 3. Deploy to Netlify or Vercel

1. Connect the repository in the hosting dashboard.
2. Set the build command to `npm run build` and the publish directory to `dist`.
3. Ensure the working directory is `site/` (most hosts support this as an advanced setting).
4. Every push to the configured branch will trigger a fresh Astro build and redeploy.

## 4. Manual hosting / S3 + CloudFront

1. After running `npm run build`, upload the contents of `site/dist/` to your bucket or server.
2. Configure the bucket for static site hosting (index document `index.html`).
3. Invalidate your CDN cache (CloudFront or similar) after uploading new versions.

## 5. Content workflow best practices

- **Preview first**: `npm run dev` provides instant hot reload while editing copy or layouts.
- **Branch per update**: collaborate via pull requests to review content, visuals, and layout changes.
- **Track assets**: store imagery or downloads under `site/public/` (served statically) and optimize before commit.
- **Document releases**: summarize major content updates in the blog section to keep visitors informed.

Following this workflow keeps the Astro site fast to iterate on and simple to deploy across hosting providers.
