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

## Data

Figures are drawn from the public sources listed in the "Data Sources &
Methodology" section and are indicative only. Not investment advice.

Two caveats worth carrying forward if you update the numbers:

- **The global totals and the country rows use different methodologies.** The
  $624.62T / $506.73T headline figures are Statista *forecast market volumes*.
  The per-country capitalizations come from national sources measuring
  *realised asset value* (Zillow for the US, Savills for the UK). They are not
  comparable and deliberately do not sum to the global total.
- **China's capitalization has a very wide estimate range.** The ~$33T shown is
  household balance-sheet real estate; Goldman Sachs puts unsold inventory
  alone at ~$13T. Treat it as an order of magnitude, not a measurement.

## Notes

- The mobile hamburger button in the nav is currently decorative — the nav links
  are hidden below the `md` breakpoint and no drawer is wired up yet.
