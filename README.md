# CV Port IK — Editorial redesign

A personal portfolio for **Ioannis Koupidis**, designed around his journey from creative work and entrepreneurship to digital product management. The website was built as a completely separate repository, leaving the previous `IoannisK_CV` website untouched.

## Design direction

The November 2026 redesign draws on the **page architecture** of [Charles Honig's portfolio](https://charleshonig.design/) rather than copying its content or proprietary assets:

- Dark editorial canvas, compact name-and-metrics introduction, and an image-first project gallery.
- Five distinct case-study narratives with oversized project artwork, structured metadata and long-form sections.
- Dedicated **Full / TL;DR** reading modes on every project; modes update the content, chapter navigation, query string and reading estimate.
- "Play" experiments, career narrative, experience, About and downloadable CV.
- Navigation hover effects, scroll reveals, progress indicators, animated contact invitation, keyboard support and reduced-motion styles.

## Projects

1. **HIROOM / Book an Island** — Hyper Island student prototype; user interviews, usability feedback and prioritization. Public prototype: https://book-an-island.lovable.app/
2. **Scribe** — macOS recorder; product decisions, acceptance tests and manually identified defects.
3. **Agent X** — UX design project; interviews, synthesis and wireframe testing.
4. **PM Compass** — private ongoing PM assistant. **In progress**, not launched.
5. **TEDx Circles** — concept discovery and pitch, not a launched service.

**HIROOM's artwork is a concept illustration, not a screenshot** of the Lovable editor or published prototype. The access-token-bearing Lovable editor URL supplied during discussion is deliberately **not stored** in this public repository. The public prototype link is included in the case study. To replace schematic artwork with actual interface images, use screenshots you own and have permission to share.

## Content integrity

Case studies distinguish research findings, recommendations, prototypes, completed capabilities and validated outcomes. Scribe's 283 passing automated tests and four manually discovered defects describe a historical snapshot, not necessarily the current state. PM Compass is private and still in progress. Konduko's SEK 1.5B+ amount refers to estimated aggregate procurement framework value, **not** company revenue.

## Editing

No build step is required. Pages are small, static HTML entry points and ES modules.

- `data.js` — biographies and case-study text
- `app.js` — layouts, case-study components and interactions
- `styles.css` — original base styling and illustration styles
- `redesign.css` — November 2026 editorial redesign overrides
- `work/*/index.html` — project entry points
- `assets/Ioannis-Koupidis-CV.pdf` — printable existing CV

### Preview locally

Run `python3 -m http.server 8000` at the repository root, then open `http://localhost:8000/`.

### GitHub Pages

In **Settings → Pages**, choose **Deploy from a branch**, `main`, `/ (root)`.

Expected preview: https://ioanniskp.github.io/CV-Port-IK/

The original CV repository is not modified. The pre-redesign state of this separate repository is preserved in branch `backup-before-editorial-redesign`.

## Notes

- Real Scribe screenshots linked to the existing public site may require an internet connection; they aren't faked.
- The visual reference's complete interactive animations and the authenticated Lovable editor could not be inspected through this environment. The interaction details here are original implementations based on verified public structure and documented requirements.
- Review responsive behavior and project screenshots in a real mobile browser before using the portfolio for applications.
