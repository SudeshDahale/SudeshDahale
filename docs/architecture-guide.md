# Technical Architecture Guide for SudeshDahale Repository

## System Overview
The SudeshDahale repository is a static documentation collection. It consists primarily of a README.md file that provides project description, usage, and other information. The architecture is simple and static, relying on version‑controlled markdown files rendered by GitHub or any static site generator.

## System Layers
### Source Control Layer
**Technologies:** Git

Git repository hosting the markdown files and any ancillary documentation assets.

### Documentation Storage Layer
**Technologies:** Markdown

Raw markdown files stored in the repository, serving as the single source of truth for project information.

### Presentation Layer
**Technologies:** GitHub UI, Jekyll, Hugo

GitHub's web UI or a static site generator (e.g., Jekyll, Hugo) renders the markdown into HTML for end‑users.



## Data Flow & Pipelines
When a contributor updates README.md, the change is committed to the Git repository. The Git hosting platform detects the push, stores the new version, and automatically renders the markdown to HTML for browser consumption. If a static site generator is employed, a build step reads the markdown files, transforms them into static HTML pages, and publishes them to a web server or GitHub Pages.

## Key Design Decisions
- Store documentation as plain markdown to keep it lightweight and versionable
- Rely on GitHub's built‑in markdown rendering to avoid additional infrastructure
- If richer styling is needed, optionally integrate a static site generator like Jekyll
- Keep all documentation in a single repository to simplify access and collaboration

## Scalability & Reliability
The static nature of the repository scales naturally: adding more markdown files does not affect performance of rendering on GitHub. For large documentation sets, a static site generator can pre‑render pages, and hosting on a CDN (e.g., GitHub Pages) provides global distribution with negligible cost.
