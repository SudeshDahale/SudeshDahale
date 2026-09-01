# SudeshDahale Repository Developer Runbook

## Prerequisites
- Git installed (version 2.20+ recommended)
- A markdown viewer or editor (e.g., Visual Studio Code, Typora, or any IDE with markdown preview capability)
- Internet connection for cloning the repository

## Local Setup & Development
1. 1. Clone the repository:
2.    ```sh
3.    git clone https://github.com/SudeshDahale/SudeshDahale.git
4.    ```
5. 
6. 2. Navigate into the project directory:
7.    ```sh
8.    cd SudeshDahale
9.    ```
10. 
11. 3. Verify that the `README.md` file is present at the repository root. This file contains the primary project documentation and overview.
12. 
13. 4. Open `README.md` in your preferred markdown viewer or IDE to read the documentation:
14.    - VS Code: `code README.md`
15.    - Command‑line preview (optional, using `grip`):
16.      ```sh
17.      pip install grip   # if you have Python/pip installed
18.      grip README.md
19.      ```
20. 
21. 5. (Optional) If you want a live‑reload preview, you can use a simple HTTP server:
22.    ```sh
23.    npx serve .   # requires Node.js; serves the current directory
24.    ```
25.    Then open `http://localhost:5000/README.md` in a browser.

## Running Tests
```bash

```

## Troubleshooting
### `git clone` fails with authentication or network errors.
**Resolution:** Verify that you have internet access and that the repository URL is correct. If the repository is private, ensure you have the necessary SSH keys or personal access token configured.

### `README.md` is missing after cloning.
**Resolution:** Make sure the clone completed successfully. Run `git status` to check for any incomplete checkout, or re‑clone the repository.

### Markdown does not render correctly in your editor.
**Resolution:** Install a markdown extension/plugin for your editor (e.g., "Markdown All in One" for VS Code) or use an external viewer such as `grip` or a web‑based markdown preview tool.


