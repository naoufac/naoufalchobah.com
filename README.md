# naoufalchobah.com — static mirror

A static mirror of [naoufalchobah.com](https://naoufalchobah.com/) — "Personal studio. Astrology, books, Transurfing, health as energy, and the physics school skipped. Pattern, not costume."

## Contents

- `index.html` — home (hero, room grid, birth-date calculator)
- `library.html` + `library/` — essays and the book shelf
- `reading.html`, `play.html` — longer notes and tools
- `health.html`, `health/sickness.html` — health as energy
- `fabric.html`, `fabric/being.html`, `fabric/manifestation.html` — the physics school skipped
- `_astro/` — hashed CSS/JS build assets (React island for the birth-date calculator)
- `nsc.svg` — favicon

## Deploying to GitHub Pages

1. Push this repo to GitHub.
2. Settings → Pages → Deploy from a branch → `main` / root.
3. Set a custom domain (`naoufalchobah.com`) if you want the original URLs to resolve.

Notes:

- `.nojekyll` is required so GitHub Pages serves the `_astro/` directory (Jekyll ignores underscore-prefixed folders).
- Assets are referenced with root-absolute paths (`/_astro/...`), so the site works on a root domain or custom domain. If you serve it from a subpath (`user.github.io/repo/`), rewrite `/_astro/` to `./_astro/` in `index.html` and `play.html`.

## Provenance

Mirrored with `wget` from the live site; the two hydration bundles (`BirthMath`, `client`, `react` chunks) were fetched manually. The `robots.txt` of the source site allows crawling (`User-agent: * Allow: /`).

Source content © its original author.
