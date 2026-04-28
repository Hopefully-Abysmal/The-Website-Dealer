# The Website Dealer

Static portal for properties under **Hopefully Abysmal LLC** (e.g. `twd.hopefullabysmal.com`).

## Layout

- `index.html` — hub listing each site.
- `el-ultimo/index.html` — merged launch page: **el-ultimo v2** narrative + gunmetal/silver/bronze/blood palette and armor textures from the folio, plus a **family / Uncle Daniel** block.
- `el-ultimo/studio.html` — tabbed folio (landing mock, shop, packaging, checklist).
- `el-ultimo/atlas.html` — fragrance industry reference (comparative analysis), same type palette as El Último.
- `ha-apex/index.html` — stub for Hopefully Abysmal LLC apex marketing.
- `byod/index.html` — BYOD landing placeholder.
- `c/demo-client/index.html` — proves `/c/<slug>/` client path pattern.
- `desire-paths/index.html` — placeholder for Desire Paths × El Último music side.

This repo is **Hopefully Abysmal / TWD only** — no separate foundation or other product sites here.

## Serve locally

From this folder, any static server works, for example:

`npx --yes serve -l 3000`

Then open `/` and `/el-ultimo/`.

## GitHub

Remote: [The-Website-Dealer](https://github.com/Hopefully-Abysmal/The-Website-Dealer.git). After the first push, connect the custom subdomain in your DNS and host (Cloudflare Pages, Netlify, GitHub Pages, etc.) to the repository root.
