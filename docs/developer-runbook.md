# SudeshDahale Repository Developer Runbook

## Prerequisites
- Git installed (version 2.20+)
- A text editor or IDE (e.g., VS Code, Atom, Sublime Text)
- Markdown preview tool (optional, e.g., VS Code Markdown preview or a web browser)

## Local Setup & Development
1. 1. Clone the repository:
2.    ```bash
3.    git clone https://github.com/SudeshDahale/SudeshDahale.git
4.    cd SudeshDahale
5.    ```
6. 
7. 2. Verify the repository contents:
8.    ```bash
9.    ls -R
10.    # You should see at least a README.md file
11.    ```
12. 
13. 3. (Optional) Install a Markdown preview extension for your editor or install a static site generator if you intend to render the documentation as a site:
14.    - VS Code: Install the "Markdown All in One" extension.
15.    - MkDocs (Python):
16.      ```bash
17.      pip install mkdocs
18.      mkdocs serve
19.      ```
20.    - Docsify (Node):
21.      ```bash
22.      npm install -g docsify-cli
23.      docsify serve .
24.      ```
25. 
26. 4. Edit the documentation:
27.    - Open `README.md` (or any other `.md` files) in your editor.
28.    - Make changes, save, and preview using your chosen markdown preview method.
29. 
30. 5. Commit and push changes:
31.    ```bash
32.    git add .
33.    git commit -m "Your descriptive commit message"
34.    git push origin main
35.    ```

## Running Tests
```bash

```

## Troubleshooting
### Markdown preview does not render correctly in the editor.
**Resolution:** Ensure you have a markdown preview extension installed (e.g., "Markdown All in One" for VS Code) and that the file has a `.md` extension.

### Running `mkdocs serve` or `docsify serve` fails with a "command not found" error.
**Resolution:** Install the required tool globally: `pip install mkdocs` for MkDocs or `npm install -g docsify-cli` for Docsify. Verify installation with `mkdocs --version` or `docsify --version`.

### Git push is rejected due to permission errors.
**Resolution:** Check that you have write access to the repository. If using SSH, ensure your SSH key is added to your GitHub account. If using HTTPS, verify your username/password or token.


