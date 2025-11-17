# Hands! AI Chef — Legal Pages (Vercel)

Static site ready for **Vercel** with clean URLs:
- https://legal.izzyappz.com/privacy
- https://legal.izzyappz.com/terms
- https://legal.izzyappz.com/support

## Deploy on Vercel (GitHub flow)
1. Create a new public repo (e.g., `hands-legal-vercel`).
2. Upload the contents of this folder to the repo root:
   - `index.html`
   - `privacy_index.html`
   - `terms_index.html`
   - `support_index.html`
   - `vercel.json`
3. In Vercel, **New Project** → import the repo → Framework: **Other** (static).
4. Keep defaults; Vercel will auto-deploy on every push.

## Add Custom Domain on Vercel
We’ll use `legal.izzyappz.com`:

1. In Vercel Project → **Settings → Domains** → **Add** → enter `legal.izzyappz.com`.
2. Vercel shows a **CNAME** target (usually `cname.vercel-dns.com`).

### If your DNS is on Squarespace
- Add a **CNAME** record:
  - **Host/Name**: `legal`
  - **Value/Target**: `cname.vercel-dns.com`
  - **TTL**: default
- Back in Vercel, wait for verification and enable **Enforce HTTPS**.

> If your DNS is at a registrar (e.g., GoDaddy, Namecheap, Cloudflare), create the same CNAME record there.

## Optional: Keep old .html links working
We added redirects in `vercel.json` so `/privacy.html` → `/privacy`, `/terms.html` → `/terms`, and `/support.html` → `/support`.

## Link inside your apps
- App Store Connect & Play Console: use `https://legal.izzyappz.com/privacy`, `https://legal.izzyappz.com/terms`, and `https://legal.izzyappz.com/support`.
- Inside the app: Settings → About → link to those URLs.

—
© 2025 IzzyAppz LLC
