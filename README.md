Publishing instructions

This repository contains a small static site for the Reno Outdoor Activities Guide.

Option A — Quick (GitHub Pages from `docs/`)
1. Commit and push this repository to GitHub (preferably `main` branch).
2. The included GitHub Actions workflow will automatically deploy the `docs/` folder to GitHub Pages on push to `main`.
3. After the workflow runs, your site will be available at `https://<your-username>.github.io/<repo-name>/`.

Commands to run locally (PowerShell):

```powershell
# Outdoor Activities Guide — Reno, Dublin (CA), Lone Pine (CA)

A fast, mobile-first static site that converts CSV datasets into beautiful, filterable activity cards with full contact details and one-tap WhatsApp sharing.

Why you'll love it
- Clean, scannable card UI ideal for mobile and social sharing.
- One-click WhatsApp sharing pre-fills the full activity details (date, location, phone, website, description, season).
- Drop-in data: add new city guides by placing a CSV and a simple HTML page in `docs/`.
- Works offline / via `file://` using the CSV file-input fallback.

Quick links
- Index: [docs/index.html](docs/index.html)
- Reno: [docs/reno_activities.html](docs/reno_activities.html)
- Dublin, CA: [docs/dublin.html](docs/dublin.html)
- Lone Pine, CA: [docs/lonepine.html](docs/lonepine.html)

Local preview
```bash
cd docs
python -m http.server 8000
# open http://localhost:8000
```

Publish (GitHub Pages)
1. Push your repository to GitHub.
2. The repository ships with a Pages workflow that deploys the `docs/` folder. Ensure the workflow has permissions and the Pages source is set appropriately in repository settings.

Notes
- To add another city: create `docs/<city>_outdoor_activities.csv` and `docs/<city>.html` using the existing pages as templates.
- If you want, I can commit and push these files and enable publishing to `gh-pages` for you.

---

If you'd like a shorter tagline or a graphical badge for the README header, tell me the style and I will add it.
