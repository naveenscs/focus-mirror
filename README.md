# Focus Mirror

An ambient, client-side WebGL canvas that reacts to your real-time posture and focus state using in-browser computer vision.

Focus Mirror transforms real-time posture monitoring into an interactive visual experience. Instead of intrusive pop-ups or alarms, it renders a dynamic particle field that expands, contracts, and shifts color in response to your physical alignment.

## Key Features

- **100% Client-Side Privacy:** Powered entirely by MediaPipe and WebGL inside the browser. No webcam frames, processing data, or telemetry ever leave your local machine.
- **Ambient WebGL Visualization:** Uses Three.js particle swarms to provide immediate, non-intrusive visual feedback on posture and presence.
- **Dual Tracking Modes:**
  - **Screen Mode:** Optimized for monitor-based tasks (coding, writing, typing).
  - **Book Study Mode:** Adjusts detection baselines to accommodate physical reading and desk notebook usage without triggering false posture warnings.
- **Zero Installation Required:** Download and run directly as a static file or host via GitHub Pages.

## Quick Start (Local Download)

1. Clone or download this repository.
2. Open `index.html` directly in any modern web browser (Chrome, Edge, Firefox, Safari).
3. Allow camera permissions when prompted.
4. Position your browser window on a secondary display or alongside your primary editor.

## Technical Architecture

- **Pose Detection:** `@mediapipe/pose` running locally via WASM/WebGL acceleration.
- **Graphics Pipeline:** `Three.js` (WebGL particle system rendering at 60 FPS).
- **Interface:** HTML5 / CSS3 with glassmorphic overlay controls.

## License

MIT License
