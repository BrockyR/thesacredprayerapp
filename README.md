# Sacred Prayer

Installable web app (PWA) with:

- **The Lost Prayer of Solomon**: a 7-day prayer journey with progress tracking
- **The Manuscript of Solomon**: 7 teachings with commentary and a daily practice
- **Specific Prayers**: 28 prayers in 4 categories (Strength & Comfort, Work & Provision, Family, Peace & Protection)
- **Gifts**: Song of God player, Divine Vitality recipes, Bible of Solomon

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app (HTML, CSS and JS) |
| `manifest.webmanifest` | App name, colors and icons used when installing |
| `sw.js` | Service worker: offline support |
| `icons/` | App icons (Android, iPhone, favicon) |
| `_headers` | Cloudflare Pages headers (service worker never cached, manifest type) |

## Hosting (Cloudflare Pages)

Connect this repository in Cloudflare Pages with:

- Framework preset: **None**
- Build command: *(empty)*
- Build output directory: **/**

The install button only works over HTTPS, so always share the `*.pages.dev` link (or a custom domain), never the raw file.

## Updating

After changing `index.html`, bump `VERSION` in `sw.js` (for example `sp-v2`) so installed apps pick up the new version.
