Publishing instructions

This repository contains a small static site for the Reno Outdoor Activities Guide.

Option A — Quick (GitHub Pages from `docs/`)
1. Commit and push this repository to GitHub (preferably `main` branch).
2. The included GitHub Actions workflow will automatically deploy the `docs/` folder to GitHub Pages on push to `main`.
3. After the workflow runs, your site will be available at `https://<your-username>.github.io/<repo-name>/`.

Commands to run locally (PowerShell):

```powershell
git add .
git commit -m "Publish site to docs/ and add GitHub Pages workflow"
git push origin main
```

Option B — Serve locally (quick test)

```powershell
cd 'C:\Users\callm\OneDrive\Documents\GitHub\Reno\docs'
python -m http.server 8000
# open http://localhost:8000/reno_activities.html
```

Notes
- The workflow expects the branch to be named `main`. If you use a different branch name, update `.github/workflows/pages.yml`.
- If you prefer auto-deploy to the `gh-pages` branch or a different setup, I can add that workflow instead.
