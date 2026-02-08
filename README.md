# Matter.js Rigid Body Editor

A lightweight visual editor for creating **usable Matter.js rigid body shapes**, built with PixiJS rendering and a Windows-classic inspired UI.

This editor was created because existing tools often export incorrect or unusable vertex data. The goal of this project is simple:

> **Draw → preview → export → use immediately in Matter.js**

No broken coordinates. No manual fixing.

---

## ✨ Features

* Visual rigid body editor for Matter.js
* Polygon / vertex editing
* Circle primitives
* Direction/orientation controls
* Per-vertex corner rounding
* Live physics preview (Matter.js renderer)
* PixiJS high-performance canvas rendering
* Windows 98 style UI (98.css aesthetic)
* Background image import for tracing shapes
* One-click export of Matter.js-ready code

Exported shapes are designed to work directly with:

```js
Matter.Bodies.fromVertices(...)
```

without requiring manual correction.

---

## 🎯 Why this exists

As of **Feb 8, 2026**, popular online editors such as:

[https://samgeven.github.io/matter-vertices-editor/](https://samgeven.github.io/matter-vertices-editor/)

export vertex data with incorrect coordinate mapping (X/Y values collapse or become invalid), making the shapes unusable in real Matter.js simulations.

This editor was built to solve exactly that problem:

✔ Correct coordinate space
✔ Accurate vertex export
✔ Immediate compatibility with Matter.js

---

## 🖥 Demo

Live demo:

[https://mossback360.github.io/](https://mossback360.github.io/)

No installation required — runs entirely in the browser.

---

## 🚀 Usage

1. Open the demo in your browser
2. Import a background image (optional)
3. Create shapes:

   * Add vertices
   * Adjust corners
   * Modify orientation
4. Preview physics behavior
5. Export generated Matter.js code

Example exported output:

```js
const body = Matter.Bodies.fromVertices(
  x,
  y,
  vertices,
  options
);
```

Drop it directly into your project.

---

## 🔧 Tech Stack

* PixiJS — rendering
* Matter.js — physics preview
* 98.css — retro UI styling
* Vanilla JavaScript

---

##  Current Limitations

* No magic-wand auto tracing tool (planned or undecided)
* Manual vertex placement required
* Focused on 2D rigid body workflows only

---

##  Design Philosophy

This tool prioritizes:

* Correct physics geometry
* Immediate usability
* Lightweight browser workflow
* Visual clarity over feature bloat

It’s meant to be a **practical bridge between art assets and physics simulation**, not a full modeling suite.

---

##  Roadmap Ideas

Possible future improvements:

* Auto edge tracing / magic wand
* SVG import cleanup
* Vertex snapping
* Constraint preview
* Shape presets

---

##  Contributing

Feedback, bug reports, and improvements are welcome.

If you find exported vertices behaving incorrectly in Matter.js — please open an issue.

---

##  License

Choose your license here.

---

##  Credits

Inspired by the need for reliable Matter.js tooling.

Built with vibe coding and stubborn refusal to accept broken vertex exports.

---

Enjoy building physics shapes that actually work.
