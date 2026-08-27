# Technical Architecture Guide for SudeshDahale Documentation Repository

## System Overview
The repository is a static documentation site consisting solely of Markdown files, primarily README.md. It follows a monolithic static documentation architecture, where content, build, and delivery are tightly coupled within the repository.

## System Layers
### Content Layer
**Technologies:** Markdown, Git

Markdown source files stored in the repository, version‑controlled with Git.

### Build Layer
**Technologies:** GitHub Actions, Static Site Generator (e.g., Jekyll, MkDocs)

Processes that render Markdown to HTML for publishing, typically using static site generators or GitHub Actions.

### Presentation Layer
**Technologies:** GitHub Pages, HTML, CSS

The web UI that serves the generated HTML to end‑users via a static hosting platform.



## Data Flow & Pipelines
Author edits Markdown in the Content Layer → Commit → CI pipeline in Build Layer renders Markdown to HTML → Artifacts are pushed to the Presentation Layer repository branch (e.g., gh‑pages) → Static host serves HTML to visitors.

## Key Design Decisions
- Use Markdown for human‑readable documentation and easy versioning
- Leverage GitHub Actions for automated build and deployment
- Host on GitHub Pages to provide free, globally distributed CDN
- Keep architecture monolithic to reduce complexity for a single‑document repository

## Scalability & Reliability
Scalability is achieved by the underlying CDN of GitHub Pages; adding more documents does not affect performance as each page is served as static assets. For larger documentation sets, consider a dedicated static site generator with incremental builds.
