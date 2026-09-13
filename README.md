# whereiswren.com

Marketing site for the **Where is Wren** iOS app, served by GitHub Pages
at https://whereiswren.com. The app's source lives in the private
[Where-Is-Wren](https://github.com/chadakeith/Where-Is-Wren) repo.

- `index.html` – landing page
- `privacy.html` – privacy policy (draft, needed for the App Store listing)
- `favicon.svg` – site icon
- `CNAME` – custom domain for GitHub Pages
- `.nojekyll` – serve files as-is, no Jekyll processing

## Deploying

Every push to `main` runs `.github/workflows/pages.yml`, which publishes the
repo root to GitHub Pages.

One-time setup in **Settings → Pages**: set **Source** to **GitHub Actions**,
enter `whereiswren.com` as the custom domain, and tick **Enforce HTTPS** once
the certificate is issued. DNS (A/AAAA at the apex, `www` CNAME to
`chadakeith.github.io`) is managed in Cloudflare.

## Local preview

```sh
python3 -m http.server 8000
```
