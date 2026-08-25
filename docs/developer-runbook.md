# SudeshDahale Repository – Developer Runbook

## Prerequisites
- Git installed (version 2.20+)
- A text editor or IDE (VS Code, Sublime, etc.)

## Local Setup & Development
1. 1. Clone the repository:
2.    ```
3.    git clone https://github.com/SudeshDahale/SudeshDahale.git
4.    cd SudeshDahale
5.    ```
6. 2. Review the top‑level documentation:
7.    - Open `README.md` in your editor or render it with a markdown viewer.
8.    - The README contains the project overview, usage instructions, and any additional guidance.
9. 3. (Optional) If you intend to publish the static site:
10.    - Ensure you have a static‑site server (e.g., Python’s built‑in HTTP server) to preview HTML files.
11.    - Example:
12.      ```
13.      python -m http.server 8000
14.      # Then open http://localhost:8000 in a browser
15.      ```

## Running Tests
```bash

```

## Troubleshooting
### Unable to locate the repository after cloning.
**Resolution:** Verify the clone URL and ensure you have internet connectivity. Run `git status` inside the cloned directory to confirm the repository was created.

### Markdown rendering looks broken in the editor.
**Resolution:** Install a markdown preview extension (e.g., "Markdown Preview" for VS Code) or use an external viewer such as `grip` (`pip install grip`).

### Static site preview shows a 404 or blank page.
**Resolution:** Make sure you are serving the correct directory (the root of the repository) and that the server is pointed to the folder containing the HTML files.


