# Contributing

This site is content-first. Most contributions are new articles or edits to existing ones.

## Adding a new guide

1. Create a file in `_posts/` named `YYYY-MM-DD-your-slug.md` where `your-slug` matches the article's H1 (kebab-case).
2. Use the front matter below.
3. Write 800-1500 words, 5 sections: pain-point opening / existing-options table / recommended technical path / FAQ / conclusion + commercial block.
4. Place the commercial block at the very end (do not mention pricing or brand in the body).
5. Open a pull request.

## Front matter template

```yaml
---
layout: post
title: "How to watch X in Y (2026 guide)"
date: 2026-10-15 09:00:00 +0800
categories: [guides]
description: "One-line meta description for SEO."
---
```

## Local preview

Requires Ruby 3.1+ and Bundler.

```bash
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000/> in your browser.

The local server runs at the site root. The `/overseas-chinese-tv-guide/` subpath only applies when the site is served by GitHub Pages, so do not add a `baseurl` locally.

## Style rules

- All prices and feature descriptions must be sourced from the service's public page as of the article date. Add a "may change" disclaimer at the bottom of the commercial block.
- The commercial block is mandatory but should remain neutral. Do not repeat the brand name in the article body.
- The HTML for the CTA button is already provided by the post layout — do not paste additional HTML in the article body.

## License

By contributing, you agree to license your content under CC BY 4.0 (matching the rest of `_posts/`).
