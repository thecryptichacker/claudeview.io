# ClaudeView Website

Static landing page for [claudeview.io](https://claudeview.io).

## Local preview

Open a terminal in this folder and run any of:

```bash
# Python 3
python -m http.server 8000

# Node (if you have npx)
npx serve .

# VS Code: right-click index.html → "Open with Live Server"
```

Then visit `http://localhost:8000`.

## Deploying to GitHub Pages

1. Push this folder to a GitHub repo (e.g. `claudeview-site`).
2. In the repo settings → **Pages**, set the source to the branch root (`/`).
3. The `CNAME` file already points to `claudeview.io` — just add the corresponding DNS records at your domain registrar:
   - `A` records for `claudeview.io` → GitHub Pages IPs (`185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`)
   - `CNAME` for `www.claudeview.io` → `<your-github-username>.github.io`
4. Enable **Enforce HTTPS** in the Pages settings once the DNS resolves.

## Placeholders to fill in later

All `href="#"` and `href="#pricing"` CTA buttons currently point at the pricing anchor. Swap them for the real download / checkout URLs when ready:

- "Start Free 3-Day Trial" buttons (hero, pricing card, final CTA, nav)
- Footer Terms / Privacy links

## File structure

```
ClaudeViewWebsite/
├── index.html      Single-file landing page (HTML + inline CSS + JS)
├── CNAME           Custom domain for GitHub Pages
└── README.md       This file
```
