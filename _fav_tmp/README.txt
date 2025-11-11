
Ignivio Favicons & Manifest Package
-----------------------------------
Files in /assets/icons:

- favicon.ico
- favicon-16x16.png
- favicon-32x32.png
- favicon-48x48.png
- favicon-64x64.png
- favicon-96x96.png
- favicon-128x128.png
- favicon-180x180.png (apple-touch-icon.png)
- android-chrome-192x192.png
- android-chrome-512x512.png
- site.webmanifest
- HEAD-SNIPPET-FAVICONS.html (copy the tags into <head> of every page)

How to install:
1) Copy the entire /assets/icons folder into your project at the same path.
2) In every HTML <head>, paste the contents of HEAD-SNIPPET-FAVICONS.html (or include it once if you have a shared head).
3) Commit & deploy.
4) Test on desktop & mobile Google search. Favicons may take time to refresh; use the URL Inspection tool in Search Console to request reindex.

Notes:
- Google shows favicons next to site names on desktop and mobile. They must be accessible and not blocked by robots.txt.
- Keep icons square, with good contrast on dark backgrounds.
