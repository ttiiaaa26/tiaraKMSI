Dicicip.in — Knowledge Management System (KMS)
=============================================

This package contains a prototype single-file KMS (index.html) plus PWA helpers.

Files:
- index.html  -- Single-file KMS (localStorage-based)
- sw.js       -- Simple service worker for offline caching
- manifest.json -- PWA manifest
- README.md   -- this file

How to use:
1. Extract the ZIP.
2. Open index.html in your browser (for full PWA features, serve over HTTP).
   - For local testing with service worker, use a simple static server:
     - Python 3: `python -m http.server 8000`
     - Then open http://localhost:8000 in your browser.
3. Use the demo users (Login menu):
   - Admin, Editor, Viewer (select then Login)
4. Features:
   - Create / Edit / Delete articles
   - Search, filter, tags
   - Comments, rating, bookmarks
   - Import / Export JSON, backup download
   - Dashboard analytics
   - Dark mode toggle and automatic dark mode support

Deploy:
- You can host this on GitHub Pages by pushing the files to your repo's `gh-pages` branch or enabling Pages on the `main` branch (docs folder).
- For PWA behavior, ensure sw.js and manifest.json are served from the site root.

Notes:
- All data is stored locally in the browser (localStorage). To move to a server, replace localStorage logic with an API/backend.
- Icons are placeholders in manifest.json; add icons/icons-*.png to the `icons` folder for full PWA installability.
