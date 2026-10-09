# RoomSpace — VR Interior Design Studio

RoomSpace is a browser-based 3D interior design demo built with **Three.js**, **Vite**, and optional **WebXR** support. No Unity or backend is required.

## Features

- Fully interactive 3D living room
- Orbit, zoom, and pan camera controls
- Select and drag supported furniture around the room
- Change wall, sofa, and furniture accent colors
- Toggle room lighting
- Save and restore a room layout in your browser
- Reset the room to its original arrangement
- Optional VR entry button on compatible devices/browsers
- Responsive desktop and mobile interface
- MIT licensed

## Run locally

**Requirements:** Node.js 20.19+ or 22.12+ recommended.

```bash
npm install
npm run dev
```

Open the local URL shown in the terminal, usually `http://localhost:5173`.

## Build

```bash
npm run build
npm run preview
```

Vite writes production files to `dist/`.

## Controls

- Drag empty space to orbit around the room.
- Scroll or pinch to zoom.
- Use the right mouse button (or two-finger drag where supported) to pan.
- Click a furniture item or its list entry to select it.
- Drag selected movable furniture on the floor to reposition it.
- Use the color swatches to customize the room.
- **Save design** stores the current furniture positions and color choices in this browser.
- **Load design** restores the last locally saved design.
- **Reset room** returns furniture and colors to the original design.

## VR compatibility

WebXR immersive VR depends on the browser, headset, and device. A secure origin is usually required for deployed websites; `localhost` is treated as a secure origin for development. If VR is unavailable, the desktop 3D viewer remains usable.

## Deploy

This is a standard Vite site and can be deployed to Vercel, Netlify, or GitHub Pages. Follow the hosting provider's instructions for Vite projects.

## Project structure

```text
vr-interior-design-viewer/
├── src/
│   ├── main.js
│   └── style.css
├── index.html
├── package.json
├── README.md
├── LICENSE
└── .gitignore
```

## Notes

- This is a visual design prototype, not a professional architectural measurement tool.
- Layout saving uses browser `localStorage`; it does not sync between devices.
- 3D objects are procedurally built with Three.js, so the starter project does not depend on external model files.

## License

MIT
