# CV version 3 — Ioannis Koupidis

A standalone, editorial portfolio for Ioannis Koupidis. This project does **not** modify the existing `IoannisK_CV` repository.

## What is included

- A fully responsive homepage, About page, digital CV page and five case studies.
- Working **Full / TL;DR** reading modes on every case study. The URL stores the selected mode as `?view=tldr`.
- Sticky chapter navigation, animated project covers, scroll progress, in-page navigation, responsive menus and reduced-motion support.
- Download link to the existing verified PDF hosted in the original `IoannisK_CV` repository, plus real professional information. The original PDF is not duplicated in this repository.
- Schematic cover illustrations, explicitly labeled as illustrations rather than fake app screenshots.
- All content editable in `data.js`. Layout and behavior live in `app.js`; styles in `styles.css`.

## Preview locally

No build system or JavaScript framework is required. On a machine with Python:

```bash
python3 -m http.server 8000
```

Open http://localhost:8000/ in your browser. Do not open `index.html` as a `file://` URL because ES modules may be blocked.

## Publishing to GitHub Pages

1. The site files are already committed to the new repository `IoannisKP/CV-Port-IK` on `main`.
2. In repository **Settings → Pages**, select **Deploy from a branch**, `main`, `/ (root)` and save.
3. Once GitHub Pages publishes, the site URL should be `https://ioanniskp.github.io/CV-Port-IK/`.
4. Keep your existing `IoannisK_CV` repository and deployed site unchanged.

For local edits, clone `https://github.com/IoannisKP/CV-Port-IK.git` and push changes to the `main` branch.

## Before publishing publicly

- Replace the **illustrative project artwork** with selected authentic screenshots, research artifacts and wireframes as desired. The current art is openly labeled as schematic.
- Check current status of Scribe and PM Compass against their latest builds; project descriptions distinguish historical test snapshots from current behavior.
- Verify the exact counts used for TEDx Circles before publishing as measured evidence.
- Consider whether the phone number in the downloadable legacy CV should remain public. It is not displayed on the site's pages.
- Approve or revise the About Me copy; it is an editorial draft based on the supplied CV and project history.
- Add testimonials only after obtaining genuine, approved quotes. None are invented here.

## Source and design note

The editorial design is inspired by the layout principles and Full/TL;DR case-study pattern of Charles Honig's portfolio. All code, layout treatment, visual elements and text here are original, and no external proprietary design assets were copied.

## Accessibility

Semantic sections, keyboard-operated buttons, focus visibility, readable contrast and reduced-motion support are included. Test with your own browser and assistive technology before relying on a formal accessibility claim.