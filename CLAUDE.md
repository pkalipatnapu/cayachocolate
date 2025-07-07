# Caya Chocolate Website - Design Documentation

## Project Overview
This is a static website for Caya Chocolate, a California-based artisan chocolate company currently "taking a break" from operations. The site was rebuilt from archived Wix files into a clean, modern static site suitable for GitHub Pages hosting.

## Design Philosophy & Choices

### Typography
- **Primary Font**: Inter (consistent across all text elements)
- **Rationale**: Clean, modern sans-serif for better readability and consistency
- **Weight Hierarchy**: 700 for main headings, 600 for section headings, 400-500 for body text
- **Avoided**: Playfair Display (initially used) was removed for consistency

### Color Palette
- **Primary Brown**: #8B4513 (chocolate-inspired brand color)
- **Dark Brown**: #6d3410 (hover states, darker accents)
- **Dark Navbar**: #2c1810 (navigation background for logo visibility)
- **Text**: #2c1810 (headings), #4a4a4a (body), #6a6a6a (secondary)
- **Navigation**: #f0e6d2 (logo text), #b8a690 (nav links), #f0e6d2 (active/hover)
- **Background**: #fdfcf8 (warm off-white), #f8f6f1 (light sections)
- **White**: #fff (content blocks, forms)

### Content Strategy
- **Simplified Headers**: Removed verbose titles (e.g., "About Caya Chocolate" → "About")
- **Streamlined Messaging**: Focus on "taking a break" message while preserving brand story
- **No Commerce Elements**: Removed all shop links, cart widgets, booking functionality
- **Contact**: Replaced static info with functional email form

### Image Treatment
- **Aspect Ratios**: Generous vertical space (500px height for portraits, 400px for galleries)
- **Positioning**: `object-position: center center` (center 60% for face-focused images)
- **Product Images**: `object-fit: contain` to show full products without cropping
- **Hover Effects**: Smooth transitions showing chocolate bars when hovering over packaging
- **Face Positioning**: Last two gallery images and hero image positioned to center people's faces

### Layout Principles
- **Two-Page Structure**: Homepage (with break announcement) + About page
- **Responsive Grid**: Auto-fit minmax grids for flexible layouts
- **Spacing**: Reduced paragraph margins (0.75rem) for tighter text flow
- **Footer**: Minimal, compact design without photo credits

### Interactive Elements
- **Chocolate Gallery**: Hover reveals chocolate bars inside packaging
- **Contact Form**: Functional mailto form with validation
- **Navigation**: Clean, minimal navigation with active states
- **Logo**: Clickable "Caya" text returns to homepage

## Technical Decisions

### File Structure
```
cayachocolate/
├── index.html          # Homepage with break announcement
├── about.html          # Company story and process
├── styles.css          # All styling in single file
├── logo.svg           # SVG logo (from assets/Asset 4.svg)
├── assets/            # All photography and product images
└── CNAME              # GitHub Pages domain configuration
```

### Asset Management
- **Original Photography**: Preserved all DSC_* process photos
- **Product Images**: Added new PNG files for chocolate packaging and reveals
- **Logo**: Used existing SVG for scalability
- **Removed**: All Wix boilerplate, archive.org references, and unused assets

### Responsive Design & Mobile Optimization
- **Mobile-First**: Flexible grids that adapt to screen size
- **Breakpoints**: 768px (tablets), 480px (mobile), 320px (small mobile)
- **Touch-Friendly**: 44px minimum touch targets for all interactive elements
- **Navigation**: Horizontal layout maintained on mobile with optimized spacing
- **Typography**: Responsive font scaling (1.8rem → 1.6rem for titles on smallest screens)
- **Form Optimization**: 16px+ input font sizes to prevent iOS zoom, full-width submit buttons
- **Grid Adaptation**: Multi-column layouts stack to single column on mobile
- **Spacing**: Reduced padding and margins optimized for thumb navigation
- **Performance**: Lightweight CSS with no dependencies for fast mobile loading

## Content Guidelines

### Tone & Voice
- **Warm but Professional**: Reflects artisan craft approach
- **Personal**: Mentions founders by name (Pradeep and Deeksha)
- **Honest**: Clear about current "break" status
- **Quality-Focused**: Emphasizes single-origin beans and minimal ingredients

### Photography Style
- **Process-Focused**: Behind-the-scenes chocolate making shots
- **Product-Centric**: Clean product shots with hover reveals
- **Personal**: Founders photo for authentic connection
- **Professional**: High-quality, well-lit imagery throughout

## Development Notes
- **No Dependencies**: Pure HTML/CSS, no frameworks or build process
- **GitHub Pages Ready**: Static files suitable for direct hosting
- **Form Handling**: Uses mailto for contact form (simple but functional)
- **Performance**: Optimized images, minimal CSS, fast loading
- **Accessibility**: Semantic HTML, proper labels, good contrast ratios
- **Mobile Standards**: Follows Apple/Google touch target guidelines (44px minimum)
- **Cross-Device Testing**: Responsive design tested across multiple breakpoints
- **Asset Cleanup**: Only necessary files retained, unused assets removed

## Future Considerations
- Consider adding proper form backend if contact volume increases
- May add newsletter signup when business resumes
- Could expand product gallery when new chocolates are developed
- Potential for blog/updates section if regular content is created

## Brand Assets Preserved
- Single-origin chocolate focus
- Artisan/handmade positioning  
- California location pride
- Minimal ingredients philosophy
- Educational approach (tasting notes concept)
- Personal founder story
- High-quality photography aesthetic