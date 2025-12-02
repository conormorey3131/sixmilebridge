# Sixmilebridge Community Website - Repository Documentation

## Project Overview

A static HTML website for **Sixmilebridge (Droichead na Sé Míle)**, County Clare, Ireland. This community-focused website showcases the town's history, local businesses, community resources, and upcoming events.

**Location**: 52.7447°N, 8.7717°W  
**Technology Stack**: Pure HTML5, CSS3, Vanilla JavaScript  
**Build System**: None (static site)  
**Dependencies**: None

## Repository Structure

### Core HTML Pages (5 files)
- `index.html` - Homepage with hero section, welcome content, and quick links
- `community.html` - Community resources, local amenities, schools, and clubs
- `business.html` - Local business directory with interactive map
- `events.html` - Upcoming events and community calendar
- `privacy.html` - Privacy policy and data protection information

### Styling & Scripts
- `styles.css` - Comprehensive stylesheet with Irish green theme (#1a472a primary)
- `sw.js` - Service worker for offline functionality and caching

### SEO & Configuration
- `sitemap.xml` - XML sitemap for search engines
- `robots.txt` - Search engine crawling directives
- `site.webmanifest` - Progressive Web App manifest
- `CLAUDE.md` - AI assistant guidance for code maintenance

### Images & Assets (37 files)

#### Logos & Icons
- `STT Logo.svg` - Sixmilebridge Town Team vector logo
- `STT R1.png` - Site favicon/icon
- `Sixmilebridge Town Team Logo Black Text.png`
- `Sixmilebridge Town Team Logo White Text.png`
- `favicon.png`, `favicon-16x16.png`, `favicon-32x32.png`
- `apple-touch-icon.png`

#### Partner/Sponsor Logos
- `Clare County Council Logo.jpg`
- `Our Rural Future Logo.jpg`
- `Project Ireland 2040 Logo.jpg`
- `Town Centre First Logo.jpg`
- `SFCU Logo Large.PNG` - Sixmilebridge & Feakle Credit Union
- `Morey_Digital_logo.jpg`

#### Business Logos & Images
- `barknboard_logo.png`, `barknboard_image.png`
- `cozy_logo.jpg`, `cozy_picture.jpg`
- `kv_logo.jpg`

#### Photography & Hero Images
- `welcome.jpg`, `welcome2.jpg` - Welcome/hero images
- `barber.jpg` - Barber shop image
- `ducks.jpg` - Local wildlife
- `old.jpg` - Historical photo
- `tidy_towns_award_2025.png` - Tidy Towns award

#### Stock Photography (Unsplash)
- `ashleigh-joy-photography-BdEgT847nk0-unsplash.jpg`
- `dennis-van-dalen-fuiCJCUM-Yc-unsplash.jpg`
- `dylan-gillis-KdeqA3aTnBY-unsplash.jpg`
- `john-cameron--_5IRj1F2rY-unsplash.jpg`
- `k-mitch-hodge-14KNdf70poU-unsplash.jpg`
- `magdalena-smolnicka-gBMmLzK5tuw-unsplash.jpg`
- `mark-de-jong-QNPv8NXIJ8U-unsplash.jpg`
- `shane-rounce-DNkoNXQti3c-unsplash.jpg`
- `thomas-tucker-2ZWVhuUYMZo-unsplash.jpg`

#### Event Materials
- `Copy of Bold Creative Quiz Night Poster.png` - Event poster

## Technical Architecture

### Design System
- **Color Palette**:
  - Primary: #1a472a (Irish Green)
  - Secondary: #2d5a3d
  - Accent: #4a7c59
  - CTA: #ff6b35 (Orange)
  - Background: #fdfdfd
  - Text: #444

- **Typography**:
  - Font Stack: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
  - Base Font Size: 16px
  - Line Height: 1.6
  - Headings: 700 weight, 1.3 line-height

- **Layout**:
  - Max Container Width: 1200px
  - Mobile-First Responsive Design
  - CSS Grid & Flexbox layouts
  - Sticky Navigation Header

### Performance Optimizations
- Critical CSS inlined in HTML
- Async CSS loading with preload
- Service Worker caching strategy
- Resource hints (preconnect, dns-prefetch, prefetch)
- Image lazy loading
- PWA support

### SEO Features
- Comprehensive meta tags
- Open Graph tags for social sharing
- Twitter Card tags
- LinkedIn specific meta
- Structured data (JSON-LD)
- XML sitemap
- Canonical URLs
- Schema.org markup

### Security Headers
- Content Security Policy (CSP)
- X-Content-Type-Options: nosniff
- X-Frame-Options: DENY
- X-XSS-Protection: 1; mode=block
- Referrer-Policy: strict-origin-when-cross-origin

### Accessibility Features
- Skip navigation links
- Focus styles with visible outlines
- Reduced motion support
- Semantic HTML5 structure
- ARIA labels where appropriate
- Alt text for images
- Keyboard navigation support

## Content Structure

### Homepage (`index.html`)
- Hero section with gradient background
- Welcome message
- Quick links to main sections
- Community highlights
- Local business showcase
- Upcoming events preview

### Community Page (`community.html`)
- Local amenities listing
- Schools and educational facilities
- Sports clubs and organizations
- Community groups
- Healthcare services
- Nearby attractions (Bunratty Castle, Craggaunowen)

### Business Directory (`business.html`)
- Categorized business listings
- Interactive Leaflet.js map
- Business contact information
- Opening hours
- Services offered
- Location markers

### Events Page (`events.html`)
- Event calendar
- Upcoming events listing
- Event details and descriptions
- Location information
- Contact details for organizers

### Privacy Policy (`privacy.html`)
- Data protection information
- Cookie policy
- User rights
- Contact information

## Development Guidelines

### No Build Process
- Direct file editing
- No compilation required
- No package dependencies
- Static file serving

### Local Development
```bash
# Python HTTP server
python -m http.server 8000

# Node.js serve
npx serve .

# Direct browser opening
open index.html
```

### Validation
```bash
# HTML validation
html5validator *.html

# Link checking
linkchecker index.html
```

### Code Style
- Semantic HTML5 elements
- BEM-inspired CSS naming
- Minimal JavaScript (vanilla only)
- Mobile-first responsive design
- Progressive enhancement

## Analytics & Tracking
- Google Analytics 4 integration
- Event tracking for user interactions
- Page view tracking
- Custom dimensions for community metrics

## Browser Support
- Modern browsers (Chrome, Firefox, Safari, Edge)
- CSS Grid and Flexbox support required
- No Internet Explorer support
- Graceful degradation for older browsers

## Deployment
- Static hosting compatible
- No server-side requirements
- CDN-friendly structure
- GitHub Pages ready

## Future Enhancements
- Newsletter subscription
- Event submission form
- Business registration portal
- Community forum integration
- Multi-language support (Irish Gaelic)
- Enhanced PWA features

## Contributing
This is a community project. Contributions should:
- Maintain the existing design system
- Follow semantic HTML practices
- Keep JavaScript minimal
- Ensure mobile responsiveness
- Include appropriate meta tags
- Update sitemap.xml for new pages

## License & Attribution
- Community-owned project
- Stock photos from Unsplash (credited)
- Partner logos used with permission
- Open source web technologies

## Contact
Sixmilebridge Town Team  
County Clare, Ireland  
Website: https://sixmilebridge.ie

---

*Last Updated: December 2025*  
*Version: 1.0*