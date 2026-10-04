<div align="center">
  <br />
  <img src="public/img/logo.png" alt="Zentry Logo" width="80" />
  <h1>🎮 ZENTRY — The Metagame Layer</h1>
  <p>
    An award-winning, immersive gaming web experience featuring smooth GSAP animations, 3D tilt micro-interactions, dynamic video transitions, and cutting-edge Bento Grid design.
  </p>

  <p>
    <a href="https://zentry-archit.vercel.app" target="_blank">
      <img src="https://img.shields.io/badge/Live_Demo-Visit_Website-5724ff?style=for-the-badge&logo=vercel&logoColor=white" alt="Live Demo" />
    </a>
  </p>

  <!-- Tech Stack Badges -->
  <p>
    <img src="https://img.shields.io/badge/React_19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React 19" />
    <img src="https://img.shields.io/badge/Tailwind_CSS_v4-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS v4" />
    <img src="https://img.shields.io/badge/GSAP_3-88CE02?style=for-the-badge&logo=greensock&logoColor=white" alt="GSAP" />
    <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
    <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel" />
  </p>
</div>

---

## 🌐 Live Preview

Experience the live interactive animations, sound design, and 3D tilts directly in your browser:

🔗 **[https://zentry-archit.vercel.app](https://zentry-archit.vercel.app)**

---

## 📸 Showcase & Key Visuals

Here are two of the best-looking sections of the website:

### 1. 🎬 Cinematic Hero Section
*Featuring an interactive mini-video hover preview that expands into full screen with smooth GSAP clip-path morphing, custom typography, and floating background audio controls.*

<div align="center">
  <img src="screenshots/hero.png" alt="Zentry Hero Section" width="100%" />
</div>

<br />

### 2. 🧊 Interactive 3D Bento Grid
*A modern multi-column bento box showcasing dynamic gaming IP videos, dynamic radial gradient cursor tracking, and 3D perspective hover-tilt effects.*

<div align="center">
  <img src="screenshots/bento-grid.png" alt="Zentry Bento Grid Section" width="100%" />
</div>

> *Tip: Place your full-resolution screenshots inside the `screenshots/` folder as `hero.png` and `bento-grid.png`.*

---

## 🛠️ Tech Stack & Libraries

| Technology | Purpose |
| :--- | :--- |
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg" width="20" height="20" /> **React 19** | Component-driven architecture and state management |
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/tailwindcss/tailwindcss-original.svg" width="20" height="20" /> **Tailwind CSS v4** | Modern theme styling, `@utility` custom directives, and fluid responsive layouts |
| <img src="https://cdn.worldvectorlogo.com/logos/gsap-greensock.svg" width="20" height="20" /> **GSAP & ScrollTrigger** | High-performance timeline animations, scroll-bound transitions, and polygon clipping |
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vitejs/vitejs-original.svg" width="20" height="20" /> **Vite** | Lightning-fast development server and optimized production bundler |
| <img src="https://react-icons.github.io/react-icons/favicon.png" width="20" height="20" /> **React Icons & React-Use** | Sleek iconography and responsive window scroll hooks |
| <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vercel/vercel-original.svg" width="20" height="20" /> **Vercel** | Seamless cloud continuous deployment and global CDN hosting |

---

## ✨ Features

- **Expanding Hero Video Portal**: Seamless video switching where hovering near the center reveals the next video clip, expanding into full-screen on click.
- **GSAP ScrollTrigger Polygon Morphing**: Custom `polygon()` clip paths that smoothly scale and unmask content as the user scrolls down the page.
- **3D Bento Grid Tilt Physics**: Custom mouse coordinate calculation (`perspective(700px) rotateX(...) rotateY(...)`) for realistic tactile card tilts.
- **Floating Intelligent Navbar**: Navbar that hides on scroll down, reappears with a sleek floating pill style on scroll up, and features an interactive audio frequency visualizer.
- **Prologue / Story Interactive Mask**: Cursor-interactive floating image mask using SVG filters (`#flt_tag`) and matrix transformations.
- **Custom Font System**: Hand-tuned `@font-face` integration with **Zentry**, **Circular Web**, **General Sans**, and **Robert Medium**.

---

## 💡 What I Learnt (Key Takeaways)

- **Tailwind CSS v4 `@utility` Cascade Rules**: Transitioned from legacy `tailwind.config.js` to Tailwind v4’s `@theme` and learned how custom utilities must be declared with `@utility` so responsive modifiers (`md:col-span-1`) properly override base grid styles in the CSS cascade.
- **Complex Bento Grid Layouts**: Mastered multi-row, multi-column CSS Grid spanning (`col-span` & `row-span`) to achieve asymmetrical 2/3 and 1/3 layout proportions across responsive screen breakpoints.
- **GSAP Timeline & ScrollTrigger Orchestration**: Learned how to link scrubbed timeline animations to scroll position and execute smooth `clipPath` transitions.
- **3D Transform Math & Micro-interactions**: Computed relative mouse offsets `(event.clientX - left) / width` to apply real-time 3D rotation matrix styles without lagging the render cycle.
- **Clean React Architecture**: Structured modular, reusable components (`BentoCard`, `BentoTilt`, `Button`, `AnimatedTitle`) with clean separation of concerns.

---

## 🚀 Getting Started

Follow these steps to run the project locally on your machine:

### Prerequisites
- Node.js (v18 or higher recommended)
- npm or yarn

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/<your-username>/zentry-clone.git
   cd zentry-clone
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the local development server:**
   ```bash
   npm run dev
   ```

4. **Build for production:**
   ```bash
   npm run build
   ```

---

## 📁 Project Structure

```text
zentry-clone/
├── public/               # Static video assets, images, and custom fonts
│   ├── audio/            # Background audio loop
│   ├── fonts/            # Zentry, Circular, General Sans, Robert
│   ├── img/              # Images, masks, and swordman visual
│   └── videos/           # Hero and Bento Grid video clips (feature-1 to feature-5)
├── screenshots/          # Showcase screenshots for README
│   ├── hero.png
│   └── bento-grid.png
├── src/
│   ├── components/       # Modular UI Components
│   │   ├── About.jsx
│   │   ├── AnimatedTitle.jsx
│   │   ├── Button.jsx
│   │   ├── Contact.jsx
│   │   ├── Features.jsx   # Bento Grid with BentoTilt & BentoCard
│   │   ├── Footer.jsx
│   │   ├── Hero.jsx       # Video portal hero section
│   │   ├── Navbar.jsx     # Floating audio-reactive navbar
│   │   ├── RoundedCorners.jsx
│   │   └── Story.jsx      # Interactive image mask story
│   ├── App.jsx           # Main application entry layout
│   ├── index.css         # Tailwind v4 @theme, custom @utility rules & fonts
│   └── main.jsx
├── .gitignore            # Git exclusion rules (node_modules, dist, env, vercel)
├── package.json
└── vite.config.js
```

---

## 📄 License

This project was built for educational and portfolio purposes, inspired by the award-winning **Zentry** website.
