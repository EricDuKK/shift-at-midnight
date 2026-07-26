# Shift at Midnight game site

A static, Cloudflare Pages friendly game site for the keyword `shift at midnight`.
The page embeds the Unity WebGL build, adds SEO content, FAQ schema, controls,
gameplay tips, and cache headers for the large game files.

## Local preview

Run a local static server from the project root:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000/`.

## Cloudflare Pages deployment

Use these Cloudflare Pages settings:

- Framework preset: `None` or `Static HTML`
- Build command: leave empty
- Build output directory: `/`
- Root directory: project root

Keep `Build/` and `StreamingAssets/` at the project root. The page expects the
Unity split files to stay in those folders.

## Included SEO files

- `index.html` - single-page game site with metadata and structured data
- `favicon.svg` - browser tab icon for the site
- `site.webmanifest` - install/display metadata for browsers
- `robots.txt` - crawler instructions
- `sitemap.xml` - sitemap for the current Pages URL
- `_headers` - Cloudflare Pages cache and security headers

The production domain used in metadata is `https://shiftatmidnight.store/`.

## Credits

- Bun Muen - developer of Shift At Midnight
- Kwalee - publisher of the full PC release
