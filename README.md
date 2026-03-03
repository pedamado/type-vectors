# Type Vectors Diagnostic

A lightweight, single-file web application designed for type design classes and typography enthusiasts. This tool allows users to inspect the vector architecture of any custom font, providing a visual, anatomical breakdown of bezier curves, nodes, and typographic metrics.

Inspired by the structural analysis of typeforms found in comprehensive studies like Albert Kapr's *The Art of Lettering*, this tool acts as an accessible, browser-based diagnostic window (similar to the glyph environments in FontLab or Glyphs App).

## 🚀 Live Demo

*(You can add a link to GitHub Pages here if you host it, e.g., <https://pedamado.github.io/type-vectors/>)*

## ✨ Features

- **Drag & Drop Interface:** Easily load local .otf, .ttf, or .woff font files directly into the browser.

- **Vector Anatomy Grammar:** The app automatically parses OpenType curve data and visually classifies nodes based on their geometric continuity:

    - 🟡 **Smooth Nodes (Circles):** Continuous curves where control points are collinear.
    - 🟡 **Tangent Nodes (Triangles):** Smooth transitions between straight lines and curves.
    - 🟡 **Corner Nodes (Squares):** Angled transitions or kinks in the path.

- **Layered Visibility:** Toggle individual anatomical elements on and off:

    - Fill Preview
    - Outlines (1px non-scaling stroke)
    - Handle Bars & Off-Curve Points (x-marks)
    - Font Metrics (Baseline, X-Height, Cap-Height, Ascender, Descender)
    - Sidebearings

- **Dynamic Testing:** Input custom text or use predefined industry-standard test words (e.g., *adhesion*, *hamburgefonstiv*). Includes quick toggles for Uppercase, Lowercase, and Sentence case.

- **Responsive Viewport:** The canvas natively scales the vector data to fit the screen width, keeping strokes perfectly crisp at 1px regardless of scale.

- **Export:** Download the current view as a fully layered, cleanly styled SVG file for use in vector editors like Adobe Illustrator.

- **Dark/Light Mode:** Accessible color schemes (Black, White, and Yellow) tailored for screen comfort and high contrast.

## 🛠️ Technology Stack

- **HTML5 / CSS3 / Vanilla JavaScript:** All contained within a single `type_vectors.html` file for ultimate portability.
- [**OpenType.js**](https://opentype.js.org/): Used to parse binary font files and extract path commands and metrics.
- [**Tailwind CSS**](https://tailwindcss.com/): Sourced via CDN for rapid UI styling and layout management.
- **Inline SVG:** Used for rendering the viewport to guarantee perfect vector scaling, non-scaling strokes, and clean export.

## 📥 Installation & Usage

Because this is a completely client-side, single-file application, no build steps or servers are required.

1. Clone or download this repository.
2. Open `type_vectors.html` in any modern web browser (Chrome, Firefox, Safari, Edge).
3. Drag and drop a font file into the sidebar to begin inspecting.

## 📝 Credits

- **Designed by:** Pedro Amado (FBAUP / i2ADS / Ligatures)
- **Developed by:** Gemini Pro 3.1 (March 2026)
- **More Information:** <https://github.com/pedamado/type-vectors>

## 📄 License

This project is open-source and available under the [MIT License](https://github.com/pedamado/type-vectors/blob/main/LICENSE).
