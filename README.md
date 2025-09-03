 # 📸 Nina Carducci – Photographer Portfolio Website  

This project is part of my Web Development program. The goal was to **debug and optimize** a photographer's portfolio website for better functionality, performance, accessibility, and SEO.  

 **Live Site:** [Nina Carducci Portfolio](https://portuguesricardo.github.io/Debug-Optimize-Photographer-Website/)  


---

## Project Overview  

- Debugged broken functionality (gallery modal navigation, filter highlight).  
- Optimized images and loading strategy to achieve high Lighthouse performance.  
- Improved accessibility (labels, semantic structure, color contrast).  
- Enhanced SEO (meta tags, structured data, Open Graph & Twitter Cards).  

---

## Tech Stack  

- **HTML5 / CSS3**  
- **JavaScript (jQuery)**  
- **Bootstrap 5** (layout, modals, navigation)  
- **Maugallery.js** (custom lightbox/gallery plugin)  

---

## Debugging  

### Fixed Issues:  
1. **Gallery Modal Arrows**  
   - Bug: Navigation arrows didn’t work.  
   - Cause: Absolute vs relative path mismatch in `src` comparison.  
   - Fix: Unified comparison logic using `document.querySelector(...).src`.  

2. **Category Filter Highlight**  
   - Bug: Gold highlight not showing.  
   - Cause: Wrong CSS class targeted (`.active` instead of `.active-tag`).  
   - Fix: Updated JS to toggle the correct CSS class.  

---

## Optimization  

- Compressed and converted large images to **WebP**.  
- Reduced LCP (Largest Contentful Paint) from ~10s → ~1.6s.  
- Added `width` and `height` attributes to images to prevent layout shifts.  
- Lighthouse **Performance score: 96**.  

---

## Accessibility  

- Added `<label>` elements to all form inputs.  
- Improved heading hierarchy (`h1` as main page title).  
- Introduced `<main>` and `<nav>` landmarks.  
- Fixed color contrast for gallery filter buttons.  
- Lighthouse **Accessibility score: 100**.  

---

## SEO  

- Added `<title>` and `<meta name="description">`.  
- Added `alt` attributes to images.  
- Implemented Open Graph + Twitter Cards for social sharing.  
- Added structured data (`LocalBusiness`) for Google Rich Snippets.  
- Lighthouse **SEO score: 100**.  

---

## Final Scores (Lighthouse Audit)  

- **Performance:** 96 (updated)  
- **Accessibility:** 100  
- **Best Practices:** 100  
- **SEO:** 100  
 **Lighthouse Report:** https://portuguesricardo.github.io/Debug-Optimize-Photographer-Report/
---

## How to Run Locally  

1. **Clone the repository**
   ```bash
   git clone https://github.com/portuguesricardo/Debug-Optimize-Photographer-Website.git   
2. **Navigate into the project folder**
```bash
cd Debug-Optimize-Photographer-Website
```
3. **Open the site in your browser**

- Locate the index.html file.
- Right-click → “Open with” → Choose your browser (Chrome, Firefox, etc.).
- Alternatively, serve it with a live server (e.g., VS Code Live Server extension).
