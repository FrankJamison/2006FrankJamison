# 2006 Frank Jamison — Resume / Portfolio Site

A simple, static resume/portfolio website built with plain **HTML + CSS**.

- Single-page layout (About, Work Experience, Education, Contact)
- Downloadable PDF resume
- Responsive layout via media queries
- No build step, no framework

## Demo

- Local preview: open `index.html` or run a tiny static server (see below)
- Production: deploy to any static host (GitHub Pages, Netlify, Vercel, IIS/Apache static folder, S3, etc.)

## Tech

- HTML5
- CSS3
- Google Fonts
- Font Awesome (icons)

## Technical details / skills demonstrated

- Semantic HTML and in-page navigation via anchor links (`#about`, `#work`, `#education`, `#contact`)
- Responsive design using media queries (switches between stacked and two-column layout)
- CSS fundamentals: typography, spacing containers, utility classes, and button/link styling
- Fixed navigation bar and consistent page structure
- Asset management with relative paths (images and a downloadable PDF resume)
- External CDN integrations (Google Fonts, Font Awesome)
- Static-site deployment readiness (no build tooling required)

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

If this workspace includes a VS Code task named **Open in Browser**, you can run:

- `Terminal → Run Task… → Open in Browser`

In this repo, the task is set up to open `index.html` directly in Chrome.

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

## License

No license is currently specified in this repository.