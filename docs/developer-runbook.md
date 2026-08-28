# SudeshDahale Repository – Developer Runbook

## Prerequisites
- Git client (e.g., git)
- A text editor or IDE capable of editing Markdown (e.g., VS Code, Atom, Sublime Text)
- Markdown preview tool (many editors have built‑in preview, or use a simple static site previewer like `markdown-preview` or a browser extension)
- Optional: If the repository uses a static site generator (e.g., Jekyll, Hugo, MkDocs) – install the corresponding tool as described in the README

## Local Setup & Development
1. 1. Clone the repository:
2.    ```
3.    git clone https://github.com/SudeshDahale/SudeshDahale.git
4.    cd SudeshDahale
5.    ```
6. 2. Review the `README.md` for any repository‑specific instructions. The README is the primary source of usage guidance for this documentation‑only project.
7. 3. If a static‑site generator is referenced in the README (e.g., Jekyll, Hugo, MkDocs), install it following the official installation guide:
8.    - **Jekyll**: `gem install jekyll bundler`
9.    - **Hugo**: download the binary from https://gohugo.io/getting-started/install/
10.    - **MkDocs**: `pip install mkdocs`
11.    *If no generator is mentioned, you can work directly with the raw Markdown files.*
12. 4. (Optional) Install any listed development dependencies with the appropriate package manager:
13.    - npm/yarn for JavaScript‑based tooling
14.    - pip for Python‑based tooling
15.    - gem for Ruby‑based tooling
16.    *Only required if the README specifies a `package.json`, `requirements.txt`, or `Gemfile`.*

## Running Tests
```bash
No automated tests are detected in this repository. Validation is performed manually via the Markdown preview or static‑site generator preview described above.
```

## Troubleshooting
### Preview does not render or shows raw Markdown.
**Resolution:** Ensure you are using the correct preview method. If a static‑site generator is required, verify it is installed and run the appropriate `serve` command (e.g., `bundle exec jekyll serve`).

### `bundle exec jekyll serve` fails with missing gems.
**Resolution:** Run `bundle install` to install the gems listed in `Gemfile`. If no `Gemfile` exists, install Jekyll globally with `gem install jekyll bundler`.

### Command `hugo` not found.
**Resolution:** Install Hugo following the official guide (download binary, place it in your PATH, or use a package manager such as Homebrew: `brew install hugo`).

### Markdown preview in editor shows broken links or missing images.
**Resolution:** Check that the referenced files exist relative to the Markdown file. Use relative paths (`../images/pic.png`) and verify case‑sensitivity on case‑sensitive file systems.


