# Technical Architecture Guide – SudeshDahale Personal Profile Repository

## System Overview
The SudeshDahale repository is a monolithic static site built entirely from Markdown source files. Its sole module is the Documentation module, represented by the top‑level `README.md`. The site is rendered as HTML (typically via GitHub Pages or a similar static‑site host) and delivered directly to end‑users without any server‑side processing. This guide describes the layers, data flow, design decisions, and scalability considerations of this lightweight architecture.

## System Layers
### Content Layer
**Technologies:** Markdown

All content is authored in plain Markdown files stored in the repository. The primary artifact is `README.md`, which contains personal profile information, project listings, and other documentation. This layer is version‑controlled by Git, providing history, branching, and collaboration capabilities.

### Build/Rendering Layer
**Technologies:** GitHub Pages (built‑in Jekyll renderer) or any Markdown‑to‑HTML static site generator

When the repository is built (e.g., by GitHub Pages or a local static‑site generator), the Markdown source is transformed into static HTML, CSS, and optional assets. No dynamic runtime code is introduced; the transformation is a pure compile‑time step.

### Hosting & Delivery Layer
**Technologies:** CDN (GitHub Pages CDN, Cloudflare, etc.), HTTPS

The generated static assets are served from a content‑delivery network (CDN) or static‑file host (GitHub Pages, Netlify, etc.). Because the site consists only of static files, the hosting layer can scale automatically without any server provisioning.



## Data Flow & Pipelines
1️⃣ **Authoring** – A contributor edits `README.md` (or adds new Markdown files) in the Git repository. 2️⃣ **Commit & Push** – Git records the change and pushes it to the remote origin. 3️⃣ **Build Trigger** – The hosting platform detects the push and runs a static‑site build step, converting Markdown to HTML. 4️⃣ **Artifact Publication** – The resulting static files are uploaded to the CDN. 5️⃣ **User Access** – End users request the site URL; the CDN serves the pre‑rendered HTML/CSS instantly, with no server‑side logic.

## Key Design Decisions
- Use of Markdown as the sole content format – ensures simplicity, readability, and easy editing for non‑technical contributors.
- Monolithic static site approach – eliminates runtime dependencies, reduces attack surface, and lowers operational overhead.
- Leverage Git‑based hosting (e.g., GitHub Pages) – provides built‑in CI for static site generation and automatic HTTPS.
- Single‑file documentation model – the entire site lives in `README.md`, keeping the repository small and focused.

## Scalability & Reliability
Because the architecture is static, scalability is achieved automatically by the underlying CDN. Adding more Markdown pages only increases the build time linearly and the storage footprint marginally. The site can handle any amount of traffic without additional configuration, as each request is served from edge caches. If the documentation set grows substantially, a static‑site generator can be introduced to split content into multiple files while preserving the same delivery model.
