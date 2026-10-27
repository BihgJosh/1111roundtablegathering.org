MDGIFT 11:11 ROUNDTable — Complete Source Bundle

This bundle includes the full single-page site, build files, and the image, logo, flyer, brochure, video, and yearly photo archive resources referenced by the page.

Contents:
- index.html: full page markup, CSS, and browser JavaScript
- public/resources/: images and media referenced by the page
- scripts/extract-gallery-zips.cjs: prepares the 2023–2025 albums
- package.json and Vite/PostCSS/Tailwind configuration
- tests/tests.json: AppDeploy UI workflow checks

To build locally:
1. Install Node.js.
2. Open a terminal in this folder.
3. Run: npm install
4. Run: npm run build
5. The static site output is generated in dist/.

Keep the public/resources filenames unchanged; the page references these paths directly.
