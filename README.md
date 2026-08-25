# Sudesh Dahale Portfolio & Documentation

A static site showcasing Sudesh Dahale’s projects, resume, and technical documentation.

## Overview

This repository houses a static website that serves as Sudesh Dahale’s personal portfolio and documentation hub. Built with plain HTML, CSS, and optional client‑side JavaScript, the site presents an overview of Sudesh’s professional background, links to projects, a résumé, and detailed documentation for his work. All content is organized in markdown files that are rendered as static pages, making the site lightweight, easy to host, and straightforward to maintain.

## Features

- Responsive, mobile‑first design for seamless viewing on any device.
- Project showcase with descriptions, screenshots, and live demo links.
- Embedded résumé download (PDF) and contact form using a third‑party form handler.
- Markdown‑based documentation section that can be extended with new pages.
- Simple deployment: can be hosted on GitHub Pages, Netlify, or any static‑site host.

## Quick Start

```bash
git clone https://github.com/SudeshDahale/SudeshDahale.git
cd SudeshDahale
# No build step required – open the site locally
python -m http.server 8000   # or any static server of your choice
# Then navigate to http://localhost:8000 in your browser
```

## Architecture

The project follows a classic static‑site architecture: source files (HTML, CSS, JS, and markdown) reside in the repository; the browser directly serves these assets without server‑side processing. Documentation pages are written in markdown and converted to HTML at build time (if a static site generator is added) or served as pre‑rendered HTML. This simple, file‑based structure ensures fast load times and easy hosting.

---
*This file is kept in sync by [AutoScribe](https://github.com) — edits here may be overwritten on the next sync.*
