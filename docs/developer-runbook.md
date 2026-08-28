# SudeshDahale Repository Developer Runbook

## Prerequisites
- Git installed (minimum version 2.20).
- A text editor or IDE of your choice (VS Code, IntelliJ, etc.).
- Optional: Markdown preview tool or static site generator if you intend to render documentation (e.g., VS Code Markdown preview, MkDocs, Jekyll).

## Environment Variables
| Variable | Status | Description |
| :--- | :--- | :--- |
| `MARKDOWN_PREVIEW_PORT` | Optional | Port used by local Markdown preview servers (e.g., MkDocs). |


## Local Setup & Development
1. 1. Clone the repository:
   ```bash
   git clone https://github.com/SudeshDahale/SudeshDahale.git
   cd SudeshDahale
   ```
2. 2. Verify that the repository contains the expected documentation files (e.g., `README.md`).
3. 3. (Optional) If you plan to render the docs as a static site, install a generator:
4.    - **MkDocs**: `pip install mkdocs` and then run `mkdocs serve`.
   - **Jekyll**: `gem install bundler jekyll` and then `bundle exec jekyll serve`.
   Choose the tool that matches the project’s existing configuration (look for `mkdocs.yml`, `Gemfile`, etc.).
5. 4. Open `README.md` in your editor to start reviewing or editing documentation.
6. 5. (Optional) Configure any IDE extensions for Markdown linting and preview to get live feedback while editing.

## Running Tests
```bash
```bash
# Using markdownlint (install with npm if not present)
npm install -g markdownlint-cli
markdownlint "**/*.md"
```
```

## Troubleshooting
### Markdown preview server fails to start or reports "port already in use".
**Resolution:** Ensure the port is free or set a different port via the `MARKDOWN_PREVIEW_PORT` environment variable, e.g., `export MARKDOWN_PREVIEW_PORT=8081` before running the server.

### Missing static site generator configuration files (e.g., `mkdocs.yml` or `Gemfile`).
**Resolution:** The repository may be intended as raw documentation only. Skip the static site generation step and view files directly in a Markdown viewer.

### markdownlint reports errors you are unfamiliar with.
**Resolution:** Review the rule definitions in the project's `.markdownlint.json` (if present) or refer to the markdownlint documentation: https://github.com/DavidAnson/markdownlint.


