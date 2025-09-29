# Project Airos Website Deployment Guide

The Project Airos site lives in the [`site/`](../site) directory. It is a static bundle (HTML, CSS, and a small JavaScript
snippet) that can be hosted on any CDN or static web platform.

## 1. Prepare the build

Because the site is already static, the "build" step is simply ensuring all files under `site/` are up to date.

```bash
cd site
python -m http.server 8000  # optional sanity check locally
```

Commit and push your changes once you are satisfied with the preview.

## 2. Deploy to GitHub Pages

1. Create a branch and push the updated site content.
2. In the GitHub repository, enable **GitHub Pages** with the `main` branch and `/site` folder.
3. GitHub will automatically serve the content at `https://<org>.github.io/<repo>/`.
4. When you merge new updates into `main`, Pages will redeploy.

> Tip: if you prefer a dedicated branch such as `gh-pages`, add a GitHub Action that copies the `site/` directory into that
> branch on every push.

## 3. Deploy to Netlify or Vercel

1. Connect the repository to your hosting provider.
2. Configure the project to serve from the `site` directory with no build command (or `cp -r site/* public/` if a step is
   required).
3. Every push to the configured branch will trigger a redeploy.

## 4. Manual hosting / S3 + CloudFront

1. Zip the contents of `site/` and upload them to an S3 bucket configured for static site hosting.
2. Invalidate the CDN cache (CloudFront or similar) after uploading new versions.
3. Automate the upload with a script if you frequently update content.

## 5. Content workflow best practices

- **Preview first**: use `python -m http.server` or a Live Server plugin to view updates locally.
- **Branch per update**: collaborate via pull requests to review copy, visuals, and layout changes.
- **Track assets**: store future imagery under `site/assets/` and optimize (WebP/AVIF) before commit.
- **Document releases**: summarize major content updates in the blog section to keep visitors informed.

With these steps you can iterate quickly on the Project Airos site and publish changes to production safely.
