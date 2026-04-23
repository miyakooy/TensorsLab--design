# Assets

This folder holds the reusable starter components for TensorsLab Design.

## What these starter components mean

These are not final deliverables. They are the **base design primitives** the skill copies into an HTML file or adapts into a deck / prototype / motion piece.

They should give the agent:

- a known visual frame
- a predictable layout contract
- a reusable interaction shell
- a stable export structure

## Core starter components

### `animations.jsx`
Use for motion-heavy work.

Expected contract:

- timeline helpers
- easing helpers
- sprite / scene primitives
- reusable animation loop logic

### `ios_frame.jsx`
Use for iPhone prototypes.

Expected contract:

- device bezel
- safe-area handling
- dynamic island / status-bar placement
- app content viewport

### `android_frame.jsx`
Use for Android device mockups.

Expected contract:

- device silhouette
- top and bottom system chrome
- app viewport sizing

### `macos_window.jsx`
Use for desktop app mockups.

Expected contract:

- window chrome
- traffic-light controls
- title bar
- content viewport

### `browser_window.jsx`
Use for web app mockups shown inside a browser.

Expected contract:

- tab bar or URL bar
- browser chrome
- content viewport

### `deck_stage.js`
Use for single-file slide decks.

Expected contract:

- slide navigation
- active slide state
- keyboard controls
- speaker-note support
- scale-to-fit handling

### `deck_index.html`
Use for multi-file slide decks.

Expected contract:

- deck manifest
- slide list / slide embedding
- keyboard navigation wrapper
- print/export-friendly structure

### `design_canvas.jsx`
Use for side-by-side design variants.

Expected contract:

- comparison grid
- labels for variants
- responsive spacing
- consistent framing

## Manual fill requirements

Some components only become useful after you add TensorsLab assets:

- logo files
- brand colors
- real screenshots
- hero images
- product imagery
- case-study images

## How to use these files

1. Copy the relevant starter into the project HTML or task folder.
2. Replace placeholders with TensorsLab assets.
3. Keep the layout contract intact.
4. Export or verify once the design is complete.
