# Safeguarding — Static informational site

A small static website that provides plain-language guidance, reporting pages, and signposting for safeguarding concerns in workplaces and educational settings. The site is intended to be easy to scan, accessible, and ready to serve as a simple resource and reporting front-end.

## Key features

- Plain-language guidance about what safeguarding is and how to act.
- Dedicated pages for help, reporting, and confirmation.
- A minimalist responsive layout styled with `assets/css/style.css`.
- Accessible content and simple structure so it can be hosted or embedded in larger sites.

## Project files (overview)

- `index.html` — Home / overview page
- `help.html` — Guidance and contact/signposting information
- `Report.html` — Reporting form/page
- `success.html` — Confirmation page shown after a report
- `assets/css/style.css` — Main stylesheet
- `assets/images/` — Images, webmanifest, and project graphics (e.g., `site.webmanifest`, `wireframe-safeguarding.bmpr`)

## How to view locally

1. Quick (no server): double-click `index.html` to open in your browser.
2. Recommended (local server) — useful for testing fetches or service worker behavior:

```powershell
# from the project root folder
python -m http.server 8000
```

Then open <http://localhost:8000> in your browser.

## Development notes

- Editing HTML: update the `.html` files at the repo root.
- Styling: `assets/css/style.css` contains the main styles — edit and refresh.
- Images and assets: placed under `assets/images/`.
- Accessibility: the content aims to follow simple accessibility guidelines (clear headings, readable contrast). If you update markup, please check headings and form labels.

## Contributing

1. Create a short-lived branch from `main` (or working branch).
2. Make changes and open a pull request describing the update.

## License

No license specified for this repository. Add a `LICENSE` file if you want to publish under an open license.

---

Updated README to clarify purpose, file layout, and how to preview the site locally.
