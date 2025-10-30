# Safeguarding — Static informational site

A small static website that provides plain-language guidance, reporting pages, and signposting for safeguarding concerns. The site is intentionally simple, responsive, and accessible so it can be hosted on static web hosts or embedded into larger sites.

## Key features

- Plain-language guidance about recognising, responding to, and preventing harm.
- Quick action links (report, support, emergency) and a reporting page.
- Clear layout with semantic HTML and accessible attributes.
- Styles in `assets/css/style.css` and images under `assets/images/`.

## Deployment

![Deployment][deploymentLink]

## Repository

![Repository][repositoryDefinition]

## Project Board

![Project Board][safeguardingProjectDef]

## User Stories

### 1

![User story 1][userStory1Image]

### 2

![User story 2][userStory2Image]

### 3

![User story 3][userStoryImage3]

### 4

![User story 4][userStory4Image]

### 5

![User story 5][userStory5Image]

### 6

![User story 6][userStoryImage6]

### 8

![User story 8][def]

### 9

![User story 9][userStoryImage9]

### 10

![User story 10][userStoryImage10]

### 11

![User story 11][userStoryImage11]

#### Website is fully responsive — Mobile

![mobile][mobileImage2]
![mobile][mobileImage1]
![Mobile device screenshot of the safeguarding website home page showing a single-column layout with a top navigation bar containing a logo and hamburger menu, a hero section with the heading Safeguarding — Static informational site and a short explanatory paragraph, three quick-action tiles labeled Report, Get support, Emergency, and a visible call-to-action button; white background with blue accent elements; overall calm, clear, and helpful tone](assets/images/readme-image/mobile-3.png)
![Mobile screenshot of the Safeguarding website showing the Types of Abuse section. Top header with a small shield logo and hamburger menu, centered page title TYPES OF ABUSE. A green carousel card is focused with heading Domestic abuse, paragraph: Threats, violence and abuse between individuals that are family members or in an intimate relationship. Subheading Signs | Indicators followed by bullets: Unexplained injuries; Changes in behaviour; Fearfulness around certain individuals; Withdrawal from social activities. Below the card the heading ACTION STEPS is partially visible. Single-column mobile layout, calm and informative tone](assets/images/readme-image/mobile-4.png)
![mobile](assets/images/readme-image/mobile-5.png)
![mobile](assets/images/readme-image/mobile-6.png)
![mobile](assets/images/readme-image/mobile-7.png)

#### Website is fully responsive — Tablet

![Tablet](assets/images/readme-image/ipad-1.png)
![Tablet](assets/images/readme-image/ipad-2.png)
![Tablet](assets/images/readme-image/ipad-3.png)

#### Website is fully responsive — Laptop

![Laptop](assets/images/readme-image/laptop-1.png)
![Laptop](assets/images/readme-image/laptop-2.png)

#### Website is fully responsive — Desktop

![Desktop](assets/images/readme-image/desktop-1.png)
![Desktop](assets/images/readme-image/desktop-2.png)

## Files (overview)

- `index.html` — Home / overview page (documented below)
- `help.html` — Guidance and contact/signposting information
- `Report.html` — Reporting form/page
- `success.html` — Confirmation page shown after a report
- `assets/css/style.css` — Main stylesheet
- `assets/images/` — Images and manifest (`site.webmanifest`)

The repository includes a small set of demo screenshots used for the README and documentation previews. They live in `assets/images/readme-image/`.

## Wireframe images

Belsamiq--used for wireframes for mobile, table and desktop screen sizes.

Desktop, tablet and mobile views:

![Desktop view](assets/images/readme-image/Desktop.png)

_Desktop — full-width preview used for README showcase._

![Tablet view](assets/images/readme-image/Tablet.png)

_Tablet — medium-width preview._

## Project-Board

![Mobile view](assets/images/readme-image/safeguarding-project-board.png)

## Repository (screenshots)

![Mobile view](assets/images/readme-image/safeguarding-repository.png)

_Mobile — narrow/small-screen preview._

Additional screenshots (click to open full size):
![Hero image](assets/images/readme-image/hero.png)
If you rename or move these images, update the paths above. To reduce README size on GitHub, consider using lower-resolution thumbnails or linking to the full-size images instead of embedding them all.

## Sections in `index.html`

Below are the primary sections found in `index.html`. Each entry lists the element/ID, its purpose, and quick notes for editing.
![Hero image](assets/images/readme-image/index.png)

-- Navigation (`<nav id="navbar">`)

- Purpose: global site navigation and brand/logo.
- Links: Home (`index.html`), Information (`#information`), Help (`#action`), Report (`report.html`).
- Edit notes: Update links or add menu items here. The small script at the bottom closes the mobile menu after link clicks.
  ![Hero image](assets/images/readme-image/report.png)

-- Header / Hero (`<header id="header">`)

- Purpose: site tagline and primary message.
- Edit notes: contains `#hero-section` placeholder and the main heading copy. Use `assets/images/` for any hero imagery.

