# Paper Straw Texture Preview Tool

This project provides a web-based 3D visualization tool for previewing paper straw textures. It was developed as a custom feature for a client to help showcase how printed designs will appear on spiral-wrapped paper straws.

Live Preview: [https://ristic99.github.io/paperstrawpreview/](https://ristic99.github.io/paperstrawpreview/)

## Features

- Realistic spiral geometry simulating a rolled paper straw
- Texture upload interface for custom design previews
- Interactive 3D preview with mouse-based rotation and zoom
- Sample texture assets included (`texture.png` and `texture.psd`)

## How It Works

The script uses [Three.js](https://threejs.org/) to render a 3D spiral mesh and apply image textures to its surface.

### Geometry and Wrapping

- The mesh simulates a continuous paper ribbon spirally wrapped around a cylindrical form.
- Parameters used:
  - Straw length: 28.5 units
  - Straw diameter: 0.8 units
  - Wrapping follows a 45-degree diagonal spiral pattern
- A flat plane geometry is mathematically deformed into a helical ribbon structure using trigonometric transformations.

### Texture Mapping

- Users can upload image files via an HTML file input.
- The uploaded image is converted into a Three.js texture and mapped to the spiral mesh.
- Texture wrapping and rotation are applied to simulate how the design wraps around the straw.

### Controls

- Rotate the straw by dragging horizontally with the mouse
- Zoom in/out using the mouse scroll wheel

## Files

| File             | Description                               |
|------------------|-------------------------------------------|
| `index.html`| Main HTML and JavaScript for visualization |
| `texture.png`    | Example texture for testing                |
| `texture.psd`    | Editable Photoshop file for custom designs |

## Usage Instructions

1. Open `paperstrawpreview.html` in a web browser (no server needed).
2. Use the "Load texture" input at the top-left corner to upload your image.
3. The 3D model will update in real time with your uploaded texture.
4. Use mouse controls to rotate or zoom the preview.

## Project Purpose

This feature was developed for a client who needed a way to preview straw textures before production. It enables their customers to visualize how a printed design will appear when spirally wrapped around a paper straw, improving the design approval workflow and reducing misunderstandings during manufacturing.

## Dependencies

- [Three.js](https://threejs.org/) (via CDN, version r115)
- No build tools required — works as a standalone HTML file in any modern browser

## License

This project was developed for a specific client use case and may be subject to usage restrictions. Contact the author for licensing or reuse inquiries.
