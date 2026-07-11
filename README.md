# iPhone 15 Pro — Animated Landing Page Clone

A pixel-focused recreation of Apple's iPhone 15 Pro product page, built to practice scroll-driven animation, 3D product visualization, and responsive landing-page design.

## Overview

This project rebuilds Apple's iPhone 15 Pro marketing page as a single-page React application. It focuses on the same techniques real landing pages rely on: scroll-triggered motion, a 3D hero model, and layout that holds up cleanly across devices.

## Tech Stack

- **React** (Vite) — component structure and state
- **GSAP** (GreenSock) — scroll-triggered timelines and micro-interaction animations
- **Three.js** — interactive 3D model rendering for the product hero section
- **Tailwind CSS** — utility-first responsive styling

## Features

- Scroll-triggered GSAP animation timelines synced to page sections
- Interactive 3D iPhone model rendered with Three.js, with camera/rotation controls
- Fully responsive layout across mobile, tablet, and desktop breakpoints
- Section-by-section reveal animations mirroring Apple's original product page feel

## Notable Technical Work

- Migrated the styling layer from **Tailwind CSS v3 to v4**, resolving breaking changes in class behavior and config structure to keep the design system stable
- Updated integration with **Sentry v8**, adapting to its revised initialization and error-tracking API
- Tuned initial load performance by optimizing 3D asset loading and animation trigger timing

## Getting Started

```bash
# Clone the repository
git clone <repo-url>
cd iphone-15-pro-clone

# Install dependencies
npm install

# Run the development server
npm run dev
```

The app will be available at `http://localhost:5173` by default (Vite's default port).

## Build

```bash
npm run build
```

Outputs a production-ready build to the `dist/` folder.

## Folder Structure (typical)

```
├── src/
│   ├── components/     # Section components (Hero, Highlights, Model, Footer, etc.)
│   ├── assets/         # Images, 3D models, textures
│   ├── App.jsx
│   └── main.jsx
├── public/
├── tailwind.config.js
├── vite.config.js
└── package.json
```

## What This Project Demonstrates

- Building animated, landing-page-style UI with GSAP
- Working with 3D rendering in the browser via Three.js
- Responsive, utility-first design with Tailwind CSS
- Handling real-world dependency/version migration issues (Tailwind v3→v4, Sentry v8)
