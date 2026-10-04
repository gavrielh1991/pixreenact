# PixReenact — Project Page

Static project page for **PixReenact: Pixel-Conditioned Causal Video Diffusion for Streaming Head-Avatar Reenactment**.

Fully self-contained: all CSS/JS (Bulma + bulma-carousel), figures, and videos are vendored under `static/` — no CDN or external requests.

## Preview locally

```bash
cd project_page
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy to GitHub Pages (github.com/gavrielh1991)

Option A — dedicated repo (recommended, URL: `https://gavrielh1991.github.io/pixreenact/`):

```bash
cd project_page
git init -b main
git add .
git commit -m "PixReenact project page"
git remote add origin git@github.com:gavrielh1991/pixreenact.git
git push -u origin main
```

Then on GitHub: repo **Settings → Pages → Source: Deploy from a branch → main / (root)**.
The page goes live at `https://gavrielh1991.github.io/pixreenact/` within a minute or two.

Option B — user site (URL: `https://gavrielh1991.github.io/`): push the same contents to a repo named
`gavrielh1991.github.io` (branch `main`, root).

Total size is ~27 MB (largest file: the 5-minute video, ~19 MB) — well within GitHub limits.

## TODO before/after arXiv

- `index.html`: replace the `href="#"` on the **Paper** button with the arXiv URL and remove "(coming soon)".
- `index.html`: same for the **Code** button once the repo is public.
- `index.html`: update the BibTeX block with the arXiv identifier.
- `index.html`: the `og:image` meta tag assumes the page lives at
  `https://gavrielh1991.github.io/pixreenact/` — update the absolute URL if hosted elsewhere.

## Template credit

Layout adapted from the [Nerfies project page](https://github.com/nerfies/nerfies.github.io)
(CC BY-SA 4.0) — attribution is kept in the page footer.
