Key Highlights & Features
Procedural Cosmos Shader: Direct GPU rendering using Three.js custom Simplex noise shaders,
twinkling multi-layered stars, and mouse-reactive cosmic nebula distortion.
Ultra-Smooth Drum Rolling Digits: Physical mechanical split-flap/roller simulation engineered with
hardware-accelerated CSS cubic-bezier curves and seamless 0 → 9 → 0 rollover strips.
Interactive 3D Parallax: Smooth mouse tracking using linear interpolation (lerp) giving the glass bezel
multi-axial tilt and optical depth.
Glassmorphic Display Shell: Multi-layer CSS backdrop filters ( blur(40px) saturate(170%) ), specular
rim gradients, and ambient neon separators.
Authoritative Time Synchronization: Uses JavaScript Intl.DateTimeFormat with target Asia/
Kolkata timezone, guaranteeing 100% precision across client machines worldwide.
Lightweight & Responsive: Self-contained in a single executable file with dynamic layout scaling from 4K
down to compact mobile screens.

Technology Stack
Graphics & Shaders
Three.js (r128) & GLSL: Fullscreen quad rendering
with custom fragment shaders, procedural noise
calculations, dynamic star clusters, and interactive
uniform buffers.

Typography & UI
Google Fonts & Modern CSS: Cinzel, IBM Plex Serif
(for tactile clock drums), Space Grotesk, and Plus
Jakarta Sans paired with CSS 3D perspective
transforms.

Repository Architecture
G I T H U B R E P O S I T O R Y D O C U M E N T A T I O N
India Standard Time — Cosmic Glass Edition
A high-precision digital roller clock fixed to India Standard Time (UTC+05:30), featuring procedural
WebGL cosmos shaders, layered glassmorphism, 3D mouse parallax tilt, and mechanical drum digit
physics.
Three.js r128 GLSL Shaders Timezone IST (Asia/Kolkata) Zero Build Step MIT License

•

•

•

•

•

•

├── index.html # Complete single-file application (WebGL, CSS, JS engine)
├── README.md # Project overview & documentation
└── LICENSE # MIT License terms

India Standard Time — Cosmic Glass Edition | GitHub Documentation Page 1 of 2

Quick Start & Setup
1. Clone the repository

2. Local Execution
Because there are no compile pipelines or npm dependencies required, you can test immediately:
Direct Browser Launch: Open index.html directly in any web browser supporting WebGL.
Local HTTP Server (Recommended):

Then visit http://localhost:8000 in your browser.
Configuration & Customization
Changing the Target Timezone:
Locate the clock configuration inside index.html and edit the IANA timezone string:

Modifying Parallax Sensitivity:
Adjust tilt responsiveness by modifying the rotational scale factors in the mouse event listener:

License
Released under the MIT License. Free for personal, academic, and commercial open-source projects.
