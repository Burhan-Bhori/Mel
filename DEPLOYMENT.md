# Deployment Guide - Melissa Disla Website

## 📋 Pre-Deployment Checklist

Before deploying, ensure:

- [x] `melissa-disla.jpg` is in the root folder
- [ ] Contact email in `index.html` is correct (line search for `mailto:`)
- [ ] All content has been reviewed for accuracy
- [ ] Test website locally in multiple browsers
- [ ] Verify mobile menu works (resize browser to 375px)
- [ ] Test FAQ accordion (click questions)
- [ ] Verify all images load
- [ ] Check keyboard navigation (Tab key)

---

## 🚀 Deployment Option 1: GitHub Pages (Recommended)

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** icon → **New repository**
3. Repository settings:
   - **Name:** `melissa-disla-website` (or your preferred name)
   - **Description:** "Personal brand website for Melissa Disla - Confidence Coach & Leadership Developer"
   - **Visibility:** Public
   - **Initialize:** Do NOT add README, .gitignore, or license
4. Click **Create repository**

### Step 2: Upload Files

**Option A: Web Interface (Easiest)**
1. On your repository page, click **uploading an existing file**
2. Drag and drop these files:
   - `index.html`
   - `styles.css`
   - `melissa-disla.jpg`
   - `README.md`
3. Add commit message: "Initial website deployment"
4. Click **Commit changes**

**Option B: Git Command Line**
```bash
# Navigate to your project folder
cd C:\Users\Burhan\.gemini\antigravity\scratch\melissa-disla-website

# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial website deployment"

# Add remote (replace YOUR_USERNAME and REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to repository **Settings**
2. Scroll to **Pages** section (left sidebar)
3. Under "Build and deployment":
   - **Source:** Deploy from a branch
   - **Branch:** Select `main` (or `master`)
   - **Folder:** Select `/ (root)`
4. Click **Save**

### Step 4: Wait for Deployment

- GitHub will build your site (takes 1-3 minutes)
- Once ready, you'll see: "Your site is live at https://YOUR_USERNAME.github.io/REPO_NAME/"
- Click the URL to view your live website!

### Step 5: Custom Domain (Optional)

If you have a domain (e.g., `melissadisla.com`):

1. In GitHub Pages settings, enter your custom domain
2. Check "Enforce HTTPS"
3. In your domain registrar (GoDaddy, Namecheap, etc.):
   - Add CNAME record pointing to `YOUR_USERNAME.github.io`
   - Wait 24-48 hours for DNS propagation

---

## 🌐 Deployment Option 2: Netlify (Fastest)

### Drag & Drop Method

1. Go to [netlify.com](https://www.netlify.com/)
2. Sign up or log in (free account)
3. Click **Add new site** → **Deploy manually**
4. Drag your entire `melissa-disla-website` folder to the drop zone
5. Wait 10-30 seconds
6. Your site is live! (e.g., `random-name-12345.netlify.app`)

### Custom Domain on Netlify

1. Click **Domain settings**
2. Click **Add custom domain**
3. Enter your domain name
4. Follow DNS configuration instructions
5. Enable HTTPS (automatic with Netlify)

---

## ⚡ Deployment Option 3: Vercel (Developer-Friendly)

### One-Click Deploy

1. Go to [vercel.com](https://vercel.com/)
2. Sign up with **GitHub account**
3. Click **Add New** → **Project**
4. Import your GitHub repository
5. Settings:
   - **Framework Preset:** None (static site)
   - **Root Directory:** `./`
   - **Build Command:** (leave empty)
   - **Output Directory:** `./`
6. Click **Deploy**
7. Live in ~30 seconds!

---

## 🔍 Post-Deployment Testing

### Browser Testing
Visit your live site and test:
- [ ] Desktop view (1920x1080, 1366x768, 1024x768)
- [ ] Mobile view (iPhone, Android)
- [ ] Tablet view (iPad)

### Functionality Checklist
- [ ] All navigation links work
- [ ] Mobile hamburger menu opens/closes
- [ ] FAQ questions expand/collapse
- [ ] LinkedIn link opens in new tab
- [ ] Scroll progress indicator works
- [ ] Hero photo loads correctly
- [ ] All sections are visible
- [ ] Footer displays properly

### Performance Testing
Run [PageSpeed Insights](https://pagespeed.web.dev/):
```
https://pagespeed.web.dev/?url=YOUR_SITE_URL
```

Target scores:
- **Performance:** 90+
- **Accessibility:** 95+
- **Best Practices:** 90+
- **SEO:** 90+

---

## 🔧 Updating Your Live Site

### On GitHub Pages:
1. Edit files locally
2. Commit changes: `git add .` → `git commit -m "Update content"`
3. Push: `git push`
4. GitHub automatically redeploys (1-3 minutes)

### On Netlify:
1. Drag updated folder to Netlify dashboard
2. Instant deployment

### On Vercel:
1. Push to GitHub
2. Vercel auto-deploys on push

---

## 🎨 Quick Content Updates

### Change Contact Email
**File:** `index.html`  
**Search for:** `mailto:hello@melissadisla.com`  
**Replace with:** Your actual email

### Update Footer Year
**File:** `index.html`  
**Search for:** `© 2025 Melissa Disla`  
**Update year** when needed

### Change LinkedIn URL
**File:** `index.html`  
**Search for:** `https://www.linkedin.com/in/melissadisla`  
**Replace with:** Your actual LinkedIn profile URL

