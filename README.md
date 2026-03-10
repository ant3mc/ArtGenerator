   # Art Generator

A real-time generative art application for relax, that creates "breathing" visual patterns using canvas and WebGL 2.0 .  All-in-one html file( with integrated CSS and JS).

![IMG_20260227_150039](https://github.com/user-attachments/assets/d28b93bd-33ea-4f22-b979-75c23fa6696b)


## Features

### Visual Generation
- **4 Generation Methods:**
  - 2 in index.html   
  - 2 in ArtGenAlt.html

- **Customizable Visuals:**
  - 8, 10, or 12 dynamic spots with breathing animations
  - Adjustable saturation, brightness, opacity, color variety, etc.

### Audio Reactivity
- Uses pentatonic scales for sound generation 
- **Sound Mapping:** Each spot corresponds to a frequency based on its hue value; volume is based on its brightness value 
- The audio **mutes** if spots number > 12 or color variety < 30 
### Additional Features
- Auto-stop after 5 minutes
- If the saturation increases, it is recommended to reduce color variety 
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

<video src="https://github.com/ant3mc/ArtGenerator/raw/refs/heads/main/FBMSpotsVideo.mp4" controls width="600"></video>










