# Technical Architecture Guide for SudeshDahale Documentation Repository

## System Overview
The SudeshDahale repository is a monolithic collection of static documentation written in Markdown. The sole artifact observed is `README.md`, which serves as the primary entry point for the project's documentation. All documentation assets reside within the same repository, adhering to a single-tier architecture where content, build, and delivery are tightly coupled in a static site model.

## System Layers
### Content Layer
**Technologies:** Markdown

All documentation is authored in plain Markdown files. The repository currently contains `README.md` as the main document, and any additional Markdown files would be stored alongside it.

### Build/Transformation Layer
If a build pipeline is employed, a static site generator (e.g., Jekyll, Hugo, or MkDocs) would consume the Markdown source and produce HTML assets. The repository does not include explicit configuration for a generator, so this layer is optional and can be added without altering the core architecture.

### Delivery Layer
The final HTML (or raw Markdown) is served to consumers via a static hosting platform such as GitHub Pages. Because the site is static, the delivery layer requires no server‑side logic.



## Data Flow & Pipelines
Author -> Git Repo (Markdown) -> Optional CI/Static Site Generator -> Static Hosting (GitHub Pages) -> End User

## Key Design Decisions
- Use of Markdown as the sole authoring format – ensures low barrier to contribution and platform‑agnostic content.
- Monolithic repository layout – all documentation lives in a single repo, simplifying versioning and traceability.
- Static site approach – eliminates runtime dependencies, enabling inexpensive, highly performant hosting.

## Scalability & Reliability
Static documentation scales effortlessly: the content is served from a CDN (e.g., GitHub Pages) which can handle arbitrarily high request volumes with minimal latency. Adding new documents does not change the architecture; it merely increases the size of the static asset bundle. If the documentation set grows substantially, the optional Build Layer can be extended with a static site generator that supports incremental builds, keeping build times low.
