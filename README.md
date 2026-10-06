# etlkit.org

The landing page for [EtlKit](https://github.com/etlkit/etlkit) — a fully open-source (MIT) ETL toolkit for .NET.

This is a single static page. No build step, no framework.

## Structure

```
index.html          markup, meta tags, JSON-LD structured data
styles.css          page layout
etlkit-tokens.css   EtlKit brand tokens (colors, type, spacing, fonts)
assets/             logo, mark, favicons, social preview image
llms.txt            summary of EtlKit for LLM assistants (https://llmstxt.org)
robots.txt          crawler rules and sitemap location
sitemap.xml         page list for search engines
tools/              sources of generated assets, not deployed (.vercelignore)
```

The canonical host is `https://www.etlkit.org` (the apex domain redirects
there). Use it in `canonical`, `og:url`, `sitemap.xml` and `robots.txt`.

When the page content changes, update `lastmod` in `sitemap.xml`. When facts
about the library change (packages, connectors, API), update `llms.txt` and
the connector table in `index.html` together.

The social preview `assets/og-image.png` is rendered from
`tools/og-image.html`; the command is in that file's header comment.

## Local preview

Any static server works, e.g.:

```bash
npx serve .
# or
python3 -m http.server
```

Then open http://localhost:3000 (or :8000).

## Deploy on Vercel

It's a plain static site, so no configuration is required — Vercel serves the
repo root as-is.

1. Push this repo to GitHub.
2. In Vercel, **Add New → Project** and import the repo.
3. Framework preset: **Other**. Leave build command empty and output directory
   as the root.
4. Deploy, then add `etlkit.org` under **Settings → Domains**.

`vercel.json` is included with sensible caching headers for the static assets.

## License

Site content and code: MIT. EtlKit branding © EtlKit contributors.
