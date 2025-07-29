# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML website for Sixmilebridge, County Clare, Ireland - a community website showcasing the town's history, local businesses, and events. The site uses vanilla HTML5, CSS3, and minimal JavaScript with no build system or dependencies.

## Architecture

**Static Website Structure:**
- 4 main HTML pages: `index.html` (homepage), `community.html`, `business.html`, `events.html`
- Single comprehensive CSS file: `styles.css` 
- Minimal vanilla JavaScript for mobile navigation toggle
- SEO optimized with sitemap.xml, robots.txt, and structured JSON-LD data

**Design System:**
- Irish green color theme (#1a472a primary, #2d5a3d secondary, #4a7c59 accent)
- Responsive mobile-first design using CSS Grid and Flexbox
- Semantic HTML5 markup throughout
- Accessibility features (focus styles, reduced motion support)

**Key Files:**
- `styles.css:1-50` - CSS reset and typography system with Irish green theme
- `index.html:24-47` - Structured data (JSON-LD) for SEO
- All HTML pages include comprehensive meta tags and Open Graph data

## Development Commands

**No build system required** - this is a static website that can be:
- Opened directly in browser for development
- Deployed to any web server without compilation
- Edited with any text editor

**Local Development:**
```bash
# Serve locally (if Python available)
python -m http.server 8000

# Or use any static file server
npx serve .
```

**Validation:**
```bash
# Validate HTML (if w3c validator available)
html5validator *.html

# Check links (if linkchecker available) 
linkchecker index.html
```

## Content Guidelines

**Irish Community Focus:**
- All content relates to Sixmilebridge town and County Clare
- Irish language names included where appropriate (e.g., "Droichead na Sé Míle")
- Local business directory and community events are key features
- Geographic coordinates: 52.7447°N, 8.7717°W

**SEO Requirements:**
- Update sitemap.xml when adding new pages
- Include structured data (JSON-LD) for location/business information
- Maintain consistent meta descriptions and titles
- Use semantic HTML5 elements (header, nav, main, section, article, footer)

## Technical Notes

**CSS Architecture:**
- Single CSS file with organized sections (reset, typography, layout, components, responsive)
- CSS custom properties used for consistent theming
- Mobile-first responsive design with desktop breakpoints
- Grid and Flexbox layouts throughout

**JavaScript Usage:**
- Minimal vanilla JS only for mobile menu toggle
- No external libraries or frameworks
- Keep functionality lightweight for fast loading

**Browser Support:**
- Modern CSS features (Grid, Flexbox, custom properties)
- Graceful degradation for older browsers
- No IE support assumed