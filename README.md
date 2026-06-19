# rakshpradhan.github.io
# Rakshit Pradhan — Personal Website

Minimal single-page site (`index.html`) in the Newsreader serif style. Dark theme by default with a light/dark toggle. No build step.

## Files (upload ALL of these to the repo root)
- `index.html` — the site
- `Rakshit_Pradhan_Resume.pdf` — linked from the "Résumé" link in the top-right
- `.nojekyll` — tells GitHub Pages to serve files as-is

> The résumé link is relative (`Rakshit_Pradhan_Resume.pdf`), so the PDF must sit next to `index.html` in the repo. To swap in an updated résumé later, just replace that file (keep the same name) or update the `href` in `index.html`.

## Deploy to GitHub Pages

### Option A — user site (`https://Rakshit-p.github.io`)
1. Create a public repo named exactly `Rakshit-p.github.io`.
2. Upload `index.html`, `Rakshit_Pradhan_Resume.pdf`, and `.nojekyll` to the repo root.
3. **Settings → Pages → Source: Deploy from a branch**, branch `main`, folder `/ (root)`, **Save**.
4. Live in ~1 min at `https://Rakshit-p.github.io`.

### Command line
```bash
git init
git add index.html Rakshit_Pradhan_Resume.pdf .nojekyll
git commit -m "Personal site"
git branch -M main
git remote add origin https://github.com/Rakshit-p/Rakshit-p.github.io.git
git push -u origin main
```
Then enable Pages under Settings → Pages.

## Notes
- **Theme:** starts dark; the sun/moon button toggles it and remembers the choice in the browser.
- **Editing:** all HTML/CSS/JS is in `index.html`. Theme colors live in the `[data-theme="dark"]` and `[data-theme="light"]` blocks near the top.
