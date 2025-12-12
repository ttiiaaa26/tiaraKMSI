Dicicip.in — KMS (Single-file final)
====================================

This ZIP contains a polished single-file Knowledge Management System for Dicicip.in.
Navbar combines original website menu (Home, Menu, About, Contact) plus KMS pages:
Home | Menu | Artikel | Kategori | Bookmark | Dashboard | About | Contact

Files:
- index.html  -- single-file app (HTML + CSS + JS)
- sw.js       -- service worker (simple caching)
- manifest.json
- README.md
- icons/      -- placeholder icons

How to run:
1. Extract ZIP.
2. For full PWA/service-worker functionality, serve over HTTP:
   python3 -m http.server 8000
   open http://localhost:8000
3. Use Login -> select Admin/Editor/Viewer to test permissions.
4. Import/Export JSON available.

Notes:
- All data stored in browser localStorage.
- No external API required.
- To deploy to GitHub Pages, push files to repo and enable Pages (root).
