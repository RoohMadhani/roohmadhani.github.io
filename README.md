# roohmadhani.github.io

The Rooh Madhani (ਰੂਹ ਮਧਾਣੀ) website, served by GitHub Pages at
https://www.roohmadhani.com (custom domain via `CNAME`; also
https://roohmadhani.github.io).

Built with Jekyll (GitHub Pages builds it automatically — no local tooling
required to publish; just push to `main`).

## Adding a new page

1. Create a Markdown file in the repo root, e.g. `blog.md`:

   ```markdown
   ---
   layout: page
   title: Blog
   subtitle: Optional subtitle shown under the title
   permalink: /blog/
   ---

   Page content in Markdown here.
   ```

2. Add it to the banner navigation in `_data/navigation.yml`:

   ```yaml
   - title: Blog
     url: /blog/
   ```

That's it — commit and push, and the page appears with the site header,
banner navigation, and footer.

## Structure

- `_layouts/default.html` — base HTML shell (header/banner nav/footer)
- `_layouts/page.html` — standard inner page (title hero + content)
- `_data/navigation.yml` — banner navigation links
- `assets/css/style.css` — brand styles (colors and fonts from the Rooh
  Madhani brand guidelines: Lilita One for display, Questrial for body)
- `assets/fonts/` — self-hosted webfonts (OFL-licensed; see LICENSE.md there)
- `assets/images/logo.png` — logo (exported from Canva; source designs
  live in Canva)

## Compliance posture (keep it this way)

The site intentionally collects **nothing**: no cookies, no analytics, no
forms, and **no third-party requests** (fonts are self-hosted rather than
loaded from Google's CDN, which would transmit visitor IPs to Google — a
GDPR problem and a COPPA concern for a children's brand). The privacy
policy (`privacy.md`) promises this, so if you ever add analytics, embeds
(YouTube, social widgets), or forms, update `privacy.md` first and expect
to need a consent banner for EU visitors. Text colors are chosen to meet
WCAG 2.1 AA contrast (see `accessibility.md`); raw brand terracotta
`#C6804C` fails as a text/background color for white or dark text — use
`--terracotta-ink` for text on light backgrounds.

## Brand palette

| Role | Hex |
|---|---|
| Terracotta (primary) | `#C6804C` |
| Green (primary) | `#5A8D3C` |
| Pink (primary) | `#EEB3E7` |
| Blue (supporting) | `#1800AD` |
| Cyan (supporting) | `#5CE1E6` |
| Lime (supporting) | `#DFFD6E` |
| Dark green (text/footer) | `#395628` |
