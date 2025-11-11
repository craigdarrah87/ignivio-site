# Ignivio — Static Site (Cleaned)

This package is ready for GitHub → Vercel static hosting.

## Quick Deploy
1. Push all files to a GitHub repo (public or private).
2. In Vercel: **New Project → Import** the repo.
3. **Framework Preset**: "Other".
4. **Build Command**: _None_.
5. **Output Directory**: `/` (root).
6. Set **Production Domain** to `ignivio.co` (or your preview domain).

## Cache-busting
All pages reference `assets/css/styles.v28.css?v=2025-11-11`. If you change CSS later, bump the query string (e.g., `?v=2025-12-01`) so Vercel/CDN serves the fresh file.

## SEO
- `robots.txt` and `sitemap.xml` are included.
- Canonical tags were added per page.
- OpenGraph/Twitter meta exists (index) and base OG fields were added to others.

## Accessibility
- Missing `alt` attributes were filled from filenames.
- External links with `target="_blank"` now include `rel="noopener noreferrer"`.

## Mobile
- Responsive meta viewport is set.
- Layout uses fluid widths with breakpoints in `assets/css/styles.v28.css`.

## Troubleshooting
- If styles don't appear to update: purge your browser cache and hard refresh.
- In Vercel, re-deploy after pushing changes and verify `styles.v28.css` loads **with** the `?v=` query string.
- If a page looks off, open devtools → Network tab → ensure all assets return status 200.

— Cleaned on 2025-11-11
