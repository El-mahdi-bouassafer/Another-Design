ANOTHER DESIGN — Website project

Contents
- docs/: all 13 website pages, CSS, JavaScript and images, ready to host on GitHub Pages.
- build.py: optional Python script that regenerates the HTML pages in docs/.

Hosting on GitHub Pages
1. Upload docs/ and build.py to the repository (drag the folders in, not a zip).
2. Settings > Pages > Deploy from a branch > main > /docs > Save.
3. The site is served at https://el-mahdi-bouassafer.github.io/Another-Design/

BASE path (important)
Links in the pages are written with a prefix set at the top of build.py:
  BASE='/Another-Design'
- Keep it as is for https://USER.github.io/Another-Design/
- Change it to '' (empty) if you use a custom domain, or if the repository is named
  USER.github.io (site served from the root), then run: python3 build.py

Preview locally (same URL layout as GitHub Pages)
1. In the project folder run:
     mkdir -p /tmp/site && ln -sfn "$PWD/docs" /tmp/site/Another-Design
     python3 -m http.server 8000 --directory /tmp/site
2. Open http://localhost:8000/Another-Design/

The contact form prepares a WhatsApp message for the visitor to review and send.
