# SudeshDahale/SudeshDahale Repository – Developer Runbook

## Prerequisites
- Git installed (>=2.20) for cloning the repository.
- A text editor or IDE (e.g., VS Code, Sublime Text, Vim).
- Optional: A Markdown preview tool or static‑site generator (e.g., VS Code Markdown Preview, MkDocs, Jekyll) if you want to render the README as a site.

## Local Setup & Development
1. 1. Clone the repository:
2.    ```bash
3.    git clone https://github.com/SudeshDahale/SudeshDahale.git
4.    cd SudeshDahale
5.    ```
6. 2. Open the project folder in your preferred editor.
7. 3. Edit `README.md` as needed. The file is plain Markdown; no build step is required for simple edits.
8. 4. (Optional) If you want to preview the Markdown as a static site:
9.    - **VS Code**: Open `README.md` and press `Ctrl+Shift+V` (or `Cmd+Shift+V` on macOS) to view the preview.
10.    - **MkDocs** (if you prefer a local site):
11.      ```bash
12.      pip install mkdocs
13.      mkdocs serve
14.      ```
15.      This will serve the `docs/` folder (create one if you want) at `http://127.0.0.1:8000`.
16.    - **Jekyll** (GitHub Pages style):
17.      ```bash
18.      gem install bundler jekyll
19.      jekyll new . --force
20.      bundle exec jekyll serve
21.      ```
22.      The `README.md` can be renamed to `index.md` inside the Jekyll site structure to render.
23. 5. Commit and push changes:
24.    ```bash
25.    git add README.md
26.    git commit -m "Update profile documentation"
27.    git push origin main
28.    ```

## Running Tests
```bash
There are no automated tests for this repository. Validation is limited to visual inspection of the rendered Markdown (see step 4).
```

## Troubleshooting
### Markdown preview does not render correctly in VS Code.
**Resolution:** Ensure the built‑in Markdown preview is enabled (`Ctrl+Shift+P` → `Markdown: Open Preview`). If extensions interfere, disable them temporarily.

### MkDocs or Jekyll commands fail with `ModuleNotFoundError` or `GemNotFound`.
**Resolution:** Install the missing dependencies: `pip install mkdocs` for MkDocs, or `gem install bundler jekyll` for Jekyll. Verify your Python or Ruby environment is correctly set up.

### Git push is rejected due to permission errors.
**Resolution:** Check that you have write access to the repository. Use SSH keys or a personal access token for HTTPS authentication.


