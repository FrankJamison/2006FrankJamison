# 2006-FrankJamison (Portfolio)

Static portfolio site for the **2006 Frank Jamison** project.

## Project Structure

- `index.html` — main page
- `css/` — stylesheets
  - `css/styles.css` — site styles
- `images/` — image assets
- `documents/` — downloadable documents/assets

## Preview / Run

This project is plain HTML/CSS (no build step).

### Option A: Open the file directly

You can double-click `index.html` to open it in your browser.

Note: some browsers enforce restrictions when opening local files (for example, certain font or fetch requests). If you run into anything like that, use a local server (Option B).

### Option B: Serve with any local web server (recommended)

From this project folder, start a static server and open the URL it prints.

Examples:

- Python: `python -m http.server`
- Node: `npx serve`

Typical URLs look like `http://localhost:8000/` or `http://localhost:3000/`.

### Option C: Use the VS Code task (if available)

This workspace may include a VS Code task named **Open in Browser**. If it exists, you can run it to launch the site using your local setup.

## Editing Content

- HTML structure and content live in `index.html`.
- Styles are in `css/styles.css`.
- Add or replace images in `images/` and reference them from HTML/CSS using relative paths.
- Add PDFs or other downloads in `documents/` and link them from `index.html`.

## Deployment

Because everything is static, deployment is just copying files to a web host.

- Upload `index.html`, `css/`, `images/`, and `documents/` to the same folder on your server.
- Keep paths relative (e.g., `css/styles.css`, `images/...`) so the site works when hosted at different URLs.
- If you host under a subfolder (not the domain root), relative links will typically still work as long as you keep the same folder structure.
