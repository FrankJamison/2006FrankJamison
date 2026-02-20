# FrankJamison.com v2006

2006-era resume/portfolio site as a simple static page (plain HTML + CSS). No build step, no framework.

## Live preview

- https://frankjamison2006.fcjamison.com/

## What’s in here

- Single-page layout (About, Work Experience, Education, Contact)
- Downloadable PDF resume
- Responsive layout via media queries
- External CDNs: Google Fonts + Font Awesome

## Tech stack

- HTML5
- CSS3
- Google Fonts
- Font Awesome (icons)

## Project structure

```text
.
├─ index.html
├─ css/
│  └─ styles.css
├─ images/
│  ├─ frank-jamison.jpg
│  └─ education-background-image.jpg
└─ documents/
   └─ resume-frank-jamison.pdf
```

## Run locally

This is a static site — any static file server works.

### Option A: open the file directly

Double-click `index.html`.

If your browser blocks something due to local file restrictions, use Option B.

### Option B (recommended): run a local static server

From the project folder:

**Python (built-in):**

```bash
python -m http.server 8000
```

Then open:

- http://localhost:8000/

**Node (one-liner):**

```bash
npx serve
```

### Option C: VS Code task

This workspace includes a VS Code task named **Open in Browser**.

- Run it via **Terminal → Run Task… → Open in Browser** (or Command Palette: **Tasks: Run Task**).
- It opens Chrome at `http://frankjamisoncomv2006.localhost/`.
- This assumes you already have a local web server and host mapping configured for that hostname.

If you don’t use that local setup, prefer Option A or B.

## Customize content

### Update text and sections

Edit `index.html`:

- Header name + title
- About paragraph
- Work Experience entries
- Education section
- Footer contact links

### Replace images

Replace files in `images/` (or add new ones) and update references in `index.html` or `css/styles.css`.

Current key assets:

- `images/frank-jamison.jpg` (profile photo)
- `images/education-background-image.jpg` (education section background)

### Update the downloadable resume

Replace `documents/resume-frank-jamison.pdf` with your latest PDF.

Note: the download link in `index.html` points at that exact filename.

### Styling

All styling is in `css/styles.css`.

Key areas:

- Global typography + layout (`body`, `.content-wrap`)
- Navigation bar (`nav`)
- Responsive behavior (media queries at the bottom)

## Deployment

Because this is a static site, deployment is just hosting these files together:

- `index.html`
- `css/`
- `images/`
- `documents/`

### GitHub Pages

1. Push this repo to GitHub.
2. In GitHub: `Settings → Pages`.
3. Set **Source** to `Deploy from a branch`.
4. Select branch `main` (or `master`) and folder `/ (root)`.

After it builds, GitHub will provide a public URL.

### Custom domain (optional)

If you use a custom domain, configure DNS with your host and (for GitHub Pages) add a `CNAME` file.

## Developer notes

- The page uses in-page anchor navigation (`#about`, `#work`, `#education`, `#contact`).
- Asset paths are relative; keep `css/`, `images/`, and `documents/` alongside `index.html` when deploying.
- External dependencies are loaded from CDNs, so local previews require an internet connection.

## License

No license is currently specified in this repository.
