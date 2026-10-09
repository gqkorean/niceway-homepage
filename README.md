NICE-WAY HOMEPAGE v21 — MOBILE FIXES (2026-10-10)

Based on the user-provided v20 archive.

Changes
1. Mobile sauce-drop drawers: last menu items remain visible, left/right drawers size to the viewport.
2. Mobile shared header: search is icon-only on narrow widths; brand mark no longer overlaps it.
3. Homepage full-width banners: parallax now uses a clamped, section-relative offset; disabled movement on mobile to avoid exposed gaps.
4. Main footer: NICEWAY INC logo and copyright centered on phones.
5. Nice Works: removed MAKING / ON FOOD / USE IT / KEEP GOING badge overlays from work videos (captions retained).
6. About: first view now has a full-screen moving video and strong copy overlaid, matching Nice Works. Original headline and all chapters retained.
7. Nice Works first view: aligned full-height mobile hero behavior with About.
8. Product + recipe marquee: added direct touchscreen horizontal dragging, retaining desktop mouse-steered movement and automatic cycling; vertical page scrolling remains enabled.

Implementation
- New CSS name niceway-common-v21.css; all site pages refer to it to avoid old mobile cache.
- Previous v17 CSS and JS remain in the archive; original v17 JavaScript retained for the common menus/search.
- Existing linked actions, forms, and external image/video URLs were not changed.

Deployment
- Extract the ZIP and upload the CONTENTS (index.html, all other HTML files, styles, scripts and images directory) into the existing GitHub Pages website ROOT, replacing matching files.
- Keep the images/ directory and external assets. Do not only upload the ZIP file into the repository.
- After GitHub Pages deploys, refresh on mobile. If styles look unchanged, open a private/incognito tab or clear browser cache.
- Verify menu links, search, product/recipe carousels, About/Works hero footage, and the sample inquiry form on your phone.

Test notes
- Checked HTML script syntax using Node.js.
- Ran Chromium layout and synthetic touch-pointer checks using inlined local HTML/CSS for 390x844, 360x720 and 320x568 viewport sizes.
- Browser environment blocked normal URL navigation and external media/font loading, so real-device video autoplay, external footage and online submissions still require deployment testing.
