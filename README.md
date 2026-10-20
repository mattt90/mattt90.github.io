# Brew City Data

The company website and data & AI blog for Brew City Data, built with Jekyll and the [Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/).

## Local development

Use the included devcontainer with VS Code and a supported container runtime, or install Ruby and Bundler locally.

```sh
bundle install
bundle exec jekyll serve --livereload
```

Open `http://localhost:4000`. Restart Jekyll after changing `_config.yml`.

To produce the static site:

```sh
bundle exec jekyll build
```

The generated output is in `_site/`; edit source files rather than generated HTML.

## Site structure

- `index.html`: company introduction, focus areas, founder cards, and recent posts.
- `_pages/`: about, contact, founder directory, two founder profiles, and blog archives.
- `_data/navigation.yml`: main navigation.
- `_data/authors.yml`: shared founder names, bios, profile URLs, and avatars.
- `_posts/`: articles about data and AI.
- `assets/css/main.scss`: theme settings and responsive company styling.
- `assets/images/brew-city-data.svg`: company mark and favicon.

## Personalize before launch

The two founder profiles are deliberately generic. Replace "Founder One" and "Founder Two" in `_data/authors.yml` and the corresponding page titles and biographies in `_pages/founder-one.md` and `_pages/founder-two.md`. Keep the author keys (`founder-one` and `founder-two`) stable to preserve article attribution, or update matching post front matter when changing them.

Add real contact details to `_pages/contact.md`, and remove the placeholder notices when the profiles are ready. The included blog articles are starter editorial content for review, not claims about past client work.

The existing `CNAME` domain is unchanged. Before deployment, confirm the production domain and set `url` in `_config.yml` to its HTTPS origin. Set `baseurl` only if deploying under a subpath.

## Publish an article

Create `_posts/YYYY-MM-DD-your-title.md`:

```yaml
---
title: "Your article title"
author: founder-one
categories:
  - data
tags:
  - analytics
excerpt: "A short summary for listings and search."
---
```

Write the article below the front matter. Use `founder-one` or `founder-two` for attribution and `data` or `ai` for the main topic. Posts appear automatically on the homepage, blog archive, matching founder profile, topic and tag archives, search, and RSS feed. Jekyll does not publish future-dated posts by default.
