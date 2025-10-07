# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a personal portfolio and landing page for Clissman Camacho, Engineering Manager & Senior Software Engineer. It's a static single-page application built with vanilla HTML, CSS, and jQuery.

## Architecture

**Static Single-Page Website**: All content is in a single `index.html` file with section-based navigation (home, about, experience, journey, projects, contact).

**Key Files**:
- `index.html` - Main entry point containing all content sections
- `assets/css/style.css` - Custom styles (based on "Freelancer" template by UIdeck)
- `assets/js/main.js` - jQuery-based interactions (sticky nav, smooth scroll, animations)
- `resume.pdf` - Downloadable resume linked from the site

**External Dependencies**:
- Bootstrap 4
- jQuery 1.12.4
- LineIcons (icon font)
- WOW.js animations (via animate.css)
- Google Analytics (tracking ID: G-HQTJE2VJTW)

**Domain**: Hosted at clissmancamacho.com (see CNAME)

## Development

**Preview**: Open `index.html` directly in a browser, or use a local server:
```bash
python -m http.server 8000
# or
npx http-server
```

**No Build Process**: This is a static site with no compilation or bundling required.

## Content Structure

The site follows a timeline-based narrative:
- Header with social links (LinkedIn, GitHub, Twitter, Instagram)
- Hero section with CTA to download resume
- About section highlighting hiring value propositions
- Experience section with chronological work history (2024-2019)
- Journey section showing skills progression timeline (2017-2025)
- Projects section showcasing key achievements
- Contact section with email CTA
- Footer with navigation and social links

## Making Changes

**Content Updates**: All text content is directly in `index.html`. Sections use specific CSS classes for styling.

**Animations**: Uses WOW.js with `data-wow-duration` and `data-wow-delay` attributes for staggered fade-in effects.

**Navigation**: Smooth scrolling handled by `scrolling-nav.js` with `page-scroll` class on links. Active section highlighting in `main.js`.

**Resume**: Update `resume.pdf` when changing the resume. Link is at `/resume.pdf`.

## Important Notes

- Analytics tracking is enabled with Google Analytics (gtag.js)
- Email contact: mail@clissmancamacho.com
- Template credits: UIdeck "Freelancer" template
- Uses Bootstrap grid system for responsive layouts
