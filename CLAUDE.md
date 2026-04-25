# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a GitHub Pages portfolio site for Roman Shtykov, built with Jekyll using the `jekyll-theme-minimal` theme. It is deployed automatically by GitHub Pages on push to `master`.

## Structure

- `index.md` — the entire site content (Markdown with YAML front matter support)
- `_config.yml` — Jekyll configuration: site title, description, and theme

## Local Development

To preview locally, you need Ruby and Bundler. If a `Gemfile` doesn't exist yet, create one with:

```ruby
source "https://rubygems.org"
gem "github-pages", group: :jekyll_plugins
```

Then:

```bash
bundle install
bundle exec jekyll serve
```

The site will be available at `http://localhost:4000`.

## Deployment

Push to `master` — GitHub Pages builds and deploys automatically. No CI/CD configuration is needed.

## Content Editing

All visible content lives in `index.md`. The theme is controlled solely by `_config.yml` (`theme: jekyll-theme-minimal`). There are no layouts, includes, assets, or CSS overrides in this repo — the theme provides everything.
