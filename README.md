# CV Port IK

A portfolio for Ioannis Koupidis, built in a separate repository so the original `IoannisK_CV` website remains untouched.

## Current design

- **Light-first monochrome palette**: off-white, white, charcoal and gray, with automatic dark mode via `prefers-color-scheme: dark`.
- **Typography**: Manrope across the website; IBM Plex Mono is reserved for small labels and metadata. No serif display type.
- **Project gallery**: six image-led project tiles with gentle staggered reveals, desktop pointer-responsive movement, and reduced-motion support.
- **Case studies**: each project has its own shareable page with Full and TL;DR reading modes, chapter navigation and reading-time estimates.
- **Navigation**: Home, Work, About, CV and contact. No standalone Play / Other Experiments section.

## Featured projects

1. **HIRoom** | Hyper Island room booking prototype, including 10 moderated booking-task participants. Five authentic screenshots are included; the teammate email addresses in one image are blurred.
2. **Scribe** | macOS meeting recorder. A documented snapshot reported 283 passing automated tests and four defects found through manual checks.
3. **Agent X** | UX research, synthesis and wireframe evaluation.
4. **PM Compass** | private, ongoing product. Not publicly launched.
5. **TEDx Circles** | community concept and pitch. Not a deployed program.
6. **Radio** | an eight-hour iOS app build, independent agent review and device testing. A separate review reported four blocking faults, and the iPhone exposed a network problem not seen in the simulator. This is a working build, not a released app.

The Radio case-study artwork uses an image from the original public portfolio. Actual project screenshots retain their native colors; the **site interface itself has no decorative accent color**.

## Source files

- `data.js`: biography, experience, project content and Full/TL;DR case-study narratives
- `app.js`: page composition, gallery and reading-mode interactions
- `styles.css`: shared baseline component styles
- `redesign.css`: light/dark palettes, typography and contemporary editorial layout
- `work/*/index.html`: project-specific pages

There is no build step. Serve the repository locally with `python3 -m http.server 8000`, then open `http://localhost:8000/`.

## GitHub Pages

In GitHub repository **Settings > Pages**, select deployment from `main` and `/(root)`.

Expected public address: https://ioanniskp.github.io/CV-Port-IK/

The original portfolio remains unchanged. A backup of the state before the current monochrome redesign was created as `backup-before-monochrome-radio`.

## Accuracy and remaining work

The project descriptions distinguish research evidence, prototypes, proposed improvements and finished behavior. Konduko's estimated aggregate SEK 1.5B+ procurement-framework value is **not** company revenue.

Authentic HIRoom screenshots are committed locally, but some other portfolio images are linked from the original public portfolio. Check those links and review responsive layouts in a real browser before relying on the portfolio for job applications.
