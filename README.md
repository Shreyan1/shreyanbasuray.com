# shreyanbasuray.com

Personal site of Shreyan Basu Ray, applied ML engineer and independent advisor on AI product evaluation and go-to-market.

Static site, no build step required to serve. Deployed to the apex domain
`shreyanbasuray.com` (see `CNAME`).

## Structure

```
/                     homepage
/work/                case studies
/consulting/          engagement types
/writing/             articles, papers, book, policy
/about/               background
/assets/              images (JPEG + WebP)
/papers/              PDFs
robots.txt            crawl rules, incl. AI answer engines
sitemap.xml           all five routes
llms.txt              plain-text brief for generative engines
.htaccess             Apache-only rules (ignored by GitHub Pages)
```

## Source

Pages are authored as Claude Design canvas documents (`*.dc.html`) and compiled
by `build.py` in the parent directory, which strips the canvas runtime, converts
hover styles to CSS, inlines behaviour as plain JS, and emits SEO metadata.
