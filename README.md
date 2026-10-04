<div align="center">
  <img src="public/img/logo.png" alt="Zentry Logo" width="70" />
  <h1>Zentry Clone</h1>
  <p>
    A frontend recreation of the Zentry website built with React 19, Tailwind CSS v4, and GSAP. Features scroll-triggered animations, interactive video reveals, and 3D card tilt effects.
  </p>

  <p>
    <a href="https://zentry-archit.vercel.app" target="_blank">
      <img src="https://img.shields.io/badge/Live%20Demo-View%20Site-5724ff?style=for-the-badge&logo=vercel&logoColor=white" alt="Live Demo" />
    </a>
  </p>

  <p>
    <img src="https://img.shields.io/badge/React%2019-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React 19" />
    <img src="https://img.shields.io/badge/Tailwind%20CSS%20v4-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS v4" />
    <img src="https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=white" alt="GSAP" />
    <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
    <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Vercel" />
  </p>
</div>

---

## Live Demo

Website: **[https://zentry-archit.vercel.app](https://zentry-archit.vercel.app)**

---

## Screenshots

### Hero Section
Center hover mini-player that expands into a full screen video transition on click, with clip-path scaling and audio controls.

<div align="center">
  <img src="screenshots/hero.png" alt="Hero Section" width="100%" />
</div>

<br />

### Bento Grid
Multi-card responsive bento layout with auto-playing video cards and mouse-tracking 3D tilt interaction.

<div align="center">
  <img src="screenshots/bento-grid.png" alt="Bento Grid" width="100%" />
</div>

---

## Tech Stack

- **React 19**: Component structure, refs, and state management
- **Tailwind CSS v4**: Theme styling, custom `@utility` classes, and responsive design
- **GSAP & ScrollTrigger**: Scroll animations, timelines, and clip-path transitions
- **Vite**: Build tool and local development
- **React Icons & react-use**: Icons and scroll position tracking
- **Vercel**: Deployment and hosting

---

## Features

- **Expanding Video Hero**: Hovering over the center shows a preview of the upcoming video, clicking expands it to full screen using GSAP clip-path animations.
- **Bento Grid**: Asymmetric grid layout that adjusts between mobile and desktop with hover tilt physics based on cursor position.
- **Scroll Animations**: Elements reveal and scale as you scroll down using GSAP ScrollTrigger.
- **Interactive Story Section**: Image mask that shifts and tilts with mouse movement.
- **Navbar with Audio**: Floating navigation bar that hides on scroll-down, reappears on scroll-up, and includes background audio with an animated equalizer indicator.
- **Custom Typography**: Custom fonts (Zentry, Circular Web, General Sans, and Robert Medium) loaded locally via `@font-face`.

---

## What I Learned

- **Tailwind v4 utility priority**: How Tailwind v4 handles the cascade with custom classes. Defining custom CSS rules with `@utility` is necessary so responsive modifiers like `md:col-span-1` can override base grid spans without getting blocked by specificity or source order.
- **CSS Grid spanning**: Building asymmetrical layouts using `col-span` and `row-span` combinations that look good on both mobile (stacked) and desktop (2-column bento).
- **GSAP ScrollTrigger**: Connecting scroll position directly to timeline tweens and coordinating `clip-path` polygon morphs.
- **Mouse coordinate math**: Calculating element bounds with `getBoundingClientRect()` to produce real-time 3D tilt styles (`rotateX` / `rotateY`) on card hover.
- **Video preloading and state synchronization**: Managing multiple HTML5 video elements in React, handling loading states, and keeping active indices in sync.

---

## Getting Started

### Prerequisites
- Node.js (v18+)
- npm

### Run Locally

1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/zentry-clone.git
   cd zentry-clone
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start dev server:
   ```bash
   npm run dev
   ```

4. Build for production:
   ```bash
   npm run build
   ```

---

## Project Structure

```text
zentry-clone/
├── public/
│   ├── audio/
│   ├── fonts/
│   ├── img/
│   └── videos/
├── screenshots/
│   ├── hero.png
│   └── bento-grid.png
├── src/
│   ├── components/
│   │   ├── About.jsx
│   │   ├── AnimatedTitle.jsx
│   │   ├── Button.jsx
│   │   ├── Contact.jsx
│   │   ├── Features.jsx
│   │   ├── Footer.jsx
│   │   ├── Hero.jsx
│   │   ├── Navbar.jsx
│   │   ├── RoundedCorners.jsx
│   │   └── Story.jsx
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
├── .gitignore
├── package.json
└── vite.config.js
```
