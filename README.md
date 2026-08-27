# SudeshDahale – Personal Documentation Hub

A single‑source markdown repository for Sudesh Dahale's projects, notes, and technical write‑ups.

## Overview

This repository is a static, monolithic markdown site that consolidates all of Sudesh Dahale's documentation into one place. It contains human‑readable guides, project overviews, and technical notes, all written in plain Markdown and rendered via any static‑site generator or simply viewed in a markdown viewer. The layout is deliberately simple: a top‑level README provides navigation to the various markdown files that make up the documentation suite.

## Features

- Centralized markdown documentation for all personal and professional projects.
- Clear navigation structure driven by the top‑level README.
- Zero‑runtime dependencies – view locally with any markdown viewer or host on GitHub Pages.
- Version‑controlled documentation that evolves with the codebase.

## Quick Start

```bash
git clone https://github.com/SudeshDahale/SudeshDahale.git
cd SudeshDahale
# View locally with a markdown viewer, e.g.:
# macOS: open README.md
# Linux: xdg-open README.md
# Or serve as a static site using a simple tool like mdbook or MkDocs:
# pip install mkdocs
# mkdocs serve
```

## Architecture

The repository follows a static‑site, monolithic architecture: a single Markdown tree serves as the entire content layer, with no separate services or back‑end components. All documentation lives under the repository root, and rendering is performed by the consumer (browser, markdown viewer, or static‑site generator).

---
*This file is kept in sync by [AutoScribe](https://github.com) — edits here may be overwritten on the next sync.*
