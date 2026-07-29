# understory-site

Landing page for [Understory](https://github.com/VaishGajaraj/Understory-AI) — an open
benchmark asking whether NISAR L-band coherence can detect forest degradation beneath
closed canopy.

One file, no build step, no dependencies. `index.html` is the whole site.

## Deploying

This repo is **private**, and GitHub Pages does not serve private repositories on the
Free plan. Three ways to get a public URL:

| Option | URL you get | Cost | Private repo? |
|---|---|---|---|
| **Cloudflare Pages** | `understory.pages.dev` | free | yes |
| **Vercel** | `understory.vercel.app` | free (hobby) | yes |
| **GitHub Pages** | `vaishgajaraj.github.io/understory-site` | needs GitHub Pro | only on Pro |

### Cloudflare Pages (recommended — shortest URL, free with private repos)

1. <https://dash.cloudflare.com> → Workers & Pages → Create → Pages → Connect to Git
2. Authorise GitHub, pick `understory-site`
3. Framework preset **None**, build command **empty**, output directory `/`
4. Deploy. Every push to `main` redeploys automatically.

### Vercel

1. <https://vercel.com/new> → import `understory-site`
2. Framework preset **Other**, no build command, output directory `.`
3. Deploy.

### Custom domain

Both providers take a custom domain in one screen. `understory.earth`,
`understory.eco` or similar would be the shortest, most citable option — worth
doing before the benchmark result is published and people start linking to it.

## Editing

The page is deliberately dependency-free: open `index.html` in a browser and it
works. The hero is a `<canvas>` simulating a coherence field — a persistent skid
trail emerging from speckle while a transient rain blob does not. It is labelled as
simulated, and must stay labelled that way until it is replaced with real acquired
data.
