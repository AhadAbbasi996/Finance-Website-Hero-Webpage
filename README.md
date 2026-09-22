# Sellix — Cross-border Finance Hero Section

A single-file, zero-dependency, ultra-high-performance landing page hero section built with standard HTML5, CSS3, and modern Vanilla JavaScript. 

It features a fluid reference-pixel design system (`--u`), a dual-element cross-fading background video loop that eliminates loop seam cuts, and an engineered entrance animation timeline tied to font-loading metrics and reduced-motion preferences.

---

## 🌟 Key Features

* **Zero Build Step & Zero Dependencies:** Single `index.html` file with all styles contained in a `<style>` block and native inline scripts. No Webpack, Vite, Tailwind, or React required.
* **Proportional Reference-Pixel Architecture (`--u`):** Built against a `1280x800` reference frame. All desktop measurements use fractional multiples of a single dynamically calculated root unit (`--u`), ensuring bit-identical scaling across displays without standard CSS reflow glitches.
* **Seamless Video Cross-fading Loop:** Utilizes a dual HTML5 `<video>` element technique (`#bgVideoA` & `#bgVideoB`). A modern JS `timeupdate` engine triggers a 0.9s cross-fade before video completion, masking the source video's end-to-beginning jump cut into an endless, imperceptible loop.
* **Font-Locked Entrance Animation Sequence:** The entrance timeline uses masked line rises and spring curves tied directly to `document.fonts.ready`. Text is revealed only when fonts are fully loaded to prevent invisible text jumps (FOIT/FOUT).
* **Fully Responsive Adaptive Architecture:**
  * **Desktop (>1160px):** Proportional `--u` fluid scaling.
  * **Tablet (553px – 1160px):** Adaptive layout with mobile menu drawer toggling.
  * **Mobile (<552px):** Dynamic headline calculation using non-hyphenating bounds so `"Cross-border"` never breaks mid-word on narrow viewports.
  * **Short Landscape:** Viewport height-compensated typography and padding adjustments.
* **Accessibility & Reduced Motion Native:** Full compliance with `prefers-reduced-motion: reduce`. Automatically disables video playback, anchors the hero frame to still poster capture, and bypasses entrance keyframes.

---

## 📂 File Structure

```text
├── index.html       # The self-contained production file
└── README.md        # Documentation
