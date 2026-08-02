# Nelson Martinel — Portfolio

My personal portfolio website, built with [Astro](https://astro.build). Showcases who I am, my projects, and how to get in touch.

**Live site:** [[Deployed with Netlify](https://nelson-martinel-portofolio.netlify.app/)]

---

## ✨ Features

- **Light / dark theme** — animated sun/moon toggle in the nav, theme preference saved to `localStorage` and respected on load (no flash of wrong theme)
- **triangle corners background** — triangle lines allong the borders of my background
- **Bento-style "Who I am" grid** — tilt-on-hover cards, an animated ticker, and a live-rendered 3D graduation cap (`<model-viewer>`) that follows your cursor
- **Live LeetCode stats** — fetched at build time from the LeetCode stats API and displayed on the home page
- **Infinite tech/language carousels** — auto-scrolling chip lists, pausable on hover
- **Draggable project carousel** — snap-to-center cards that expand to show description, stack, what I learned, and links; falls back to a simple tap-to-expand grid on mobile
- **Contact form** — client-side validated, opens a pre-filled `mailto:` link (no backend required)
- Fully responsive, with reduced-motion support for accessibility
- **SEO optimizations** This project incorporates structured layout components (like Base.astro with meta tags) and performance-focused practices such as responsive design and reduced-motion support. Additionally, deployment on a global CDN (Netlify) enhances page speed and accessibility, which are key ranking factors.

## 🛠️ Tech Stack

- [Astro](https://astro.build) — static site framework / file-based routing
- TypeScript
- Vanilla CSS (custom properties for theming, no framework)
- [`<model-viewer>`](https://modelviewer.dev/) for the 3D graduation cap
- [LeetCode Stats API](https://leetcode-stats.tashif.codes/) for coding stats
- Deployed on Netlify

## 📁 Project Structure

```
my-portofolio/
├── .astro/
├── .vscode/
├── node_modules/
├── public/              # static assets (images, favicon, 3D model, etc.)
├── src/
│   ├── images/
│   ├── layouts/
│   │   └── Base.astro   # shared layout: <head>, nav, theme toggle, footer
│   ├── lib/
│   └── pages/
│       ├── index.astro      # home page
│       ├── projects.astro   # projects carousel
│       └── contact.astro    # contact page + form
├── .env
├── .gitignore
├── astro.config.mjs
├── package.json
├── package-lock.json
├── README.md
└── tsconfig.json
```

### Key files

| File | Purpose |
|---|---|
| `src/layouts/Base.astro` | Shared page shell — meta tags, fonts, aurora background, nav bar, animated theme toggle, footer |
| `src/pages/index.astro` | Hero section, "Who I am" bento grid, tech/language carousels, experience timeline, LeetCode stats, social links |
| `src/pages/projects.astro` | Draggable/snapping project carousel with expandable cards |
| `src/pages/contact.astro` | Contact info cards + validated contact form |

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org) (LTS recommended)
- npm (or your package manager of choice)

### Installation

```bash
# Clone the repo
git clone https://github.com/Nelson-Mart/Portofolio.git
cd Portofolio

# Install dependencies
npm install
```

### Development

```bash
npm run dev
```

Opens the site locally, usually at `http://localhost:4321`.

### Build

```bash
npm run build
```

Outputs a production-ready static site to `dist/`.

### Preview production build

```bash
npm run preview
```

## 🌐 Deployment

This project is deployed on [Netlify](https://nelson-martinel-portofolio.netlify.app/). Pushing to the main branch triggers an automatic build and deploy.

## 📬 Contact

- **Email:** nelsonmartinel2@gmail.com
- **LinkedIn:** [nelson-martinel](https://linkedin.com/in/nelson-martinel-529546358)
- **GitHub:** [@Nelson-Mart](https://github.com/Nelson-Mart)
- **Instagram:** [@Nelson-Mart](https://www.instagram.com/nelsonmcoding/)

---

© 2026 Nelson Martinel