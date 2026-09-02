# Giant Component — course site

Static site for a 02805 group blog. No build step — plain HTML/CSS.

## Deploy to GitHub Pages

1. On github.com, click **New repository**. Give it any name (e.g. `giant-component`). Public, no README/gitignore needed (you already have files).
2. On your computer, in this `site/` folder, run:
   ```
   git init
   git add .
   git commit -m "First version of the site"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
   git push -u origin main
   ```
3. On GitHub, go to the repo's **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
5. Wait a minute, then your site is live at `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`.

## Editing

- `index.html` — homepage: hero text, member names, posts list, about section.
- `posts/week1-bootstrap.html` — first post; duplicate this file for each new week and add a matching `<li>` to the posts list in `index.html`.
- `style.css` — all styling in one file, colors defined as CSS variables at the top.
- Replace the `GitHub` link in `index.html`'s nav with your actual repo URL once it exists.

## Adding images

Put images in an `assets/` folder and reference them with `<img src="assets/your-image.png" alt="...">` inside a post's `<figure>` block.
