# SudeshDahale Repository – Developer Runbook

## Prerequisites
- Git client (>=2.20)
- Node.js (optional, if you plan to run a local static site server like `serve` or `http-server`)
- A Markdown viewer/editor (VS Code, typora, etc.)

## Local Setup & Development
1. 1. Clone the repository:
   ```bash
   git clone https://github.com/SudeshDahale/SudeshDahale.git
   cd SudeshDahale
   ```
2. 2. Verify that the repository contains the documentation files (e.g., `README.md`).
3. 3. (Optional) If you want to preview the markdown as a static site, you can use a simple HTTP server:
   ```bash
   # Using Node's http-server (install globally if not present)
   npm install -g http-server
   http-server . -p 8080
   ```
   Then open `http://localhost:8080/README.md` in a browser.
   
4. 4. (Optional) For a richer preview, you may install a Markdown preview extension in VS Code or use tools like `markdown-it`.
   ```bash
   # Example using markdown-it-cli
   npm install -g markdown-it-cli
   markdown-it README.md -o index.html
   open index.html
   ```

## Running Tests
```bash

```

## Troubleshooting
### Unable to locate `README.md` after cloning.
**Resolution:** Ensure the clone completed successfully. Run `git status` to verify files. If the repository is empty, check the remote branch and pull the correct branch (`git checkout main`).

### Markdown preview shows raw markdown instead of formatted HTML.
**Resolution:** Use a proper Markdown preview tool or serve the file through a static site generator. In VS Code, press `Ctrl+Shift+V` to open the preview pane.

### `http-server` command not found.
**Resolution:** Install it globally with `npm install -g http-server` or use any other simple HTTP server (e.g., Python’s `python -m http.server`).