### Update Trust Badge Numbers
**File:** `index.html`  
**Search for:** `<div class="badge-number">20+</div>`  
**Update numbers** as your experience grows

---

## 📊 Analytics Setup (Optional)

### Google Analytics

1. Create account at [analytics.google.com](https://analytics.google.com/)
2. Get your tracking ID (e.g., `G-XXXXXXXXXX`)
3. Add to `index.html` before `</head>`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

### Plausible Analytics (Privacy-Friendly Alternative)

1. Sign up at [plausible.io](https://plausible.io/)
2. Add to `index.html` before `</head>`:

```html
<script defer data-domain="yourdomain.com" src="https://plausible.io/js/script.js"></script>
```

---

## 🐛 Troubleshooting

### Site Not Loading
- Check GitHub Pages is enabled in settings
- Verify branch is set to `main` or `master`
- Wait 3-5 minutes for initial deployment
- Clear browser cache (Ctrl+Shift+R)

### Images Not Showing
- Verify `melissa-disla.jpg` is in root folder
- Check filename matches exactly (case-sensitive)
- Ensure path in `index.html` is correct: `src="melissa-disla.jpg"`

### Mobile Menu Not Working
- Hard refresh: Ctrl+Shift+R (Windows) or Cmd+Shift+R (Mac)
- Check browser console for JavaScript errors (F12)
- Verify mobile width < 768px triggers hamburger

### FAQ Not Expanding
- Check JavaScript is enabled in browser
- Hard refresh page
- Test in different browser

---

## 🎯 SEO Improvements (Recommended)

Add to `<head>` section in `index.html`:

```html
<!-- Primary Meta Tags -->
<meta name="description" content="Melissa Disla - Confidence Coach, Leadership Developer, and L&D Strategist. Helping executives and leaders develop grounded presence and sustainable confidence.">
<meta name="keywords" content="confidence coach, leadership development, executive coaching, L&D strategy, keynote speaker">
<meta name="author" content="Melissa Disla">

<!-- Open Graph / Facebook -->
<meta property="og:type" content="website">
<meta property="og:url" content="https://yourdomain.com/">
<meta property="og:title" content="Melissa Disla | Confidence Coach & Leadership Developer">
<meta property="og:description" content="Helping executives and leaders develop grounded presence and sustainable confidence through coaching and L&D strategy.">
<meta property="og:image" content="https://yourdomain.com/melissa-disla.jpg">

<!-- Twitter -->
<meta property="twitter:card" content="summary_large_image">
<meta property="twitter:url" content="https://yourdomain.com/">
<meta property="twitter:title" content="Melissa Disla | Confidence Coach & Leadership Developer">
<meta property="twitter:description" content="Helping executives and leaders develop grounded presence and sustainable confidence.">
<meta property="twitter:image" content="https://yourdomain.com/melissa-disla.jpg">
```

---

## ✅ Launch Checklist

### Pre-Launch
- [ ] All content proofread
- [ ] Contact email verified
- [ ] Images optimized (< 500KB each)
- [ ] Tested on Chrome, Firefox, Safari
- [ ] Tested on iPhone and Android
- [ ] LinkedIn profile URL confirmed
- [ ] Run accessibility audit
- [ ] Run Lighthouse performance test

### Launch Day
- [ ] Deploy to chosen platform
- [ ] Verify live URL works
- [ ] Test all links
- [ ] Test mobile responsiveness
- [ ] Share on LinkedIn
- [ ] Update LinkedIn profile with website link
- [ ] Submit to Google Search Console

### Post-Launch (Week 1)
- [ ] Monitor analytics
- [ ] Check for broken links
- [ ] Gather user feedback
- [ ] Make any quick fixes
- [ ] Add to email signature

---

## 🎉 You're Ready to Launch!

Your website is **production-ready** and optimized for:
- ✅ Performance
- ✅ Accessibility  
- ✅ Mobile experience
- ✅ SEO
- ✅ Conversion

**Choose your deployment method above and go live! 🚀**

---

## 📞 Support Resources

- **GitHub Pages Docs:** https://docs.github.com/en/pages
- **Netlify Docs:** https://docs.netlify.com/
- **Vercel Docs:** https://vercel.com/docs
- **Web.dev Testing:** https://web.dev/measure/
- **HTML Validator:** https://validator.w3.org/
