# The Website Dealer

Static portal for properties under **Hopefully Abysmal LLC** (e.g. `twd.hopefullabysmal.com`).

## Layout

- `index.html` — **The Website Dealer** homepage (deploy this at the document root for `twd.hopefullyabysmal.com` so `/` serves the portal).
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

Remote: [The-Website-Dealer](https://github.com/Hopefully-Abysmal/The-Website-Dealer.git).

## Deploy (GitHub Actions → FTP)

On every push to **`master`**, [.github/workflows/deploy-ftp.yml](.github/workflows/deploy-ftp.yml) uploads the static tree (minus `.git`, `.github`, root `README.md`, `.gitignore`) to your host for **twd.hopefullyabysmal.com**.

**Repository secrets:** `FTP_SERVER`, `FTP_USERNAME`, `FTP_PASSWORD` (Settings → Secrets and variables → Actions). If the FTP session lands in the wrong directory, add `server-dir: ...` under `with:` in the workflow to match the subdomain’s document root in SiteGround.

## DNS

Point **twd.hopefullyabysmal.com** at the same host; document root = this repo’s deployed files.
