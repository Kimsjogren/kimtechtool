# KimTechTool

Static website for [kimtechtool.se](https://kimtechtool.se) — hosted on GitHub Pages.

## Local preview

Open `index.html` directly in a browser, or run a simple server:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy (GitHub Pages)

1. Push this repo to GitHub.
2. Settings → Pages → Source: `Deploy from a branch` → `main` / `/ (root)`.
3. Custom domain: `kimtechtool.se` (the `CNAME` file is already in place).
4. Point DNS at GitHub Pages:
   - `A` records for the apex `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` record for `www` → `<your-github-username>.github.io`
5. Enable **Enforce HTTPS** once the certificate is issued.

## Structure

- `index.html` — page markup
- `styles.css` — styles
- `IMG_*.WEBP` — images used on the page
- `CNAME` — custom domain for GitHub Pages
