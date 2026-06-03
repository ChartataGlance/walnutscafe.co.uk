# Final production-ready structure

Upload the contents of this folder to:

`chartataglance/walnutscafe.co.uk`

Recommended repository settings:

- GitHub Pages source: Deploy from branch
- Branch: `main`
- Folder: `/ (root)`
- Custom domain: `walnutscafe.co.uk`
- Enforce HTTPS: On

```text
walnutscafe.co.uk/
├── index.html
├── about.html
├── menu.html
├── locations.html
├── gallery.html
├── styles.css
├── script.js
├── CNAME
├── robots.txt
├── sitemap.xml
├── .nojekyll
├── _headers
├── _redirects
├── cloudflare-github-pages-rules.md
├── production-structure.md
├── README.md
└── assets/
    ├── walnuts-W.jpg
    └── walnuts-logo.png
```

Notes:

- `.htaccess` is not used by GitHub Pages.
- `_headers` and `_redirects` are included as alternatives for Cloudflare Pages/Netlify.
- For GitHub Pages + Cloudflare DNS, apply redirects and security headers through Cloudflare Rules.
