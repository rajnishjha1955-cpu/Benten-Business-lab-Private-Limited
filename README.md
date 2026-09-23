# Benten Business Lab — Website

Self-contained static site. Logo, founder photo, styles and scripts are all embedded in `index.html`; no build step.

## Publish on GitHub Pages
1. Create a new repository on GitHub (e.g. `benten-website`), Public.
2. Click **Add file → Upload files**, drag in every file from this folder (`index.html`, `404.html`, `.nojekyll`, `robots.txt`, `README.md`), then **Commit changes**.
   - `.nojekyll` is a hidden file; if your computer hides it, it's optional — the site works without it.
3. Go to **Settings → Pages**. Under *Build and deployment*, set Source = **Deploy from a branch**, Branch = **main**, Folder = **/ (root)**. Save.
4. After ~1 minute the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Custom domain (optional, e.g. benten.co.in)
1. In **Settings → Pages → Custom domain**, enter `benten.co.in` and save (GitHub creates a `CNAME` file).
2. At your domain registrar add DNS records:
   - `A` records for `@` → 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
   - `CNAME` for `www` → `<your-username>.github.io`
3. Tick **Enforce HTTPS** once available.

## Contact form
Submitting the form opens the visitor's email app with the enquiry pre-filled to info@benten.co.in.
