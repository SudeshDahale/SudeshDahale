# SudeshDahale Repository – Developer Runbook

## Prerequisites
- Git
- Node.js (optional, for live Markdown preview tools like `markdown-it` or `vitepress`)
- A Markdown viewer/editor (e.g., VS Code with Markdown extensions)

## Local Setup & Development
1. 1. **Clone the repository**
   ```bash
   git clone https://github.com/SudeshDahale/SudeshDahale.git
   cd SudeshDahale
   ```
2. 2. **(Optional) Install a local Markdown preview server**
   If you want a live‑reload preview, install one of the following tools globally:
3.    - **VitePress**
     ```bash
     npm i -g vitepress
     ```
   - **Docsify**
     ```bash
     npm i -g docsify-cli
     ```
   - **markdown-it-cli**
     ```bash
     npm i -g markdown-it-cli
     ```
4. 3. **Start the preview server**
   Choose the tool you installed:
5.    - VitePress:
     ```bash
     vitepress dev .
     ```
   - Docsify:
     ```bash
     docsify serve .
     ```
   - markdown-it-cli:
     ```bash
     markdown-it -w -o index.html README.md && live-server .
     ```
6. 4. **Open the site**
   Navigate to `http://localhost:3000` (or the port shown by the tool) to view the rendered Markdown documentation.

## Running Tests
```bash

```

## Troubleshooting
### Markdown preview does not update after saving changes.
**Resolution:** Ensure the preview tool is running with a watch flag (`-w` for markdown-it-cli) or use a tool that supports hot‑reload like VitePress. Restart the server if needed.

### Command `vitepress`/`docsify` not found.
**Resolution:** Make sure Node.js is installed and the tool was installed globally (`npm i -g <tool>`). Verify with `node -v` and `npm -v`.

### Port conflict when starting the preview server.
**Resolution:** Stop any process using the default port (3000) or start the server on a different port, e.g., `vitepress dev . --port 4000`.


