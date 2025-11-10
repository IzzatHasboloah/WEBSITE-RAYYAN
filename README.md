# Rayyan Aisy Production — Static Site

Single-page site with fixed golden background for Home and Showreel. When you scroll to **Showreel**, a blur layer fades in over the *same* background. **Services** and **Contact** use a vertically looping SVG background.

## Structure
```
/
├─ index.html
├─ assets/
│  ├─ A_promotional_digital_graphic_for_Rayyan_Aisy_Prod.png   (homepage background)
│  └─ services-contact-loop.svg                                 (seamless tile for Services/Contact)
├─ _redirects   (for Netlify SPA routing; optional for GitHub Pages)
└─ .gitignore
```

## Deploy to GitHub Pages (no terminal)
1. Create a new repo on GitHub (e.g. `rayyan-aisy-site`).
2. Click **Add file → Upload files**.
3. Drag & drop **all files** from this folder (or upload the zip contents) — make sure `index.html` is at the repo root and `assets/` is uploaded.
4. Commit the changes.
5. Go to **Settings → Pages**.
   - **Source:** `Deploy from a branch`
   - **Branch:** `main` (or `master`) and **/ (root)**, then **Save**.
6. Wait 1–2 minutes -> Your site will be live at:  
   `https://<your-username>.github.io/<repo-name>/`

### Custom domain (optional)
- In **Settings → Pages**, add your domain (e.g. `www.rayyanaisyproduction.com`).
- Create a `CNAME` record at your DNS pointing to `<your-username>.github.io`.
- Add a `CNAME` file in the repo root containing your domain name.

## Deploy with Git (terminal)
```bash
git init
git add .
git commit -m "Initial commit: Rayyan Aisy site"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```
Then enable GitHub Pages as above.

## Netlify (optional)
- Drag-and-drop this folder to https://app.netlify.com/drop or connect your repo.
- `_redirects` is already included for SPA-friendly routing.

## Editing
- All styling and JS are inline in `index.html` for simplicity.
- Replace content in **Services** grid or edit backgrounds in `/assets`.
