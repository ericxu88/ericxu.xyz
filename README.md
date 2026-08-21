# ericxu.xyz

A one-page personal business card.

- **Style** — borrowed from [nousresearch.com](https://nousresearch.com): white paper, cyanotype blue (`#0071a9` / `#00547e`), Courier Prime body, uppercase serif nav, dashed rules, an `OUTPUT / SEED` stamp.
- **Format** — borrowed from [fauzanrahman.com](https://fauzanrahman.com): phone top-left, school top-right, name + email centred, one info line along the bottom.

No build step. Three files:

```
index.html   content — search for "EDIT" to find every field
style.css    look and feel — colours/fonts are CSS variables at the top
favicon.svg  tab icon
resume.pdf   linked from the Resume item
```

## Edit

Open `index.html` and edit the text in each `EDIT` block: nav links, phone, school, name/email, and the bottom line (location / role / research / resume). Replace `resume.pdf` whenever the resume changes.

## Preview locally

```sh
python3 -m http.server 8000
# → http://localhost:8000
```

## Deploy

It's static, so any host works: drag the folder onto Netlify/Vercel, or push to a GitHub repo and enable GitHub Pages. Point `ericxu.xyz` at it.

## Optional: exact Nous nav font

Nous uses the pixel-serif **Mondwest** (commercial, Pangram Pangram) and falls back to Times. The site already falls back to Times New Roman. If you license Mondwest, put the `.woff2` in `./fonts/` and uncomment the `@font-face` block at the top of `style.css`.
