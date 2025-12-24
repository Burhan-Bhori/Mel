# Melissa Disla - Personal Brand Website

A jaw-dropping, emotionally grounded, ultra-premium personal brand website for Melissa Disla, Confidence Coach and Leadership Developer.

## 🎯 Design Philosophy

This website is not a marketing brochure. It's a felt experience of clarity, grounding, and restored self-trust.

**Core Intent:** Calm the nervous system, clarify the mind, and build trust before converting.

**Signature Concept:** "Return to Confidence" — threaded subtly throughout the site.

---

## 📁 Project Structure

```
melissa-disla-website/
├── index.html          # Main website file
├── styles.css          # Complete design system and styles
└── README.md           # This file
```

---

## 🖼️ Replacing the Photo Placeholder

The website includes a circular photo placeholder in the hero section. To add Melissa's photo:

1. **Download the profile photo** from LinkedIn
2. **Save the image** as `melissa-disla.jpg` (or `.png`) in the same folder as `index.html`
3. **Open `index.html`** and find the photo placeholder section (around line 33)
4. **Replace this code block:**
   ```html
   <div class="placeholder-circle">
       <span class="placeholder-text">Replace with Melissa Disla's<br>LinkedIn profile photo</span>
   </div>
   ```
   
   **With:**
   ```html
   <img src="melissa-disla.jpg" alt="Melissa Disla, Confidence Coach and Leadership Developer">
   ```

5. **Save the file** and refresh your browser

---

## ✉️ Updating the Email Address

The contact email is currently set to `hello@melissadisla.com`.

To update it:

1. **Open `index.html`**
2. **Search for** `mailto:hello@melissadisla.com` (appears in the final invitation section)
3. **Replace with** your preferred email address
4. **Save the file**

---

## ✏️ Customizing Content

All content can be edited directly in `index.html`. Each section is clearly labeled with HTML comments.

### Section Structure
- **Hero** - Main headline and CTAs
- **The Experience** - Empathetic copy validating internal experiences
- **Introducing Melissa** - Background and positioning
- **Values Contrast** - What the work is NOT
- **Who This Is For** - Audience framing
- **The Work** - Three pathway cards (Individuals, Leaders, Organizations)
- **Testimonials** - Three selected testimonials
- **Speaking** - Keynote positioning
- **Invitation** - Final CTA and closure

### Editing Tips
- Maintain the tone: calm, grounded, reflective
- Keep "Return to Confidence" threading subtle
- Preserve generous white space
- Avoid marketing jargon

---

## 🎨 Design System Reference

### Colors
- **Ivory background:** `#FDFBF7`
- **Warm gray:** `#E8E4DD`
- **Off-black text:** `#3A3A3A`
- **Deep sage accent:** `#5A6F5C`

### Typography
- **Serif (emotional depth):** Cormorant Garamond
- **Sans-serif (clarity):** Inter
- **Type scale:** 14px → 18px → 24px → 32px → 48px → 64px

### Spacing System
Based on 8px increments. Adjust in `styles.css` via CSS custom properties.

---

## 🚀 Deployment Options

### Option 1: GitHub Pages (Free)
1. Create a GitHub repository
2. Upload all files (`index.html`, `styles.css`, photo)
3. Enable GitHub Pages in repository settings
4. Your site will be live at `https://username.github.io/repository-name`

### Option 2: Netlify (Free, Recommended)
1. Create account at [netlify.com](https://netlify.com)
2. Drag and drop your project folder
3. Custom domain support included
4. Automatic HTTPS

### Option 3: Vercel (Free)
1. Create account at [vercel.com](https://vercel.com)
2. Import project from GitHub or upload directly
3. Instant deployment with custom domain support

### Option 4: Custom Hosting
Upload files via FTP to any web hosting provider. Ensure `index.html` is in the root directory.

---

## 🌱 Content Evolution Plan

This website is designed as a **living body of work**, not a static launch artifact.

### Future Expansion Ideas

**1. Long-Form Content**
- Create a `/writing` or `/reflections` folder
- Add individual HTML pages for essays, articles, or thought pieces
- Link from main site with a "Read more" section
- Maintain the same calm, editorial aesthetic

**2. Keynote Recordings**
- Embed video or audio recordings of keynote talks
- Create a `/keynotes` page with talk descriptions and recordings
- Use Vimeo or YouTube for video hosting (privacy settings available)

**3. Resources Section**
- Downloadable PDFs, worksheets, or frameworks
- Brief guides on confidence, leadership presence, etc.
- Gated content for email list building (optional)

**4. Case Studies / Client Stories**
- Anonymized or permission-based transformation stories
- Focus on internal shift, not external metrics
- Maintain privacy and psychological safety

**5. Newsletter Archive**
- If you start a newsletter, archive past issues on the site
- Create a simple chronological list page
- Reinforces "body of work" positioning

### Architecture Considerations

The current single-page design can easily expand:
- Add navigation links to the hero or create a minimal header
- Create new HTML pages following the same design system
- All styles in `styles.css` are reusable across pages
- Maintain consistent typography, colors, and spacing

### Maintaining Brand Coherence

As you add content:
- ✅ Keep the tone calm, grounded, and reflective
- ✅ Use generous white space
- ✅ Thread "Return to Confidence" where natural
- ✅ Avoid loud design or marketing language
- ✅ Prioritize clarity over cleverness

---

## 🔧 Technical Notes

### Performance
- No external dependencies (except Google Fonts)
- Minimal JavaScript (only for staged reveal and scroll progress)
- Fast load times across all devices
- Optimized for mobile-first experience

### Accessibility
- Semantic HTML5 throughout
- ARIA labels on navigation and CTAs
- Keyboard navigable
- `prefers-reduced-motion` support
- High contrast mode optimization
- Generous line-height for readability

### Browser Support
- All modern browsers (Chrome, Firefox, Safari, Edge)
- Graceful degradation for older browsers
- Responsive design from 320px to 4K displays

---

## 📞 Questions or Support

For technical questions about this website, refer to:
- [MDN Web Docs](https://developer.mozilla.org/) - HTML/CSS reference
- [CSS-Tricks](https://css-tricks.com/) - Design and layout guidance

For design or brand questions, revisit the core intent: **restoring self-trust through calm, grounded clarity.**

---

**Built with intention. Designed to calm. Created to convert through clarity.**
