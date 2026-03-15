# thoughtsre.github.io

The landing page for [thoughtsre.com](https://thoughtsre.com).

## Setup

1. Create a repo named `thoughtsre.github.io` under the `thoughtsre` GitHub org
2. Push all files in this directory to the `main` branch
3. Add your logo as `logo.png` in the repo root (the transparent PNG with white background)
4. In the repo settings → Pages → set source to "Deploy from a branch" → `main` / `/ (root)`
5. Configure DNS (see below)

## DNS Configuration

At your domain registrar, add the following DNS records for `thoughtsre.com`:

```
Type    Name    Value
A       @       185.199.108.153
A       @       185.199.109.153
A       @       185.199.110.153
A       @       185.199.111.153
CNAME   www     thoughtsre.github.io
```

After DNS propagates (may take up to 24 hours), enable "Enforce HTTPS" in the repo's Pages settings.

## Files

- `index.html` — the site (single page, no build step)
- `CNAME` — tells GitHub Pages to serve at thoughtsre.com
- `logo.png` — your wordmark (you need to add this)
