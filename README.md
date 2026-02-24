# Gallery Site

An interactive photo gallery website featuring a draggable grid layout with lightbox image viewing.

## Features

- **Draggable gallery** – drag and fling the image grid using GSAP Draggable with inertia physics
- **Lightbox viewer** – click any image to open it full-screen via PhotoSwipe
- **Loading animation** – smooth zoom-in reveal after images finish loading
- **Dark mode** – automatically adapts to the system color scheme
- **Webpack build** – separate development and production configurations

## Tech Stack

| Library | Purpose |
|---|---|
| [GSAP](https://greensock.com/gsap/) + Draggable + InertiaPlugin | Drag-and-fling interaction |
| [PhotoSwipe](https://photoswipe.com/) | Lightbox / full-screen image viewer |
| [Webpack 5](https://webpack.js.org/) | Module bundler |

## Project Structure

```
gallerySite/
├── css/
│   └── style.css          # Main stylesheet (dark mode, gallery layout, animations)
├── img/                   # Gallery images (1.jpg – 20.jpg)
├── js/
│   └── app.js             # Gallery initialization (Draggable + PhotoSwipe)
├── libs/                  # Vendored libraries (GSAP, PhotoSwipe)
├── index.html             # Entry HTML
├── webpack.common.js      # Shared Webpack config
├── webpack.config.dev.js  # Development config (source maps, live reload)
└── webpack.config.prod.js # Production config
```

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) 16+
- npm

### Installation

```bash
npm install
```

### Development

Starts a local dev server with live reload:

```bash
npm start
```

### Production Build

Outputs bundled files to the `dist/` directory:

```bash
npm run build
```

## Usage

Open the site in a browser:

- **Drag** anywhere on the gallery to pan around the image grid.
- **Click** an image to open it in the full-screen PhotoSwipe lightbox.
- Use the lightbox arrows or keyboard to navigate between images.
