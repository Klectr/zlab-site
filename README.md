# zlab-site

Marketing site for [Zlab](https://github.com/Klectr/zlab) — the infinite-canvas notes app.

Served at [zlab.klectr.dev](https://zlab.klectr.dev) from the Klectr VPS (`/var/www/zlab`, nginx, TLS at Cloudflare).

## Editing

Static files, no build step: `index.html`, `fonts/`, and `og-image.png` (1200×630 share card, composed as SVG and rendered with resvg — script kept outside the repo). Edit, commit, and copy to the VPS:

```
scp -r index.html fonts root@<vps>:/var/www/zlab/
```

Design: the DeepSeek Harness system (near-black hero with blue atmosphere, white pill CTAs, Montserrat/DM Sans/Fragment Mono, 1080px container) — same treatment as zlorb.klectr.dev. The canvas mock in the hero is hand-built HTML/CSS; the sticky notes use the app's own Virgil font (`fonts/Virgil.woff2`, from the zlab repo).
