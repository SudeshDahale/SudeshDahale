# SudeshDahale/SudeshDahale Developer Runbook

## Prerequisites
- Git installed (https://git-scm.com/)
- A text editor or IDE for editing Markdown files (e.g., VS Code, Atom, Sublime Text)
- Optional: A Markdown preview tool or static site generator if you wish to view rendered documentation locally

## Local Setup & Development
1. 1. Clone the repository:
2.    ```
3.    git clone https://github.com/SudeshDahale/SudeshDahale.git
4.    ```
5. 2. Navigate into the repository directory:
6.    ```
7.    cd SudeshDahale
8.    ```
9. 3. Verify that the documentation files are present (e.g., `README.md`).
10. 4. Open the Markdown files in your preferred editor to begin editing.
11. 5. (Optional) If you want to view the rendered documentation locally, you can:
12.    - Use the built‑in Markdown preview in VS Code (View → Open Preview).
13.    - Run a lightweight local server such as `python -m http.server` in the repo root and open the files in a browser.
14.    - If the project later adopts a static‑site generator (e.g., MkDocs, Jekyll), follow its specific build instructions.

## Running Tests
```bash

```

## Troubleshooting
### Markdown preview does not render correctly.
**Resolution:** Ensure you are using a Markdown‑aware viewer. In VS Code, open the file and press `Ctrl+Shift+V` (Windows/Linux) or `Cmd+Shift+V` (macOS) to open the preview.

### Changes to `README.md` are not reflected when viewing via a local web server.
**Resolution:** Refresh the browser page after saving the file. If using a static‑site generator, make sure you have re‑run the build command.

### Git clone fails with authentication errors.
**Resolution:** Verify that you have access to the repository and that your SSH keys or HTTPS credentials are correctly configured.


