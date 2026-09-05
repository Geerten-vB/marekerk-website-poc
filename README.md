# Astro + Markdown + GitHub Pages starter

A tiny proof-of-concept for a Git-first content website.

## Local development

Install dependencies and start Astro:

```bash
npm install
npm run dev
```

Open the local URL shown by Astro.

## Edit the website text

Most editors only need to touch:

`src/content/page.md`

The frontmatter at the top controls the hero title and subtitle:

```md
---
title: Welcome to our website
subtitle: This text is controlled by Markdown.
---
```

Everything after the closing `---` is rendered as Markdown inside the developer-controlled `<article>` on the homepage.

## GitHub Pages

1. Create a GitHub repository and push this project to the `main` branch.
2. In GitHub, open **Settings → Pages**.
3. Set the source to **GitHub Actions**.
4. Push a change to `main`.
5. The workflow builds and deploys the Astro site.

For a repository URL such as `https://YOURNAME.github.io/my-site`, the config automatically uses `/my-site` as Astro's base path in GitHub Actions.

For a custom domain, set `SITE_URL` in the workflow/environment to your full URL, such as `https://example.com`.
