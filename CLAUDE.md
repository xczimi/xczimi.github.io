# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based GitHub Pages site serving as a personal resume/portfolio for Peter Czimmermann (`xczimi`). The site uses the `jekyll-theme-minimal` theme and contains a single main content page.

## Architecture

- **Jekyll Static Site**: Uses GitHub Pages with Jekyll for automatic deployment
- **Theme**: `jekyll-theme-minimal` configured in `_config.yml`
- **Content**: Single-page resume in `index.md` with markdown formatting
- **Deployment**: Automatic via GitHub Pages when pushing to `master` branch

## Key Files

- `_config.yml`: Jekyll configuration with theme specification
- `index.md`: Main resume content with personal information, skills, and experience
- Repository serves content at `https://xczimi.github.io`

## Content Structure

The `index.md` file contains structured resume sections:
- Personal information and contact details
- Skills summary with technologies and tools
- Experience section with detailed work history (Kantar/Lightspeed Research, Vancouver Southsiders, MLab Research)
- Chronological career progression from 2000 to present

## Development Notes

- No build process required - GitHub Pages handles Jekyll compilation automatically
- Changes to `master` branch deploy immediately to live site
- Markdown content is rendered using Jekyll's markdown processor
- Theme provides minimal styling suitable for professional resume presentation