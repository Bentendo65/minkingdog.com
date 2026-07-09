# Minky The Housewolfe — GitHub Pages Site

This folder is a GitHub Pages-ready static version of the saved GoDaddy Airo preview.

## Upload to GitHub

1. Create a new public GitHub repository.
2. Upload these files to the root of the repository:
   - `index.html`
   - `CNAME`
   - `.nojekyll`
   - `README.md`
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - Source: **Deploy from a branch**
   - Branch: **main**
   - Folder: **/root**
5. Save.

## Point GoDaddy domain to GitHub Pages

For `minkingdog.com`, add these A records in GoDaddy DNS:

- `185.199.108.153`
- `185.199.109.153`
- `185.199.110.153`
- `185.199.111.153`

For `www.minkingdog.com`, add:

- Type: `CNAME`
- Name/Host: `www`
- Value/Points to: your GitHub username followed by `.github.io`

Then in GitHub Pages, set the custom domain to:

`minkingdog.com`

Enable **Enforce HTTPS** after DNS finishes updating.

## Important

The original Airo save referenced image assets from the Airo preview server. This cleaned version points those image references to the preview URL so the page works on GitHub. If those images ever disappear from Airo, download them manually and replace the image URLs with local files in an `assets/` folder.
