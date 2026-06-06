# Kaleidoscope Learning Website

Static website for [Kaleidoscope Learning](https://www.kaleidoscopelearn.com/).

## What's included

- `index.html` — main page
- `css/styles.css` — site styling
- `images/` — logo and section photos
- Contact form powered by [Formspree](https://formspree.io/)

## Run locally

```bash
python -m http.server 8080
```

Then open http://localhost:8080

## Deploy to GitHub

1. Create a new repository on GitHub (e.g. `kaleidoscope-website`)
2. Upload this entire folder, or use Git:

```bash
git init
git add .
git commit -m "Initial commit: Kaleidoscope Learning website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/kaleidoscope-website.git
git push -u origin main
```

3. Enable GitHub Pages:
   - Go to **Settings → Pages**
   - Under **Build and deployment**, set **Source** to **GitHub Actions**
   - Push this repo — the `pages.yml` workflow will deploy automatically

### If you see a 404

- Make sure `index.html` is at the **root** of the repo (not inside a subfolder)
- Your repo root should look like:
  ```
  index.html
  css/styles.css
  images/
  README.md
  ```
- In **Settings → Pages**, use **GitHub Actions** as the source (not `/docs`)

## Contact form

Submissions are sent via Formspree to the email configured in your Formspree dashboard.
