# SudeshDahale/SudeshDahale – Developer Runbook

## Prerequisites
- Git (>=2.30) – for cloning the repository.
- A Markdown viewer or editor (e.g., VS Code, Typora) – to read and edit the documentation.
- If the documentation is intended to be published as a static site, a static‑site generator (e.g., MkDocs, Hugo) may be required – verify the README or accompanying build scripts for the specific tool.

## Local Setup & Development
1. 1. Clone the repository:
   ```sh
   git clone https://github.com/SudeshDahale/SudeshDahale.git
   cd SudeshDahale
   ```
2. 2. Verify the repository contents. The only tracked source file is `README.md`, which houses the project overview and usage instructions.
3. 3. If a static‑site generator is referenced in the `README.md`, install it globally or inside a virtual environment. Example for MkDocs:
   ```sh
   pip install mkdocs
   ```
4. 4. Build / preview the documentation (only needed when a generator is used). Example for MkDocs:
   ```sh
   mkdocs serve   # launches a local server at http://127.0.0.1:8000
   ```
5. 5. Edit `README.md` (or other markdown files) using your preferred editor. Changes can be previewed live if a generator server is running.

## Running Tests
```bash
No automated tests are present in the repository. Validation is performed manually by reviewing the rendered documentation (e.g., via a Markdown preview or a static‑site generator).
```

## Troubleshooting
### `git clone` fails with authentication errors.
**Resolution:** Ensure you have proper access rights to the repository. Use an SSH key or a personal access token for HTTPS cloning if the repository is private.

### Markdown preview shows garbled formatting or missing images.
**Resolution:** Check that all referenced assets (images, links) are present in the repository and that relative paths are correct.

### Running `mkdocs serve` (or another generator) aborts with "module not found" errors.
**Resolution:** Install the required generator as documented in the README. Use a virtual environment to avoid version conflicts:
   ```sh
   python -m venv .venv
   source .venv/bin/activate
   pip install mkdocs   # or the appropriate package
   ```


