# Sellix — Cross-border Finance Hero Section

A single-file, zero-dependency hero section built with pure HTML5, CSS3, and Vanilla JavaScript. Features a proportional scaling layout, an infinite video background loop, and a font-synchronized entrance animation.

---

## Key Technical Features

- **Zero Build Step:** Entirely self-contained in `index.html`. No frameworks, CSS preprocessors, or external JavaScript libraries.
- **Proportional Scaling (`--u` system):** All desktop elements scale against a `1280x800` reference grid using a unified dynamic CSS variable (`--u`), preventing layout reflows across resolutions.
- **Seamless Video Loop:** Employs a dual-player cross-fade technique (`#bgVideoA` and `#bgVideoB`) that eliminates the end-of-file jump cut for an uninterrupted background loop.
- **Font-Synchronized Animation:** Entrance animations execute only after `document.fonts.ready` resolves, preventing invisible text glitches (FOIT).
- **Responsive & Accessible:** Custom layouts for desktop, tablet, and mobile (preventing hyphen breaks on narrow screens). Full support for `prefers-reduced-motion: reduce`.

---

## Quick Start

### Option 1: Direct File
Open `index.html` directly in any web browser.

### Option 2: Local HTTP Server
Run a quick local server using Python:
```bash
python3 -m http.server 8000
