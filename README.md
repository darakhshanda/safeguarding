# Safeguarding — Static informational site

A small static website that provides plain-language guidance, reporting pages, and signposting for safeguarding concerns. The site is intentionally simple, responsive, and accessible so it can be hosted on static web hosts or embedded into larger sites.

## Key features

- Plain-language guidance about recognising, responding to, and preventing harm.
- Quick action links (report, support, emergency) and a reporting page.
- Clear layout with semantic HTML and accessible attributes.
- Styles in `assets/css/style.css` and images under `assets/images/`.

## Files (overview)

- `index.html` — Home / overview page (documented below)
- `help.html` — Guidance and contact/signposting information
- `Report.html` — Reporting form/page
- `success.html` — Confirmation page shown after a report
- `assets/css/style.css` — Main stylesheet
- `assets/images/` — Images and manifest (`site.webmanifest`)

## Readme images / screenshots

The repository includes a small set of demo screenshots used for the README and documentation previews. They live in `assets/images/readme-image/`.

Desktop, tablet and mobile views:

![Desktop view](assets/images/readme-image/Desktop.png)

_Desktop — full-width preview used for README showcase._

![Tablet view](assets/images/readme-image/Tablet.png)

_Tablet — medium-width preview._

![Mobile view](assets/images/readme-image/mobile.png)

_Mobile — narrow/small-screen preview._

Additional screenshots (click to open full size):

![Screenshot 1](assets/images/readme-image/Screenshot%202025-10-30%20053812.png)
![Screenshot 2](assets/images/readme-image/Screenshot%202025-10-30%20053827.png)
![Screenshot 3](assets/images/readme-image/Screenshot%202025-10-30%20053912.png)
![Screenshot 4](assets/images/readme-image/Screenshot%202025-10-30%20053921.png)
![Screenshot 5](assets/images/readme-image/Screenshot%202025-10-30%20053934.png)
![Screenshot 6](assets/images/readme-image/Screenshot%202025-10-30%20053944.png)
![Screenshot 7](assets/images/readme-image/Screenshot%202025-10-30%20053954.png)
![Screenshot 8](assets/images/readme-image/Screenshot%202025-10-30%20083110.png)

If you rename or move these images, update the paths above. To reduce README size on GitHub, consider using lower-resolution thumbnails or linking to the full-size images instead of embedding them all.

## Sections in `index.html`

Below are the primary sections found in `index.html`. Each entry lists the element/ID, its purpose, and quick notes for editing.

-- Navigation (`<nav id="navbar">`)

- Purpose: global site navigation and brand/logo.
- Links: Home (`index.html`), Information (`#information`), Help (`#action`), Report (`report.html`).
- Edit notes: Update links or add menu items here. The small script at the bottom closes the mobile menu after link clicks.

-- Header / Hero (`<header id="header">`)

- Purpose: site tagline and primary message.
- Edit notes: contains `#hero-section` placeholder and the main heading copy. Use `assets/images/` for any hero imagery.

-- Information (`<section id="information">`)

- Purpose: brief introduction to safeguarding, short explanation and call-to-action.
- Edit notes: update the headline and lead paragraph to change the site's main messaging.

-- Quick Actions (`<section id="flat-signs-block">`)

- Purpose: four 'flat-sign' quick links (Report, Get support, Emergency, Look for signs).
- Edit notes: each tile is an `<a>` with label, action, and sub text. Links point to internal pages or anchors (e.g., `report.html`, `help.html`, `#types-of-abuse`).

-- People needing safeguarding (`<section id="people-needing-safeguarding">`)

- Purpose: card grid that explains groups who may need safeguarding (Children, Adults at risk, Elderly, Anyone at risk).
- Edit notes: images referenced are in `assets/images/` (filenames like `safeguarding_child.png`). Keep `alt` text descriptive for accessibility.

-- Types of Abuse (`<section id="types-of-abuse">`)

- Purpose: a Bootstrap carousel listing many abuse types and signs/indicators.
- Edit notes: carousel items are inside `.carousel-inner` as `.carousel-item` — update headings, copy, and lists here. The carousel uses Bootstrap 5 markup and controls.

-- 6 Principles (`<section id="action">`)

- Purpose: titled "6 Principles of Safeguarding". A `div` with `id="six-principles"` is present for the principles content.
- Edit notes: currently the `#six-principles` container is empty — add markup here (cards, a list, or small paragraphs) to display the six principles.

-- Helpful resources (`<section id="helpful-resources">`)

- Purpose: curated external links (NSPCC, Age UK, Childline, etc.).
- Edit notes: links are external — set `target="_blank" rel="noopener"` if you want them to open in a new tab; keep descriptions short.

-- Footer / Contact (`<footer>` and `#contact`)

- Purpose: contact details, social links, and newsletter subscribe form (posts to `success.html`).
- Edit notes: the subscribe form is a plain POST to `success.html` — adjust `action` if you wire up a real backend or JS handler.

## Quick editing guide

- Content (text): edit `index.html` directly — headings and sections are marked with IDs described above.
- Styles: open and edit `assets/css/style.css`. The active file is `assets/css/style.css` and a minified copy (`style.min.css`) is provided.
- Images: replace or add images in `assets/images/`. Keep filenames and update `src` attributes in the HTML if you rename files.
- Scripts: there's a small inline script that auto-closes the mobile navbar. Bootstrap JS is loaded via CDN — update CDN link if you prefer a different version.

## Accessibility notes

- Images include `alt` attributes; keep them meaningful. Buttons and links include ARIA labels in some places (e.g., quick actions).
- Heading order is intentionally kept simple (H1 for page title, H2/H3 for subsections) — preserve semantic headings when editing.

## How to view locally

1. Quick (no server): open `index.html` in your browser.
2. Recommended (local server):

```powershell
# from the project root folder
python -m http.server 8000
```

[link \[text\] [(http://localhost:8000)] Then open in your browser.

## Contributing

1. Create a branch from `main`.
2. Make changes and open a pull request describing what you changed and why.
3. For copy changes, ensure someone with subject-matter knowledge reviews sensitive wording (safeguarding guidance should be accurate and clear).

## License

No license is included in this repository. Add a `LICENSE` file if you want to publish under an open license.

---

This README was updated to document the sections in `index.html` and provide quick editing guidance.
