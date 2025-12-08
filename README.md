# Art Generator

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
[![WebGL](https://img.shields.io/badge/WebGL-2.0-orange.svg)](https://get.webgl.org/webgl2/)
[![Language](https://img.shields.io/badge/Language-JavaScript%20ES6-yellow.svg)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

An interactive generative art application that creates mesmerizing abstract visualizations with synchronized audio( optional), running entirely in your browser.

## 🎨 Overview

Art Generator is a browser-based creative tool that generates real-time abstract patterns using WebGL 2.0 shaders. It combines mathematical noise functions, radial gradients, and dynamic color animations to produce colored visual effects, optionally accompanied by pentatonic soundscapes.

**Key Features:**
- Real-time GPU-accelerated rendering
- Two generation algorithms: Simplex Perlin noise and radial gradients
- Configurable color dynamics with HSV/RGB transformations
- Synchronized generative audio using Web Audio API
- Fully responsive design with multi-language support (Русский/English)
- Fullscreen immersive mode
- Auto-stop safety timer (5 minutes)

## 🚀 Demo


## 📋 Requirements

- **Modern browser** with WebGL 2.0 support:
  - Chrome 56+, Firefox 51+, Safari 15+, Edge 79+
- **Web Audio API** support (for audio features)
- Recommended: GPU with OpenGL ES 3.0 support

## ⚙️ Configuration Options

### Generation Method
- **Simplex Perlin**: Organic, noise-based patterns
  - 8/10/12 spots with fractal Brownian motion
- **Radial Gradient**: Smooth, circular patterns
  - 8/10/12 spots with gradient falloff

### Visual Parameters
- **Color Accent**: Boost or reduce RGB channels( 0.9 - 1.1)
  - Options: Red±, Green±, Blue±, or none
- **Hue Rotation Speed**: 1×, 1.5×, or 2×
- **Saturation** (Radial only): 0.4 to 1.0 (slider)

### Audio Parameters
- **Sound Mode**: Pentatonic scales in different tunings
  - Base notes: C or A
  - Frequencies: 440 Hz (standard) or 432 Hz
  - Octaves:  2, or 3
- **Master Volume**: 0.05 to 0.5 (with 0.05 step)

## 🛠️ Technical Details

### Architecture
- **Frontend**: Vanilla JavaScript (no dependencies)
- **Rendering**: WebGL 2.0 with GLSL 3.00 ES shaders
- **Audio**: Web Audio API with PeriodicWave oscillators
- **Styling**: CSS3 with responsive breakpoints
- **Localization**: JSON-based translation system

### Shader Pipeline
```glsl
// Key shader features:
- Simplex noise implementation (snoise)
- Fractal Brownian Motion (FBM)
- HSV→RGB color space conversion
- Dynamic spot positioning and breathing animation
- Real-time uniform updates
```

### Performance Considerations
- 60 FPS rendering on mid-range GPUs
- Automatic canvas resizing
- Efficient Float32Array uniform buffers
- Oscillator pooling for audio
- Graceful WebGL context loss handling

## 📄 License

This project is licensed under **GNU Affero General Public License v3.0 or later** (AGPL-3.0-or-later).

- **Main license file**: `LICENSE` (included in repository)
- **Online version**: https://www.gnu.org/licenses/agpl-3.0.txt
- **Key points**:
  - Free to use, modify, and distribute
  - Source code must be disclosed for network usage
  - Copyleft license - derivative works must be AGPL-licensed


## 🤝 Contributing

**Development Notes:**
- No build tools required - pure vanilla JS
- Follow existing code style (ES6 classes, async/await)

## 🐛 Troubleshooting

### WebGL Context Loss
**Problem**: "WebGL not supported" or black screen
**Solution**: 
- Update graphics drivers
- Enable hardware acceleration in browser settings
- Try a different browser

### Audio Not Working
**Problem**: No sound or "AudioContext suspended"
**Solution**:
- Click on the canvas to unlock audio (browser policy)
- Check that audio mode is not "none" in settings
- Verify Web Audio API support

## 👨‍💻 Author

**ant3mc** (2025)

- GitHub: [@ant3mc](https://github.com/ant3mc)

## 🙏 Acknowledgments

- Simplex noise implementation based on [Stefan Gustavson's work](https://weber.itn.liu.se/~stegu/simplexnoise/simplexnoise.pdf)
- Color space conversion algorithms from standard graphics references
- Pentatonic frequency calculations based on equal temperament tuning

---
