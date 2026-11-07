# Soda — Interactive 3D Landing Page

A single-file creative product concept with a floating 3D can, Classic / Zero Lime flavor switching, cherry and blueberry models, bubbles, cursor parallax, and GSAP transitions.

## Run locally

Open `index.html` in a modern browser, preferably using a static HTTP server (for example `python3 -m http.server 8000`). No build or package installation required.

## Assets

The page loads its GLB models, PNGs, JPG textures, Google Fonts, GSAP, and model-viewer from third-party CDNs. An internet connection is required. Asset availability and cross-origin permissions must be verified before deployment.

## Deploy

Deploy this repository as a static site on Vercel, Netlify, or GitHub Pages, with `index.html` at the root. Review the preview before publishing. The repository is public; do not assume its contents are private.

## Notes

- Product prices and awards are illustrative; checkout and contact information are not implemented.
- Navigation items beyond Home display placeholder notices.
- Reduced-motion preferences disable decorative movement.
- Mobile layouts are implemented, but physical iPhone and desktop browser testing are still required.

## Mobile performance mode

On screens up to 760px, the site starts with a lightweight product PNG instead of automatically rendering WebGL. Tap **Enable 3D** to opt in to the interactive model. Decorative berries are lightweight elements rather than separate WebGL scenes. Animation updates are throttled, and bubbles are less frequent. These changes prioritize mobile stability over exact visual fidelity.

**Verification status:** code committed, but no real Safari or desktop browser performance measurements have been run yet. The Vercel production deployment on `main` is not changed by this feature branch.
