# UIUC NLP Website 2025

This is a modernized version of the UIUC NLP website.

## Key Improvements

### Design & User Experience
- **Modern, responsive design** that works seamlessly on desktop, tablet, and mobile devices
- **Professional Illinois branding** with official colors (Illinois Blue #13294B and Illinois Orange #FF5F05)
- **Improved typography** using Illinois brand typefaces (Montserrat, Source Sans Pro)
- **Visual hierarchy** with clear sections and better content organization
- **Smooth animations** and transitions for better user engagement

### Technical Enhancements
- **HTML5** - Updated from outdated HTML 4.01
- **Responsive viewport** - Mobile-friendly meta tags
- **CSS Grid & Flexbox** - Modern layout techniques
- **Semantic HTML** - Better accessibility and SEO
- **Sticky navigation** - Easy access to different sections
- **Smooth scrolling** - Enhanced navigation experience

### Content Organization
- **Hero section** with feature image
- **Events section** - Prominently displayed with visual cards
- **Faculty directory** - Clean grid layout with hover effects
- **Research groups** - Well-organized with icons
- **Sidebar widgets** - Quick access to important information
- **Professional footer** - University branding and links

### Features
- Smooth scroll navigation
- Scroll spy (active section highlighting)
- Fade-in animations on scroll
- Hover effects on interactive elements
- External links open in new tabs
- Print-friendly styles
- Accessible design (ARIA labels, skip links)

## Files

- `index.html` - Main HTML file with modern semantic structure
- `style.css` - Comprehensive stylesheet with responsive design
- `script.js` - JavaScript for smooth interactions
- `README.md` - This documentation file

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Color Palette

- **Illinois Blue**: #13294B (Primary)
- **Illinois Orange**: #FF5F05 (Accent)
- **Background**: #f5f5f5 (page), #ffffff (cards)
- **Text**: #333333
- **Light Gray**: #f8f9fa (Sections)

## Typography

- **Headings / Nav**: Montserrat (Illinois brand)
- **Body**: Source Sans Pro (Illinois brand)
- **Icons**: Font Awesome 4.7.0

## Deployment

When deploying (e.g. GitHub Pages), the site uses **relative paths** for `style.css` and `graphics/`. That works when the repo is served from its root (e.g. `https://user.github.io/repo-name/`).

- **If the live site looks different from local:**  
  1. Hard-refresh (Ctrl+Shift+R / Cmd+Shift+R) or clear cache so the latest CSS loads.  
  2. In DevTools → Network, confirm `style.css` returns 200 and is not blocked.  
  3. Asset links use a version query (`?v=20260315`) to reduce cached CSS after updates; bump the version in each HTML file when you change styles and redeploy.

- **If the site is served from a subpath** (e.g. `university.edu/departments/nlp/`), either keep the same folder structure so relative paths still point to the right files, or add a build step that sets a `<base href="...">` and adjust asset paths.

## Contact

For questions or to add information to this site, please contact:
- Email: vdongre2@illinois.edu

## Credits

Built for the University of Illinois at Urbana-Champaign.

---

© 2025 University of Illinois. All rights reserved.

