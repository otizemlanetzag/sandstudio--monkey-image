# Monkey Image Studio

A browser-based 3D scene sandbox for composing images without needing a full 3D authoring suite.

## Run

Open `index.html` through a local web server or a static hosting service. The app loads Three.js modules from jsDelivr, so an internet connection is required.

## Included in this prototype

- Four-step workflow: Layout, Lights, Focus, Camera
- Interactive Three.js viewport with orbit, zoom, and pan
- Built-in starter objects for nature and everyday scenes
- Local model import for GLB/GLTF, OBJ, and FBX
- Editable object position and scale
- Adjustable directional lighting, temperature/color, and shadows
- Focus-point selection and cinematic depth-of-field post-processing in the render pipeline
- Aspect-ratio presets, rule-of-thirds overlay, and three camera slots
- PNG/JPG export at selected output dimensions

## Notes and limitations

This is an interactive prototype, not yet a physically based offline path-tracing renderer. The Render action renders the scene at the selected dimensions and applies a Three.js Bokeh depth-of-field post-processing pass. It does not provide full ray tracing, denoising, or guaranteed photorealism. High resolutions can be limited by browser/GPU memory. OBJ/FBX materials and external texture dependencies may require additional setup. Imported files are processed locally in the browser.

## Tech

- HTML/CSS/JavaScript
- Three.js
- WebGL
