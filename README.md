# roohmadhani.github.io

The Rooh Madhani (ਰੂਹ ਮਧਾਣੀ) website, served by GitHub Pages at
https://roohmadhani.github.io.

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
- `assets/images/logo.png` — logo (exported from Canva; source designs
  live in Canva)

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
