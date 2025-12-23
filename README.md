# Cinder & Laurel Group

A minimalist, luxury holdings landing site for **cinderandlaurel.com**.

This repository contains a static website representing Cinder & Laurel Group, a private holdings company for select ventures in specialized markets.

---

## 🏗️ Tech Stack

- **HTML5** - Semantic, accessible markup
- **CSS3** - Custom design system with CSS variables
- **Vanilla JavaScript** - Minimal JS for mobile navigation
- **GitHub Pages** - Static site hosting

No frameworks, no build process, no dependencies. Just clean, fast, static files.

---

## 📁 File Structure

```
cinderandlaurel/
├── site/
│   ├── index.html           # Home page
│   ├── portfolio.html       # Operating brands portfolio
│   ├── contact.html         # Contact information
│   ├── privacy.html         # Privacy policy
│   └── assets/
│       ├── styles.css       # Main stylesheet
│       ├── logo.svg         # C&L monogram logo
│       └── script.js        # Mobile menu toggle
├── .github/
│   └── workflows/
│       └── static.yml       # GitHub Pages deployment
└── README.md                # This file
```

---

## 🚀 Local Development

### Option 1: Open Directly in Browser
Simply open `site/index.html` in your browser. All assets use relative paths.

### Option 2: Use a Local Server (Recommended)
For better testing of navigation and fonts:

```bash
# Using Python 3
cd site
python -m http.server 8000

# Using Python 2
cd site
python -m SimpleHTTPServer 8000

# Using Node.js (if you have npx)
cd site
npx serve

# Using PHP
cd site
php -S localhost:8000
```

Then visit: `http://localhost:8000`

---

## 🌐 Deployment to GitHub Pages

### Method 1: Automatic Deployment (GitHub Actions)
This repo includes a GitHub Actions workflow that automatically deploys to GitHub Pages on every push to the `main` branch.

**Steps:**
1. Push this repository to GitHub
2. Go to **Settings** > **Pages**
3. Under "Build and deployment":
   - Source: **GitHub Actions**
4. The workflow will automatically run and deploy your site

Your site will be live at: `https://[username].github.io/cinderandlaurel/`

### Method 2: Manual Deployment (Branch Publishing)
If you prefer not to use GitHub Actions:

1. Push this repository to GitHub
2. Go to **Settings** > **Pages**
3. Under "Build and deployment":
   - Source: **Deploy from a branch**
   - Branch: `main`
   - Folder: `/site`
4. Click **Save**

Your site will be live at: `https://[username].github.io/cinderandlaurel/`

### Custom Domain Setup
To use `cinderandlaurel.com`:

1. Go to **Settings** > **Pages**
2. Under "Custom domain", enter: `cinderandlaurel.com`
3. Click **Save**
4. Configure your DNS:
   - Add a `CNAME` record pointing to: `[username].github.io`
   - Or add `A` records pointing to GitHub's IPs:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
5. Wait for DNS propagation (can take up to 24 hours)
6. Enable "Enforce HTTPS" in Pages settings

---

## 🎨 Design System

### Color Variants
The site includes two color accent variants:

**Default (Brass)**
- Deep neutral background
- Brass/gold accent: `#c9a961`

**Ivory Variant**
- Slightly cooler background
- Ivory accent: `#e8dfc8`

To switch variants, add `data-theme="ivory"` to the `<html>` tag:
```html
<html lang="en" data-theme="ivory">
```

Or use the theme switcher (currently commented out in `script.js`).

### Typography
- **Headings**: Spectral (serif) from Google Fonts
- **Body**: System font stack (SF Pro, Segoe UI, Roboto, etc.)
- Fallbacks ensure fast loading and cross-platform compatibility

### Key CSS Variables
```css
--color-bg-primary      /* Main background */
--color-bg-secondary    /* Sections/footer background */
--color-bg-elevated     /* Cards and elevated surfaces */
--color-text-primary    /* Headings and primary text */
--color-text-secondary  /* Body text */
--color-text-muted      /* Labels and meta text */
--color-accent          /* Links and accents */
--color-border          /* Dividers and borders */
```

Edit these in `assets/styles.css` to customize the color scheme.

---

## ♿ Accessibility

- Semantic HTML5 elements
- ARIA labels on navigation and interactive elements
- Keyboard-navigable (test with Tab key)
- Focus indicators on all interactive elements
- Good color contrast (WCAG AA compliant)
- Reduced motion support via `prefers-reduced-motion`
- Screen reader friendly

---

## ⚡ Performance

- No external dependencies (except Google Fonts)
- Minimal JavaScript (~2KB)
- CSS uses system fonts as fallbacks
- No tracking scripts or analytics
- Fast initial load (<100KB total)
- Optimized for Lighthouse scores

---

## 🧪 Testing Checklist

Before deploying:
- [ ] Test all navigation links
- [ ] Verify mobile menu works on small screens
- [ ] Check responsive layout (mobile, tablet, desktop)
- [ ] Test keyboard navigation (Tab, Enter, Escape)
- [ ] Verify email link works
- [ ] Test in multiple browsers (Chrome, Firefox, Safari, Edge)
- [ ] Run Lighthouse audit (aim for 90+ in all categories)
- [ ] Validate HTML: https://validator.w3.org/
- [ ] Check for broken links

---

## 📝 Content Guidelines

This site represents a holdings company, NOT a consumer e-commerce site.

**DO:**
- Use institutional, professional language
- Emphasize stewardship, quality, compliance
- Keep copy concise and understated
- Maintain luxury/premium tone

**DON'T:**
- Market or sell tobacco products
- Include product pricing or "buy now" CTAs
- Use cigar/tobacco imagery
- Include shopping cart functionality
- Make health claims

---

## 🔒 Privacy & Compliance

- No analytics or tracking cookies
- No third-party scripts (except Google Fonts)
- Age-gated content considerations (21+)
- Complies with GitHub Pages terms of service
- See `privacy.html` for full privacy policy

---

## 🛠️ Customization

### Update Contact Email
Replace `hello@cinderandlaurel.com` in:
- `contact.html` (2 instances)
- `privacy.html` (2 instances)

### Update Operating Brands
Edit the portfolio cards in:
- `index.html` (Brand Architecture section)
- `portfolio.html` (Portfolio Grid section)

### Change Logo
Replace `assets/logo.svg` with your own SVG file (maintain similar dimensions)

### Add New Pages
1. Create new HTML file in `site/`
2. Use existing pages as templates
3. Add navigation link to all pages
4. Update footer if needed

---

## 📄 License

© 2024 Cinder & Laurel Group. All rights reserved.

This website code is proprietary. Not licensed for reuse or redistribution without permission.

---

## 📧 Support

For questions or issues:
- Email: hello@cinderandlaurel.com
- Create an issue in this repository (for technical problems)

---

## 🗺️ Roadmap

Future enhancements (optional):
- [ ] Add form validation to contact page
- [ ] Implement server-side contact form (if moving off GitHub Pages)
- [ ] Add subtle scroll animations (accessibility-conscious)
- [ ] Create additional portfolio detail pages
- [ ] Add team/about page
- [ ] Implement newsletter signup (if desired)

---

**Built with care by a senior full-stack engineer + brand-conscious designer.**