![Hero image](assets/images/readme-image/people.png)
-- Information (`<section id="information">`)

- Purpose: brief introduction to safeguarding, short explanation and call-to-action.
- Edit notes: update the headline and lead paragraph to change the site's main messaging.

-- Quick Actions (`<section id="flat-signs-block">`)

- Purpose: four 'flat-sign' quick links (Report, Get support, Emergency, Look for signs).
- Edit notes: each tile is an `<a>` with label, action, and sub text. Links point to internal pages or anchors (e.g., `report.html`, `help.html`, `#types-of-abuse`).
  ![Hero image](assets/images/readme-image/actions.png)

-- People needing safeguarding (`<section id="people-needing-safeguarding">`)

- Purpose: card grid that explains groups who may need safeguarding (Children, Adults at risk, Elderly, Anyone at risk).
- Edit notes: images referenced are in `assets/images/` (filenames like `safeguarding_child.png`). Keep `alt` text descriptive for accessibility.

-- Types of Abuse (`<section id="types-of-abuse">`)
![Hero image](assets/images/readme-image/types-of-abuse.png)

- Purpose: a Bootstrap carousel listing many abuse types and signs/indicators.
- Edit notes: carousel items are inside `.carousel-inner` as `.carousel-item` — update headings, copy, and lists here. The carousel uses Bootstrap 5 markup and controls.

-- 6 Principles (`<section id="action">`)

- Purpose: titled "6 Principles of Safeguarding". A `div` with `id="six-principles"` is present for the principles content.
- Edit notes: currently the `#six-principles` container is empty — add markup here (cards, a list, or small paragraphs) to display the six principles.
  ![Hero image](assets/images/readme-image/desktop-2.png)
  -- Helpful resources (`<section id="helpful-resources">`)

- Purpose: curated external links (NSPCC, Age UK, Childline, etc.).
- Edit notes: links are external — set `target="_blank" rel="noopener"` if you want them to open in a new tab; keep descriptions short.

-- Footer / Contact (`<footer>` and `#contact`)

- Purpose: contact details, social links, and newsletter subscribe form (posts to `success.html`).
- Edit notes: the subscribe form is a plain POST to `success.html` — adjust `action` if you wire up a real backend or JS handler.
  ![Hero image](assets/images/readme-image/contact.png)

## Quick editing guide

- Content (text): edit `index.html` directly — headings and sections are marked with IDs described above.
- Styles: open and edit `assets/css/style.css`. The active file is `assets/css/style.css` and a minified copy (`style.min.css`) is provided.
- Images: replace or add images in `assets/images/`. Keep filenames and update `src` attributes in the HTML if you rename files.
- Scripts: there's a small inline script that auto-closes the mobile navbar. Bootstrap JS is loaded via CDN — update CDN link if you prefer a different version.

## Accessibility notes

- Images include `alt` attributes; keep them meaningful. Buttons and links include ARIA labels in some places (e.g., quick actions).
- Heading order is intentionally kept simple (H1 for page title, H2/H3 for subsections) — preserve semantic headings when editing.

## How to view locally

1. Quick (no server): open `https://darakhshanda.github.io/safeguarding/index.html` in your browser.
2. Recommended (local server):

## Tested

`https://validator.w3.org/detailedhtml#validate-by-uri`

`https://jigsaw.w3.org/css-validator/#validate_by_urihttps://validator.w3.org/detailed.html#validate-by-uri`

`https://jigsaw.w3.org/css-validator/#validate_by_uri`

## Credits

AI generated images used, all thanks to Copilot and free icons from `https://fontawesome.com/icons`

## License

Blasamiq
Bootstrap
Visual code
`Code Institute` for providing licences included in our LMS to use in this repository. Add a file if you want to publish under an open license.

---

This README was updated to document the sections in `index.html` and provide quick editing guidance.

[deploymentLink]: https://darakhshanda.github.io/safeguarding/
[repositoryDefinition]: https://darakhshanda.github.io/safeguarding
[safeguardingProjectDef]: https://github.com/users/darakhshanda/projects/3
[userStory1Image]: assets/images/readme-image/user-story-1.png
[userStory2Image]: assets/images/readme-image/user-story-2.png
[userStoryImage3]: assets/images/readme-image/user-story-3.png
[userStory4Image]: assets/images/readme-image/user-story-4.png
[userStory5Image]: assets/images/readme-image/user-story-5.png
[userStoryImage6]: assets/images/readme-image/user-story-6.png
[def]: assets/images/readme-image/user-story-8.png
[userStoryImage9]: assets/images/readme-image/user-story-9.png
[userStoryImage10]: assets/images/readme-image/user-story-10.png
[userStoryImage11]: assets/images/readme-image/user-story-11.png
[mobileImage2]: assets/images/readme-image/mobile-2.png
[mobileImage1]: assets/images/readme-image/mobile-1.png
