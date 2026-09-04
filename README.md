# Hikaru Sushi & Asian Kitchen – Website

Single-page, bilingual (DE/EN) website. No build step – just static files.

## Files
- `index.html` – the site (HTML + CSS + JS in one file)
- `impressum.html`, `datenschutz.html` – legal pages (German market)
- `speisekarte.pdf`, `getraenke.pdf` – full menus linked from the site
- `images/` – put the restaurant's own photos here (see below)

## Before going live – placeholders to fill
1. `index.html` → `HIER_DEINEN_ACCESS_KEY_EINFUEGEN` – Web3Forms access key (free at web3forms.com)
2. `index.html` → `[ONLINE-BESTELL-LINK]` (Lieferando/own shop URL), `[E-MAIL-ADRESSE]`, `[INSTAGRAM-LINK]`, `[FACEBOOK-LINK]`
3. `impressum.html` / `datenschutz.html` → all `[…]` fields (tax IDs, hosting provider)
4. Replace stock photos: swap the `images.unsplash.com` URLs in the hero (CSS), the about image and the `photos` array in `index.html` with `images/gallery-01.jpg` etc. Use lowercase filenames – the server is case-sensitive.

## Deploy (Hostinger)
- **Git:** hPanel → Advanced → Git → repo URL, branch `main`, directory `public_html` → Deploy
- **Manual:** hPanel → File Manager → `public_html` → upload all files incl. `images/` and the PDFs

## Git (run on your own machine)
```
git init && git add . && git commit -m "Hikaru website" && git branch -M main
git remote add origin https://github.com/<user>/hikaru-website.git && git push -u origin main
```
