## Overview

Wandor is an intelligent travel planning platform that transforms how people plan trips. Simply tell our AI where you're going and what you love — it generates a fully personalized itinerary tailored to your preferences, pace, and travel style.

This repository contains the landing page built as a single-page application with a cinematic hero section, frosted-glass UI components, and a seamless user experience.

## Tech Stack

Technology	Purpose
React 19	UI component library
TypeScript	Type-safe JavaScript
Vite 6	Lightning-fast dev server & bundler
Tailwind CSS	Utility-first styling framework
lucide-react	Icon library
Fonts
Geist (sans-serif) — Body & UI text
Special Elite (serif) — Logo wordmark only

## project Structure

FemCare/
├── public/
│ └── favicon.svg
├── src/
│ ├── components/
│ │ └── Hero.tsx # Full landing page (nav, hero, glass card)
│ ├── App.tsx # Root component
│ ├── main.tsx # Entry point
│ └── index.css # Tailwind directives + global styles
├── index.html # HTML shell with Google Fonts
├── tailwind.config.js # Custom theme (colors, fonts)
├── postcss.config.js # PostCSS with Tailwind + Autoprefixer
├── vite.config.ts # Vite config with @/ path alias
├── tsconfig.json # TypeScript project references
├── tsconfig.app.json # App-specific TS config
├── tsconfig.node.json # Node-specific TS config
├── package.json
└── .gitignore

text


---

## Features

- **Cinematic Hero Section** — Full-viewport background video with a white-to-transparent gradient overlay for text legibility
- **Frosted-Glass Prompt Card** — Liquid-glass effect using `backdrop-blur`, low-opacity fills, and thick translucent borders
- **Responsive Navigation** — Desktop nav with centered links, auto-hides on mobile with adaptive spacing
- **Micro-Interactions** — Hover opacity transitions, active scale feedback, upload button hover animation
- **File Upload** — Hidden file input triggered by a frosted-glass upload button (accepts images & PDFs)
- **Mobile-First Responsive** — Breakpoint at 768px with fluid typography via `clamp()`

---

## Getting Started

### Prerequisites
- **Node.js** ≥ 18
- **npm** ≥ 9

### Installation

```bash
git clone https://github.com/vaishnavi-shukla-cs/FemCare_AI.git
cd FemCare_AI
npm install
Development
bash

npm run dev
Opens at http://localhost:5173

Production Build
bash

npm run build
npm run preview
Customization
Colors
Edit the wandor color palette in tailwind.config.js:

js

colors: {
  wandor: {
    dark: '#0a0a0a',
    text: '#1a1a1a',
    muted: '#767676',
    prompt: '#905831',
  },
}
Fonts
Replace the Google Fonts link in index.html and update tailwind.config.js:

js

fontFamily: {
  sans: ['YourFont', 'sans-serif'],
  display: ['YourDisplayFont', 'serif'],
}
Background Video
Change the src attribute on the <video> tag in src/components/Hero.tsx.

Team
Member
Role
Utkarsh Gupta	Team Leader
Vaishnavi Trivedi	Developer
Vaishnavi Shukla	Developer
Tanisha Sharma	Developer

Team ID: 26_CS_AI_3C_02
Department of Artificial Intelligence — Pranveer Singh Institute of Technology, Kanpur
Guide: Mr. Gaurav Singh, Assistant Professor
