# Cola Wars · Animations

3D drop animations for the Cola Wars Gamefound preview page. Hosted on GitHub Pages.

## Live

- **Gallery:** https://matthewmeeple.github.io/cola-wars-animations/
- **Head Space — caps drop:** https://matthewmeeple.github.io/cola-wars-animations/head-space.html
- **Shelf Space — bottles drop:** https://matthewmeeple.github.io/cola-wars-animations/shelf-space.html

## Controls

- **Drag** to orbit
- **Scroll wheel** to zoom (custom smooth-zoom)
- **Top-down / Product-shot toggle** — swap between near-top-down and 22° product angle
- **Debug slots / Debug rings** — wireframes at each slot for alignment verification
- **Record video** — captures 2 full loops as MP4/WebM

## Embed mode

Append `?embed=1` to hide the HUD (controls, title, hint) — designed for clean iframe embedding on the Gamefound preview page.

Examples:
- https://matthewmeeple.github.io/cola-wars-animations/head-space.html?embed=1
- https://matthewmeeple.github.io/cola-wars-animations/shelf-space.html?embed=1

## Architecture

Both animations share the same Three.js 0.160 architecture — walnut tabletop, 22° product-shot camera, three-point lighting, physics-feel drops via `easeInQuint`. The bottle extrusion is laid flat from the SVG silhouette so it aligns with the printed outlines on the shelf board; caps are rendered from the `bottlecap.obj` mesh on the head-space board.

Slot coordinates for Shelf Space were captured via click-calibration session (not eyeballed) to guarantee pixel-perfect alignment on the printed red outlines.
