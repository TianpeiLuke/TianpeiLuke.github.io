# Personal Website — Tianpei (Luke) Xie

A single-file, dependency-free personal academic homepage (`index.html`). Plain HTML + CSS,
no build step, dark-mode aware, mobile-responsive.

## Preview locally

Open `index.html` in a browser, or:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to GitHub Pages

The standard setup gives you `https://tianpeiluke.github.io`:

1. Create a repository named exactly **`TianpeiLuke.github.io`** on GitHub.
2. Push this folder to it:

   ```bash
   git remote add origin git@github.com:TianpeiLuke/TianpeiLuke.github.io.git
   git add index.html README.md
   git commit -m "Personal homepage"
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages** → ensure Source is “Deploy from a branch”, branch `main`, folder `/ (root)`.
4. The site goes live at `https://tianpeiluke.github.io` within a minute or two.

## Customizing

- **Photo**: drop a `photo.jpg` next to `index.html` and follow the comment in the
  `<header class="hero">` block (swap the initials `div` for the `<img>` tag).
- **Colors**: edit the CSS variables at the top of `index.html` (`--accent`, etc.).
  Both light and dark palettes are defined there.
- **Content**: everything is one file — sections are marked by `<h2 id="...">` headings.
