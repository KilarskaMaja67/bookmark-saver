# bookmark-saver

A fast, lightweight, and completely dependency-free frontend web application built to curate and organize personal web links. The application delivers immediate visual feedback and guarantees session retention using native browser ecosystem capabilities.

![Application Preview](assets/screenshot.png)

---

## Key Architectural Capabilities

### 1. Session Persistence via LocalStorage API
The application bridges application state across browser reloads without requiring an external database connection or backend server layer.
* **State Syncing:** Real-time bookmark additions or deletions automatically serialize data structures directly into browser-localized `localStorage` strings.
* **Hydration Cycle:** On page load (`DOMContentLoaded`), an asynchronous initialization handler reads the cached JSON payload, parses data strings back into functional objects, and accurately re-hydrates the UI layer.

### 2. Client-Side Input Validation Guards
Implements rigid defensive programming constraints on the UI wrapper to protect the DOM from broken references or invalid actions:
* Enforces structural presence checks ensuring both name descriptors and targets are provided.
* Leverages protocol validation regex checking to ensure incoming links explicitly start with structural `http://` or `https://` schemas, preventing broken routing loops.

### 3. Responsive Component Layouts
The styling engine uses modern CSS principles to create an interface that behaves predictably across devices:
* Employs fluid Centered Flexbox containers ensuring immediate structural adjustment across mobile, tablet, and desktop viewports.
* Implements crisp design elements like dynamic hover-state transformations and specific shadows (`box-shadow`) to emphasize application layout depth.

---

## Technical Highlights

* **Pure Architecture:** Zero external dependencies, libraries, or heavy frameworks (e.g., No React/Vue)—written purely in standard modern JavaScript (ES6+).
* **Event-Driven Lifecycle:** Fully decoupled event listeners hook directly into the window lifecycle to decouple functional logic execution from raw HTML elements.
* **Semantic Markups:** Uses clean HTML5 structure tags ensuring high screen-reader accessibility and proper element hierarchies.

---

## Quick Launch

Since this project runs directly inside the browser ecosystem, you don't need any complex build tools or compile phases.

1. **Clone the project repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/bookmark-saver.git](https://github.com/YOUR_USERNAME/bookmark-saver.git)
