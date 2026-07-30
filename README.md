# understory-site

Landing page for [Understory](https://github.com/VaishGajaraj/Understory-AI) — an open
benchmark asking whether NISAR L-band coherence can detect forest degradation beneath
closed canopy.

One file, no build step, no dependencies. `index.html` is the whole site.

## Deploying free with GitHub Pages

The included workflow publishes this static site from `main` with no build step.

1. Make this repository public (GitHub Pages is free for public repositories).
2. Open **Settings → Pages** in GitHub.
3. Under **Build and deployment**, choose **GitHub Actions** as the source.
4. Push to `main`, or run **Deploy to GitHub Pages** from the Actions tab.

The page will be available at `https://vaishgajaraj.github.io/understory-site/`.

If the repository needs to remain private, Cloudflare Pages or Vercel can host the
same `index.html` on their free tiers.

### Custom domain

Both providers take a custom domain in one screen. `understory.earth`,
`understory.eco` or similar would be the shortest, most citable option — worth
doing before the benchmark result is published and people start linking to it.

## Editing

The page is deliberately dependency-free: open `index.html` in a browser and it
works. Its interactive radar fields are simulations—a persistent skid trail emerging
from speckle while a transient rain signal does not. They must stay labelled as
simulated until replaced with real acquired data.
