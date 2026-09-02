# Positivus — Digital Marketing Agency Landing Page

![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white)
![Sass](https://img.shields.io/badge/Sass-CC6699?style=flat&logo=sass&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![pnpm](https://img.shields.io/badge/pnpm-F69220?style=flat&logo=pnpm&logoColor=white)
[![Render Status](https://img.shields.io/badge/Render-46E3B7?style=flat&logo=render&logoColor=white)](https://sz-positivus.onrender.com/)

A modern, responsive, and pixel-perfect landing page for the **Positivus** digital marketing agency, built with [Vite](https://vite.dev) and modern SCSS architecture, optimized for performance, accessibility, and clean component structure.

## ✨ Features

- **High-Performance Architecture**: Lightning-fast development and optimized production bundling powered by Vite 8 with zero heavy runtime dependencies.
- **Modern Modular SCSS**:
  - Organized using SASS 7-1 pattern principles with modern `@use` / `@forward` module system.
  - CSS custom properties (design tokens for colors, borders, radii, shadows, and spacing).
  - Fluid typography scaling via `clamp()` mixins (`fluid-text`) across viewport widths.
  - Custom branded scrollbar and text `::selection` highlighting.
- **Interactive UI Components & Micro-interactions**:
  - **Native `<dialog>` Mobile Navigation**: Lightweight drawer modal menu with accessible toggle and smooth cross-browser backdrop.
  - **Expandable Working Process Accordion**: Interactive `<details>` & `<summary>` implementation with custom plus/minus status indicators and smooth state transitions.
  - **Responsive Reviews Slider Layout**: Testimonials quote bubbles with custom star-rating indicators and interactive navigation pagination.
  - **Interactive Micro-states**: Branded `:hover` transitions and tactile `:active` micro-scale (`0.97`) click feedback for buttons.
  - **Custom Form Controls**: Styled radio buttons, fluid form inputs, and textarea with floating submit action.
- **Semantic HTML5 & Accessibility (A11y)**:
  - WAI-ARIA considerations with `.visually-hidden` screen-reader helper classes.
  - Full keyboard accessibility and focus management.
  - Responsive SVG icons and local high-speed `@font-face` WOFF2 fonts (`Space Grotesk`).
- **Complete Landing Page Sections**:
  - **Header & Navigation**: Brand logo, desktop navigation menu, CTA button, and mobile burger dialog.
  - **Hero Section**: Value proposition headline, call to action, vector illustration, and client logos ticker (Amazon, Dribbble, HubSpot, Notion, Netflix, Zoom).
  - **Services Grid**: 6 distinct marketing service cards (SEO, PPC, SMM, Email, Content, Analytics) with adaptive color schemes and visual indicators.
  - **CTA Banner**: Highlighted conversion block with customized graphic background.
  - **Case Studies**: Real-world client case study cards with interactive exploration links.
  - **Our Working Process**: 6-step numbered accordion showcasing agency workflow and methodologies.
  - **Team Showcase**: Team member profiles with roles, experience blurbs, and LinkedIn badges.
  - **Testimonials**: Branded quote cards with pagination controls.
  - **Contact Us**: Interactive consultation request form with radio mode switch.
  - **Footer**: Unified navigation, subscription form card, social channels, and copyright notice.

## 🛠️ Tech Stack

- **Bundler / Build Tool**: [Vite 8](https://vite.dev)
- **Styling**: [Sass (SCSS)](https://sass-lang.com/) (Modules, Mixins, Media queries, BEM methodology, CSS Variables)
- **Markup**: Semantic [HTML5](https://developer.mozilla.org/en-US/docs/Web/HTML)
- **Typography**: Local Space Grotesk (WOFF2)
- **Package Manager**: [pnpm](https://pnpm.io/)
- **Deployment**: [Render](https://render.com/) (Live: [sz-positivus.onrender.com](https://sz-positivus.onrender.com/))

## 🚀 Getting Started

### Prerequisites

Ensure you have [Node.js](https://nodejs.org/) installed:
- **Node.js**: `>= 20.0.0`
- **pnpm**: `>= 9.0.0` (or `npm` / `yarn`)

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/verosabyrka/positivus.git
   cd positivus
   ```

2. **Install dependencies**:
   ```bash
   pnpm install
   ```

3. **Start the development server**:
   ```bash
   pnpm dev
   ```
   Open [http://localhost:5173](http://localhost:5173) in your browser to view the project.

## 🧞 Available Scripts

| Command | Action |
| :--- | :--- |
| `pnpm dev` | Starts local development server at `localhost:5173` |
| `pnpm build` | Compiles and optimizes assets for production into `./dist/` |
| `pnpm preview` | Locally previews the production build before deployment |

## 📂 Project Structure

```text
positivus/
├── public/                 # Static assets (favicons, images, logos, partners, team)
├── src/
│   ├── assets/             # Bundled assets (fonts, background vectors)
│   ├── styles/             # Modular SCSS stylesheets
│   │   ├── base/           # Fonts, global resets, variables, normalization
│   │   ├── components/     # UI components (buttons, cards, forms, dialogs)
│   │   ├── helpers/        # Mixins, media query helpers, functions
│   │   ├── layouts/        # Layout grid system, section containers
│   │   └── sections/       # Landing page sections (hero, services, process, etc.)
│   └── main.js             # Application entry point
├── index.html              # Landing page HTML entry point
├── jsconfig.json           # Path alias configuration
├── package.json            # Project dependencies and npm scripts
└── vite.config.js          # Vite build tool configuration
```
