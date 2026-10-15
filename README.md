# Trong Srinutaphong — portfolio

Source for **https://trongsrinutaphong.vercel.app**, the personal site of Trong Srinutaphong (ตรง ศรีนุตพงษ์, Zen).

Plain static HTML and CSS: no build step, no JavaScript, no cookies, no analytics. Every push to `main` deploys on Vercel.

## Layout

| Path | Page |
|---|---|
| `index.html` | Home |
| `about/` · `projects/` · `awards/` · `contact/` | Section pages |
| `projects/<slug>/` | One page per project |
| `sitemap.xml`, `robots.txt` | Search engines (update `sitemap.xml` when you add a page) |
| `og.png` | Social preview image (1200×630) |
| `vercel.json` | Trailing-slash URLs and security headers |

The home page carries the Google Search Console `google-site-verification` meta tag; keep it in every change or Search Console loses verification.

Every page carries a canonical URL, Open Graph/Twitter tags and Person JSON-LD. When adding a page, copy an existing one and change the `<title>`, description, canonical and `og:url`.

Award wording is copied exactly as printed on each certificate.

## Preview locally

```bash
python -m http.server 4321
```
