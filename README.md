# SudeshDahale – Personal Portfolio & Documentation Site

A static, monolithic site showcasing projects, blog posts, and personal documentation.

## Overview

This repository contains the source for a static personal website built as a single‑page monolith. All content—including the project overview, usage instructions, blog posts, and other documentation—is stored in Markdown and rendered by a static site generator. The site is designed to be simple to clone, build, and deploy to any static‑hosting provider (GitHub Pages, Netlify, Vercel, etc.).

## Features

- Single‑repo monolith: HTML, CSS, JS, and all content live together for easy maintenance.
- Markdown‑driven documentation and blog posts, automatically converted to static pages.
- Responsive, mobile‑first design with a clean, modern UI.
- Zero‑runtime dependencies – the site can be built with just a static site generator or even pure HTML/CSS.
- Simple deployment to any static‑hosting platform using a single `build` command.

## Quick Start

```bash
```bash
# Clone the repository
git clone https://github.com/SudeshDahale/SudeshDahale.git
cd SudeshDahale

# If the site uses a static‑site generator (e.g., Jekyll, Hugo, or plain npm scripts), install dependencies
echo "# Install dependencies if a package.json exists"
if [ -f package.json ]; then npm install; fi

# Build the static site
echo "# Build the site – adjust the command to the generator used"
if [ -f package.json ]; then npm run build; fi
# For Jekyll: jekyll build
# For Hugo: hugo

# Preview locally (optional)
echo "# Serve locally to test"
if [ -f package.json ]; then npm run serve; fi
# For Jekyll: jekyll serve
# For Hugo: hugo server
```
```

## Architecture

The project follows a static‑site monolithic architecture: source files (Markdown, assets, templates) reside in a flat hierarchy, a build step compiles them into static HTML/CSS/JS, and the resulting `dist/` folder can be served directly without a backend.

---
*This file is kept in sync by [AutoScribe](https://github.com) — edits here may be overwritten on the next sync.*
