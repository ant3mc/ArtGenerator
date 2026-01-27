# Art Generator

A real-time generative art application for relax, that creates colorful, cloud-like visual patterns using WebGL 2.0 .  All-in-one html file( with integrated CSS and JS).

## Features

### Visual Generation
- **Two Generation Methods:**
  - **Simplex Perlin Noise** (recommended) – produces natural, organic patterns
  - **Radial Gradient** (economic) – creates smooth color transitions

- **Customizable Visuals:**
  - 8, 10, or 12 dynamic spots with breathing animations
  - Adjustable saturation, brightness, opacity, color variety, etc.

### Audio Reactivity
- Uses pentatonic scales for harmonious sound generation 
- **Sound Mapping:** Each spot corresponds to a frequency based on its hue value;
    volume is based on its brightness value

### Additional Features
- Auto-stop after 5 minutes

## Technical Requirements
- WebGL 2.0 support
- Modern JavaScript (ES6+) compatible browser
- Web Audio API for sound generation

## Usage
The application is contained in a single HTML file( with integrated JS and CSS) for easy distribution and execution.

## Implementation Notes
- **Simplex Noise:** Based on Stefan Gustavson’s implementation
- **Audio Generation:** Pure sine wave synthesis via Web Audio API
- **Rendering:** WebGL 2.0 fragment shader

---

**Created by ant3mc · 2026**


