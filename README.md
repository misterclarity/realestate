# CapYield — Global Real Estate Software Solutions

A single-page dashboard covering global real estate market capitalization, rental
yields by country, and the software platforms investors use to track them.

Everything lives in `index.html` — no build step, no dependencies to install.
Tailwind CSS, Font Awesome, and Google Fonts are loaded from CDNs at runtime.

## Viewing locally

Open `index.html` in a browser, or serve the directory:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Publishing on GitHub Pages

1. Merge this branch into `main` (or whichever branch you want to publish).
2. Go to **Settings → Pages** in the repository.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*.
4. Pick the branch and the `/ (root)` folder, then **Save**.

The site goes live at `https://<username>.github.io/<repository>/` a minute or
two later. `.nojekyll` is committed so GitHub serves the files as-is instead of
running them through Jekyll.

## Notes

- All figures on the page are demonstrative, aggregated from the sources listed
  in the "Data Sources & Methodology" section. Not investment advice.
- The mobile hamburger button in the nav is currently decorative — the nav links
  are hidden below the `md` breakpoint and no drawer is wired up yet.
