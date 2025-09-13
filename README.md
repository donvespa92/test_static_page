
# Static site starter

This is a minimal static website to get you started. It contains:
- `index.html` — the main page
- `styles.css` — simple, modern styling
- `README.md` — this file

## View locally
Open `index.html` directly in your browser, or run a tiny HTTP server and visit `http://localhost:8000`:

```bash
python3 -m http.server 8000
# then open http://localhost:8000 in your browser
```

## Publish on GitHub Pages (two simple ways)

### Option A — User/organization site (URL: `https://USERNAME.github.io/`)
1. Create a GitHub repository named `USERNAME.github.io` (replace `USERNAME` with your GitHub username).
2. Push the files to the repository (example commands below).
3. GitHub Pages will serve the site at `https://USERNAME.github.io/` once publishing is enabled in the repo settings.

### Option B — Project site (URL: `https://USERNAME.github.io/REPO/`)
1. Create any GitHub repository and push the files.
2. On the repository page, go to **Settings → Pages** and select **Branch: main** and folder **/ (root)**.
3. The site URL will be shown in the Pages section (it often appears as `https://USERNAME.github.io/REPO/`).

### Example git commands (run locally; replace `USERNAME` and `REPO`):
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/USERNAME/REPO.git
git push -u origin main
```

> If you create a repo named `USERNAME.github.io`, you can use `REPO` = `USERNAME.github.io` and get the root URL `https://USERNAME.github.io/`

## Publish with Netlify (quick, no git required)
1. Go to https://app.netlify.com/ and sign up or log in.
2. From the dashboard choose **Sites → Add new site → Deploy manually → Drag and drop** and drop the ZIP file or the extracted folder.
3. Netlify will give you a public link you can rename later.

## Custom domain (optional)
- You can point a domain you own to GitHub Pages or Netlify. For GitHub Pages, add a `CNAME` file with your domain name; update DNS (A records or CNAME) at your domain registrar. Follow the host's docs for exact DNS records.

## Next steps / extensions
- Add more pages (`about.html`, `projects.html`) and link them from `index.html`.
- Add images in a folder `images/` and reference them.
- Use a static site generator (e.g., Jekyll, Hugo, MkDocs) later when you want templates and many pages.
- If you want Python-based static generation, try MkDocs or Pelican.

---
If you tell me which hosting option you prefer (GitHub Pages or Netlify), I will give the exact commands/steps to publish and which fields to click in the UI.
