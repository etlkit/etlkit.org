# etlkit.org

The landing page for [EtlKit](https://github.com/etlkit/etlkit) — a fully open-source (MIT) ETL toolkit for .NET.

This is a single static page. No build step, no framework.

## Structure

```
index.html          markup
styles.css          page layout
etlkit-tokens.css   EtlKit brand tokens (colors, type, spacing, fonts)
assets/             logo, mark, favicons
```

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
