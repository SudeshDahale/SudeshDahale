# SudeshDahale/SudeshDahale – Developer Runbook

## Prerequisites
- Git installed (>=2.20)
- A text editor or IDE capable of rendering Markdown (e.g., VS Code, GitHub Desktop, Typora)
- Optional: A local HTTP server to preview Markdown (e.g., `python -m http.server` or VS Code Live Server extension)

## Local Setup & Development
1. 1. **Clone the repository**
   ```bash
   git clone https://github.com/SudeshDahale/SudeshDahale.git
   cd SudeshDahale
   ```
2. 2. **Verify repository contents**
   The project consists of a single documentation file:
   - `README.md` – the primary source of project overview and usage instructions.
3. 3. **Open the documentation**
   - Use any Markdown viewer/editor to read the file locally, e.g.: 
     ```bash
     code README.md            # VS Code
     typora README.md          # Typora
     ```
4. 4. **(Optional) Preview via a local web server**
   If you prefer a rendered HTML view in a browser, you can start a simple HTTP server:
   ```bash
   # Python 3
   python -m http.server 8000
   # Then open http://localhost:8000/README.md in your browser
   ```

## Running Tests
```bash
No automated tests are defined for this documentation‑only repository.
```

## Troubleshooting
### README.md does not render correctly in the editor.
**Resolution:** Ensure the editor’s Markdown preview feature is enabled or install a dedicated Markdown preview extension (e.g., VS Code’s built‑in Markdown preview: `Ctrl+Shift+V`).

### Git clone fails with authentication errors.
**Resolution:** Verify you have access to the public repository or configure SSH keys if using the SSH URL.

### Local HTTP server shows a directory listing instead of rendered Markdown.
**Resolution:** Use a Markdown‑aware server or open the raw `README.md` in a browser‑based viewer (e.g., `markdown-preview` extension) rather than a plain file server.


