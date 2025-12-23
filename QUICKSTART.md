# 🚀 Quick Start Guide - Cinder & Laurel Group

Get your site live in **5 minutes** with this streamlined guide.

---

## ⚡ Fast Track to Deployment

### Step 1: Update Email (30 seconds)
Replace the placeholder email in these files:
- `site/contact.html` (line 43 & 110)
- `site/privacy.html` (line 110 & 145)

Change: `hello@cinderandlaurel.com` → **your actual email**

### Step 2: Test Locally (2 minutes)
```bash
cd site
python -m http.server 8000
```
Open: http://localhost:8000

✅ Check all pages load  
✅ Test mobile menu (resize browser)  
✅ Click all navigation links  

### Step 3: Push to GitHub (2 minutes)
```bash
cd /config/workspace/cinderandlaurel
git init
git add .
git commit -m "Initial commit: Cinder & Laurel Group site"
git remote add origin https://github.com/YOUR-USERNAME/cinderandlaurel.git
git push -u origin main
```

### Step 4: Enable GitHub Pages (1 minute)
1. Go to: **Settings** → **Pages**
2. Source: **GitHub Actions**
3. Wait ~1 minute for deployment

**Done!** Your site is live at:  
`https://YOUR-USERNAME.github.io/cinderandlaurel/`

---

## 🎨 Optional: Choose Your Color Variant

### Option A: Keep Brass (Default)
No changes needed. Warm brass accent (#c9a961).

### Option B: Switch to Ivory
Add `data-theme="ivory"` to `<html>` tag in all pages:
```html
<html lang="en" data-theme="ivory">
```

---

## 🌐 Custom Domain Setup (Optional)

### If You Own cinderandlaurel.com:

1. **In GitHub Pages:**
   - Settings → Pages → Custom domain
   - Enter: `cinderandlaurel.com`
   - Save

2. **In Your DNS Settings:**
   - Add CNAME record: `www` → `YOUR-USERNAME.github.io`
   - OR add A records to:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```

3. **Wait & Enable HTTPS:**
   - DNS propagation: 1-24 hours
   - Enable "Enforce HTTPS" in Pages settings

---

## ✅ Pre-Launch Checklist

Quick checks before going live:

- [ ] Email address updated
- [ ] All pages load without errors
- [ ] Mobile menu works
- [ ] All links go to correct pages
- [ ] Footer copyright year is current
- [ ] Tested on phone (or responsive mode)
- [ ] No broken images or styles

---

## 🆘 Troubleshooting

### "Site not loading after deployment"
- Wait 2-3 minutes for GitHub Actions to complete
- Check Actions tab for any errors
- Verify Pages is enabled in Settings

### "Styles not loading"
- Check that all file paths are relative
- Verify `assets/` folder is in `site/` directory
- Hard refresh browser (Cmd+Shift+R or Ctrl+F5)

### "Mobile menu not working"
- Check that `script.js` is loading
- Open browser console for errors
- Verify JavaScript is enabled

### "Custom domain not working"
- Verify DNS records are correct
- Wait up to 24 hours for propagation
- Check DNS with: https://dnschecker.org/

---

## 📱 Test on Real Devices

Share these links with your phone:

**Local testing:**  
http://YOUR-COMPUTER-IP:8000

**Live site:**  
https://YOUR-USERNAME.github.io/cinderandlaurel/

Test:
- Navigation works
- Text is readable
- Buttons are tappable
- No horizontal scrolling

---

## 🔧 Common Customizations

### Change Accent Color
Edit `site/assets/styles.css` line 10:
```css
--color-accent: #c9a961;  /* Change to your color */
```

### Update Brand Cards
Edit `site/portfolio.html` starting at line 40.  
Copy/paste existing card structure.

### Add New Page
1. Copy `contact.html` as template
2. Update content and title
3. Add link to navigation in all pages
4. Test all links work

---

## 📚 Full Documentation

For comprehensive guides, see:
- **[README.md](README.md)** - Complete documentation
- **[DEPLOYMENT.md](DEPLOYMENT.md)** - Detailed deployment guide
- **[SITE_OVERVIEW.md](SITE_OVERVIEW.md)** - Full site breakdown

---

## 💬 Need Help?

- Check GitHub Actions logs for deployment errors
- Verify file paths are correct
- Test in incognito/private browsing mode
- Clear browser cache if styles aren't updating

---

**That's it! Your luxury holdings site is ready.** 🎯

---

## 🎁 Bonus: One-Command Local Preview

```bash
cd site && python -m http.server 8000
```

Then visit: http://localhost:8000

Press `Ctrl+C` to stop.

---

**Built for cinderandlaurel.com**  
Minimalist. Luxury. Ready to deploy.
