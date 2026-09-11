⏳ India Standard Time — Cosmic Glass Edition
A modern, high-precision digital roller clock fixed to India Standard Time (UTC+05:30). Built with procedural WebGL cosmic shaders, layered glassmorphism, dynamic 3D mouse parallax, and mechanical drum-style digit transitions.

✨ Features
Procedural Cosmos Shader: Runs entirely on GPU via Three.js with Simplex noise, interactive star layers, twinkling effects, and mouse-driven nebula displacement.

Ultra-Smooth Rolling Digits: Split mechanical roller drum simulation using dynamic CSS cubic-bezier transitions and endless strip resets (0 → 9 → 0).

Interactive 3D Parallax: Mouse tracking gives the central glass enclosure realistic perspective tilt and depth.

Glassmorphic UI: Multi-layered CSS backdrop filters, specular highlights, radial rim lighting, and dual-tone glowing neon separators.

Strict Timezone Lock: Calculates exact IST via native JavaScript Intl.DateTimeFormat across all devices, regardless of local client time.

Fully Responsive: Fluid scaling from high-resolution desktop monitors down to mobile viewports.

Zero Build Step: Native vanilla HTML, CSS, and JS using Three.js via CDN.

🚀 Live Demo
Check out the live deployment directly via GitHub Pages:

View Live Demo (Replace with your GitHub Pages URL)

🛠️ Tech Stack
Three.js (r128): Fullscreen canvas rendering with custom Vertex and Fragment shaders.

GLSL: Procedural 2D Simplex noise, coordinate warping, dynamic star hashing.

Vanilla CSS3: Perspective transforms, flexbox/grid architecture, backdrop blur (saturate, blur), and gradient text clipping.

Vanilla JavaScript (ES6+): Interval orchestration, Intl time formatting, DOM roller strip offsets, and linear interpolation (lerp) parallax loops.

Google Fonts:

Cinzel (Kicker & accents)

IBM Plex Serif (Roller digits)

Space Grotesk (Date & metadata)

Plus Jakarta Sans (Body base)

📂 Project Structure
Plaintext
├── index.html        # Complete application (markup, styles, WebGL shaders & engine)
└── README.md         # Documentation
💻 Quick Start
1. Clone the repository
Bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
2. Run locally
Because there are no compile steps or dependencies to install, you can run this immediately:

Option A: Direct Open
Double-click index.html to open it in any modern web browser.

Option B: Local Server (Recommended for shaders)
Using Python:

Bash
python3 -m http.server 8000
Or using Node.js:

Bash
npx serve
Visit http://localhost:8000 in your browser.

⚙️ Customization
Change Timezone
To change the clock from IST to another timezone, open index.html and update the IST_TZ variable inside the clock script:

JavaScript
const IST_TZ = 'America/New_York'; // e.g., 'UTC', 'Europe/London', 'Asia/Tokyo'
Adjust Parallax Intensity
Tweak the tilt range by adjusting the mouse multiplier inside the mousemove listener:

JavaScript
targetRY = px * 7; // Horizontal rotation range
targetRX = -py * 5; // Vertical rotation range
📄 License
Distributed under the MIT License. See LICENSE for more information.
