# Ignivio — Production Site

This is the final static build.

## Structure
- `index.html` + subpages (`about.html`, `services.html`, `why-choose-us.html`, `case-studies.html`, `clients.html`, `quote.html`, `insights.html`, `contact.html`)
- `assets/` (css, img, video, fonts)
- `vercel.json` (cache headers + clean URLs)
- `sitemap.xml`, `robots.txt`

## Deploy to GitHub → Vercel
1. Create a new GitHub repo (public or private).
2. Upload the **entire contents** of this folder at repo **root** (not inside a subfolder).
3. In Vercel, **New Project → Import from GitHub**.
   - Framework: **Other** (static)
   - Build Command: **(leave empty)**
   - Output Directory: **(leave empty)** (root)
4. After deploy, add your domain `ignivio.co` in Vercel → Domains:
   - Apex (`ignivio.co`) **A** → `76.76.21.21`
   - `www` **CNAME** → `cname.vercel-dns.com`
   - (Vercel will also offer automatic nameservers if you prefer)
5. Force www→apex or apex→www (your choice) in Vercel → Domains → Redirects.
6. Verify:
   - `https://ignivio.co/` loads
   - HD hero video plays (`/assets/video/hero_real.mp4`)
   - CSS version in use: `assets/css/styles.v28.css`

## Cache Busting
CSS/JS are long‑cached and versioned (e.g., `styles.v28.css`). When updating styles, bump the filename (e.g., `styles.v29.css`) and update the `<link>` in each page.

## Troubleshooting
- If the site looks unstyled, your browser or CDN cached an old CSS. Hard refresh (Cmd/Ctrl+Shift+R).
- Open DevTools → Network → check that `styles.v28.css` returns 200 and not from a previous path.

— Finalized for production.


## Final v30 Notes
- All pages reference `assets/css/styles.v28.css`.
- Mobile header and footer are single-line, scrollable if overflow.
- Footer is a slim Ferrari-style bar across the site.
- Founder’s Thesis (`quote.html`) guaranteed to include a footer.
- Contact page uses the Client/Candidate toggle only.

Deploy steps unchanged (GitHub → Vercel). Cache-control and clean URLs configured via `vercel.json`.
