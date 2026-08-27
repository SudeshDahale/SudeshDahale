# SudeshDahale/SudeshDahale Developer Runbook

## Prerequisites
- Git installed (for cloning the repository).
- A Markdown editor or viewer (e.g., Visual Studio Code, Typora, or any IDE with Markdown preview support).
- Optional: A local static site preview tool if you wish to view the documentation as a rendered site (e.g., `markdown-preview`, `MkDocs`, or a simple HTTP server).

## Local Setup & Development
1. 1. Clone the repository:
2.    ```bash
3.    git clone https://github.com/SudeshDahale/SudeshDahale.git
4.    cd SudeshDahale
5.    ```
6. 2. Verify that the repository contains the main documentation file:
7.    ```bash
8.    ls -1
9.    # Expected output includes:
10.    # README.md
11.    ```
12. 3. Open `README.md` in your preferred Markdown editor or IDE.
13. 4. (Optional) If you want to preview the rendered Markdown locally:
14.    - Using VS Code: open the file and press `Ctrl+Shift+V` to open the Markdown preview.
15.    - Using a simple HTTP server (Python example):
16.      ```bash
17.      python -m http.server 8000
18.      # Then navigate to http://localhost:8000/README.md in your browser.
19.      ```
20.    - Using `markdown-preview` (if installed):
21.      ```bash
22.      markdown-preview README.md
23.      ```

## Running Tests
```bash

```

## Troubleshooting
### Markdown preview does not render correctly or shows raw Markdown syntax.
**Resolution:** Ensure you are using a proper Markdown preview tool or extension. In VS Code, confirm that the Markdown preview is open (`Ctrl+Shift+V`). If using a command‑line previewer, verify it is installed and invoked correctly.

### Changes to `README.md` are not reflected in the preview.
**Resolution:** Refresh the preview window or restart the preview tool. Some editors cache the view; a manual refresh (usually `Ctrl+R` or the refresh button) forces a re‑render.

### `git clone` fails with authentication errors.
**Resolution:** Check that you have proper network access and, if the repository is private, configure SSH keys or personal access tokens as described in GitHub's documentation.


