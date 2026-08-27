# SudeshDahale Repository – Developer Runbook

## Prerequisites
- Git (v2.20+)
- A text editor or IDE (VS Code, Sublime Text, etc.)
- Markdown preview capability (built‑in in many editors or a simple static site preview tool like `markdown-preview`)

## Local Setup & Development
1. 1. **Clone the repository**
   ```bash
   git clone https://github.com/SudeshDahale/SudeshDahale.git
   cd SudeshDahale
   ```
2. 2. **Review the documentation**
   Open `README.md` in your editor or run a markdown preview to see the project overview, usage instructions, and other docs.
3. 3. **(Optional) Install a markdown preview tool**
   If your editor does not provide live preview, you can install a lightweight preview server:
   ```bash
   # Example using npm (requires Node.js) – only if you want a local web preview
   npm install -g markdown-preview
   markdown-preview README.md
   ```
   This will serve the rendered markdown at `http://localhost:8080`.
4. 4. **Make changes**
   Edit the documentation files (`*.md`) as needed. Commit and push following the usual Git workflow.
5. 5. **Validate Markdown syntax** (optional)
   ```bash
   # Using markdownlint (requires Node.js)
   npm install -g markdownlint-cli
   markdownlint "*.md"
   ```

## Running Tests
```bash

```

## Troubleshooting
### Markdown preview does not render correctly or shows raw markdown.
**Resolution:** Ensure the preview tool you are using supports GitHub‑flavored Markdown. If using `markdown-preview`, verify that Node.js is installed and that the tool is up‑to‑date (`npm update -g markdown-preview`).

### `npm: command not found` when trying to install a preview tool.
**Resolution:** Install Node.js (v14 or later) from https://nodejs.org and ensure the `npm` command is in your PATH.

### Git clone fails with authentication errors.
**Resolution:** Check that you have access to the repository. Use an SSH key or personal access token for private repos.


