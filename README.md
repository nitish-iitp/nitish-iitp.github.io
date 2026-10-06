# nitish-iitp.github.io

Personal academic website of **Nitish Kumar**, Ph.D. Scholar (CSE), IIT Patna.

Live at: https://nitish-iitp.github.io

## Deploy on GitHub Pages

1. On GitHub, create a new **public** repository named exactly `nitish-iitp.github.io`.
2. Upload the contents of this folder (`index.html`, `assets/`, `.nojekyll`, `README.md`) to the repo root.
   - Web: *Add file → Upload files*, drag everything in, commit.
   - Or from a terminal:
     ```bash
     git init
     git add .
     git commit -m "Initial site"
     git branch -M main
     git remote add origin https://github.com/nitish-iitp/nitish-iitp.github.io.git
     git push -u origin main
     ```
3. Go to **Settings → Pages**, set *Source* to **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. After a minute or two the site is live at **https://nitish-iitp.github.io**.

## Updating

Everything is in `index.html`. To add a paper, copy an `<article class="pub">…</article>` block and edit it.
When a paper under review is accepted, move its block from *Under Review* to *Published / Accepted*
and update the counts in the `stats` section near the top.

To add a downloadable CV, put the PDF at `assets/cv.pdf` and add a button next to the LinkedIn one:

```html
<a class="btn" href="assets/cv.pdf" target="_blank" rel="noopener">CV</a>
```
