# CAMERA

## Interactive 3D Camera Anatomy

A bilingual interactive educational experience for exploring the anatomy and functionality of a professional filmmaking camera.

**Created by Amir Saeid Dehghan**

### Features
- Original detailed modular cinema camera with machined surfaces, optics, lens gearing, monitor, controls, cooling and connectors.
- 24 individually selectable educational components, including a keyboard-accessible component list.
- Hand-authored English and Persian explanations with full RTL support.
- Smooth, reversible exploded view. Components remain selectable while separated.
- Damped orbit, wheel/pinch zoom, animated reset and optional auto rotation.
- Studio lighting, PBR materials, subtle material highlights and responsive layout.
- Reduced-motion preference, startup/error states and local asset bundling.

### Technology
Three.js, OrbitControls, RoomEnvironment, rounded and lathed mesh geometry, HTML/CSS, JavaScript ES modules, Vite. No server or API keys.

### Controls
Drag to orbit; scroll or pinch to zoom; click/tap a part to inspect it. The component list also supports keyboard navigation. Choose EN or فارسی. Explode separates the assemblies; Assemble returns each part to its stored original transform. Reset view restores framing without changing assembly state. Escape closes the information panel. User interaction pauses auto rotation.

### Development
Requires Node.js 22 or newer.

```sh
npm ci
npm run dev
npm run build
npm run preview
```

### GitHub Pages deployment
The workflow builds `dist` and deploys with GitHub Actions. In repository Settings → Pages, select **GitHub Actions** as the source if it has not been enabled. Relative asset paths support the `/Camera/` project URL.

Expected URL: https://saaeiddev.github.io/Camera/

### Educational scope
C–01 is an original composite cinema-camera design, not a replica of a commercial camera or a repair/disassembly manual. The internal sensor and cooling assemblies are simplified for learning; part separation illustrates functional relationships, not a physical service sequence. Focus, zoom and iris rings are inspection objects rather than optical simulators. The LCD displays an original illustrative preview, not an actual sensor feed.

### Asset credits
Camera geometry, surface noise and LCD illustration are generated locally from original project code. No third-party camera mesh or photography is used. Three.js is MIT licensed (license in its package). Typography: Manrope and Vazirmatn via Google Fonts, under the SIL Open Font License; system fallbacks remain available when external fonts cannot load.
