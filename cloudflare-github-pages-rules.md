# Cloudflare settings for walnutscafe.co.uk on GitHub Pages

GitHub Pages does not support `.htaccess`, so use Cloudflare instead.

## DNS

A records for apex domain `@`:

- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

CNAME for `www`:

- `www` → `chartataglance.github.io`

Set records to **DNS only** until GitHub Pages finishes HTTPS certificate provisioning. You can enable proxy later if needed.

## SSL/TLS

- SSL/TLS mode: Full
- Always Use HTTPS: On
- Automatic HTTPS Rewrites: On

## Redirect rule

Create a Cloudflare Redirect Rule:

- If hostname equals `www.walnutscafe.co.uk`
- Then static redirect to `https://walnutscafe.co.uk/$1`
- Status code: 301

## Cache rule

Cache static assets aggressively:

- If URI path starts with `/assets/`
- Browser TTL: 1 year
- Edge TTL: 1 month or more
