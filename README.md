# safeguarding

## Logo and icon assets

This project includes vector logo sources and a helper script to generate bitmap exports (PNG, WebP) and a favicon.

- Vector sources:
	- `assets/images/logo.svg` — primary editable SVG (full colour)
	- `assets/images/logo-mono.svg` — single-colour variant for print/stamps
	- `assets/images/logo-favicon.svg` — compact icon used as a source for favicon/exports

- Generate bitmap exports

Run the PowerShell helper to export PNG/WebP sizes and create a `favicon.ico`:

```powershell
.
\assets\tools\generate-icons.ps1
```

Prerequisites: ImageMagick (`magick`) or Inkscape installed and available in PATH. The script will prefer ImageMagick if present and fall back to Inkscape.

Generated assets will be written to `assets/images/exports/`.

This site offers straightforward, accessible information about safeguarding for workplaces and educational settings. It explains what safeguarding is, lists common indicators (behavioural, physical, online), and gives step‑by‑step actions to keep people safe and to report concerns responsibly. The site also includes emergency signposting, multi‑channel reporting options (including an anonymous option), and links to short training resources. Content is written plainly, designed for quick scanning, and follows accessibility best practices so everyone can use it
