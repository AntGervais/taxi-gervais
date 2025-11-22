# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a French taxi service website for "Taxi Anthony Gervais" based in La Roche-sur-Yon (85). The site is a static marketing/landing page built with Astro 5 and Tailwind CSS 4.

## Commands

```bash
npm run dev      # Start dev server at localhost:4321
npm run build    # Build production site to ./dist/
npm run preview  # Preview production build locally
```

## Architecture

**Stack:** Astro 5, Tailwind CSS 4 (via Vite plugin), Font Awesome icons, Inter font

**Key files:**
- `src/layouts/Layout.astro` - Base HTML layout with SEO meta tags, Open Graph, and schema.org structured data
- `src/pages/index.astro` - Main landing page composing all sections
- `src/pages/success.astro` - Contact form success confirmation page
- `src/styles/global.css` - Imports Tailwind and Font Awesome

**Components** (all in `src/components/`):
- `Navbar.astro`, `Hero.astro`, `Services.astro`, `ZoneIntervention.astro`, `Testimonials.astro`, `Contact.astro`, `Footer.astro`

**Configuration:**
- `astro.config.mjs` - Site URL (https://taxi-gervais-85.fr), sitemap integration, Terser minification
- Build outputs inline stylesheets and minifies CSS/JS

## Conventions

- All content is in French
- Uses Tailwind utility classes directly in components
- Font Awesome icons via `<i class="fas fa-*">` syntax
- Yellow (`#fbbf24`) is the primary brand color (taxi theme)
