# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Jekyll-based GitHub Pages site serving as the resume of Peter Czimmermann (`xczimi`) at https://xczimi.github.io. It uses the `sproogen/resume-theme` remote theme, so all resume content lives in `_config.yml`, not in markdown pages.

## Key Files

- `_config.yml`: all resume content (about text, experience, projects, skills) plus theme settings. Edit this to change the resume.
- `index.md`: front matter only; the theme renders the page from `_config.yml`.
- `assets/main.scss`, `images/`: styling overrides and the profile picture.
- `Gemfile`: `github-pages` plus `webrick` (needed to run `jekyll serve` on Ruby 3).

## Content Rules

- No compensation figures, no customer names, no names of colleagues or direct reports, no internal codenames. Keep industry-level descriptions.
- Plain first-person voice in `about_content`; impersonal past tense in experience entries.
- Use numbers only where they size something a reader would otherwise have to guess. No activity counts (PRs, releases, documents written).

## Local Preview

GitHub Pages builds the site on push to `master`, so no local build is required. For a local preview with a mise-managed Ruby:

```
mise exec ruby@3.3 -- bundle install
mise exec ruby@3.3 -- bundle exec jekyll serve
```

Jekyll does not reload `_config.yml` automatically; restart the server after editing it.
