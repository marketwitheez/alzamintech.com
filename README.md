# Al Zamin Technical Services — Website

Static site, no build step. Push the contents of this folder to the root of a Git repo and serve with any static host (GitHub Pages, Netlify, Vercel, cPanel). Domain: https://alzamintech.com

## Files
- `index.html` — main website (logo intro, animations, project planner chat)
- `services/` — 50 SEO landing pages (one folder each) + `services/index.html` hub
- `assets/site.css` — shared styles for the landing pages
- `company-profile.html` — printable company profile
- `img/`, `brand/` — photos and logo (required)
- `docs/` — downloadable PDFs
- `favicon.ico`, `favicon-*.png`, `apple-touch-icon.png`, `android-chrome-*.png`, `site.webmanifest` — icons
- `og-image.jpg` — social share image
- `sitemap.xml`, `robots.txt` — SEO

## After going live
1. Google Search Console → add property `alzamintech.com` → Sitemaps → submit `https://alzamintech.com/sitemap.xml`.
2. Bing Webmaster Tools → import from Search Console.
3. Create / claim the Google Business Profile with the same name, address and phone as the site (Office 401, Hamsa Building, Khalid Bin Al Waleed Rd, Dubai · 04 388 5548).
4. If the site is not served at https://alzamintech.com/, update the domain in `sitemap.xml`, `robots.txt` and the canonical / og tags.

GitHub Pages: Settings → Pages → Deploy from branch → `main` / root. Add a `CNAME` file containing `alzamintech.com` if using the custom domain.

## SEO checklist (already wired)
- `index.html` and every page carry title, description, canonical, Open Graph + Twitter tags, favicon links and business structured data in the static `<head>`, so WhatsApp, Facebook, LinkedIn and Google read them without running JavaScript.
- `og-image.jpg` (1200×630) is the share image for every page.
- `sitemap.xml` lists 54 URLs; `robots.txt` points to it.
- `404.html` is the not-found page; `.nojekyll` makes GitHub Pages serve files as-is.

## Test after publishing
- Share preview: https://developers.facebook.com/tools/debug/ and https://www.opengraph.xyz (paste https://alzamintech.com). WhatsApp caches previews; use "Scrape again" in the Facebook tool to refresh.
- Structured data: https://search.google.com/test/rich-results
- Sitemap: open https://alzamintech.com/sitemap.xml, then submit it in Google Search Console.
