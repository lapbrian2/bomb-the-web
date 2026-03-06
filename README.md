# BOMB THE WEB

A graffiti wildstyle-inspired 3D portfolio landing page for Brian Lapinski. Built with Three.js, GSAP ScrollTrigger, Web Audio API, and pure CSS in a single HTML file. Every pixel gets tagged.

## Features

### 3D Scene
- **Toon-shaded WebGL** — Cel-shaded blocks, spray cans, stars, arrows, and paint drips with thick black outlines (MeshToonMaterial + BackSide outline trick)
- **Mouse parallax** — Camera tilts with cursor, smooth lerp into main RAF loop
- **Scroll-driven animation** — GSAP ScrollTrigger powers section reveals, fly-ins, and stagger effects
- **Floating particles** — Colored paint dots drift upward through the scene

### Interactive Features
- **Spray canvas** — Click & drag to spray paint on a full-width interactive canvas with color picker and size controls
- **Sticker slap** — Double-click anywhere to slap random emoji stickers with rotation
- **Click spray effect** — Click for paint splatter burst particles
- **Custom spray can cursor** — CSS pseudo-element nozzle with trailing ring

### Easter Eggs & Secrets
- **Konami code** — Party mode with rainbow cycling
- **"BUFF" keyboard code** — Graffiti buff/erase effect
- **Triple-click footer** — Snitch mode with inverted colors
- **Secrets panel** — Hidden ? button reveals all Easter egg hints
- **Blacklight/UV mode** — Toggle for fluorescent glow effect
- **Shake to rattle** — Mobile DeviceMotion triggers spray can rattle sound + particle scatter

### Audio & Effects
- **Spray can SFX** — Web Audio API synthesized hiss and rattle (no audio files)
- **Graffiti name generator** — Type your name, get a procedurally generated tag with random styles
- **Physics paint drips** — CSS drips fall from viewport top with randomized timing
- **Glitch/VHS transitions** — Screen flash on section enter
- **Speed run timer** — Tracks time from first scroll to footer

### Portfolio Content
- 6 procedurally generated gallery mini-canvases (block stack, spray arc, star burst, drip flow, tag cloud, geometric)
- 4 graffiti crew stories with character avatars
- 5 crew rules with numbered styling
- 3 project cards linking to live work
- Visitor tag counter (localStorage)
- Contact section with email, GitHub, LinkedIn links

## Tech Stack

- Three.js r128 (WebGL, MeshToonMaterial, DataTexture)
- GSAP 3.12 + ScrollTrigger (scroll-driven animation)
- Web Audio API (AudioContext, OscillatorNode, noise buffers)
- Canvas 2D API (gallery scenes, spray canvas)
- CSS custom properties + pseudo-element cursor
- Google Fonts (Black Han Sans, Oswald, Space Mono)
- Zero build step — single HTML file, CDN dependencies only

## Browser Compatibility

- roundRect fallback for older browsers
- iOS 13+ DeviceMotion permission handling
- AudioContext user gesture deferral
- Responsive mobile layout with touch support

## Run Locally

Just open `index.html` in a browser, or serve it:

```bash
npx http-server . -p 3456
```

## Live

Deployed via GitHub Pages from `master` branch.
