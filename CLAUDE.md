# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a fashion designer portfolio website - a single-page HTML/CSS/JavaScript application with no build system or dependencies. The entire site is contained in `portfolio.html` with inline CSS and JavaScript.

## Running the Project

Open `portfolio.html` directly in a browser, or serve via any static server:
```bash
python -m http.server
```

Deploy to any static hosting (GitHub Pages, Netlify, Vercel) - no build step required.

## Architecture

**Single-file structure:**
- `portfolio.html` - All markup, styles (~550 lines CSS), and scripts (~155 lines JS)
- `Finished/` - Image assets for completed works
- `Sketches/` - Image assets for design sketches

**JavaScript architecture:**
- `galleries` object holds image arrays for three sections: designs, artworks, sketches
- `imagesPerLoad` controls pagination (default: 6)
- `createPortfolioItem()` - Creates gallery item DOM elements
- `loadMoreImages()` - Handles "Load More" pagination
- Uses Intersection Observer API for scroll-triggered animations

**CSS architecture:**
- CSS custom properties for theming (`--color-sand`, `--color-charcoal`, etc.)
- CSS Grid for responsive gallery layouts (3-column, auto-fit)
- Mobile breakpoint at 768px

## Key Customization Points

**In portfolio.html:**
- Line ~487: Logo/name in navigation
- Line ~499: Hero section name
- Lines ~543-544: Contact email and phone
- Line ~551: Footer copyright
- Lines ~557-572: Gallery image arrays in JavaScript

## Image Handling

- Supported formats: JPG, PNG, GIF, WebP
- HEIC files in assets directories need conversion for browser compatibility
- Add images by pushing paths to `galleries.designs`, `galleries.artworks`, or `galleries.sketches` arrays
