# 🚀 Deployment Guide - PR Unisex Salon Website

## ✅ Pre-Deployment Checklist

Before deploying, ensure:
- [ ] All dependencies installed (`npm install` completed)
- [ ] Build works locally (`npm run build` successful)
- [ ] Website tested on `npm run dev`
- [ ] Contact numbers are correct (+91 84149 16341)
- [ ] Google Maps link works

---

## 🌐 Method 1: GitHub Pages (100% FREE)

### ✨ Best For: Small businesses, portfolios

### Step-by-Step:

**1. Create GitHub Repository**
```bash
# Initialize git (if not done)
git init
git add .
git commit -m "Initial commit - PR Unisex Salon website"

# Create repo on GitHub, then:
git remote add origin https://github.com/yourusername/pr-unisex-salon.git
git branch -M main
git push -u origin main
```

**2. Install GitHub Pages Package**
```bash
npm install --save-dev gh-pages
```

**3. Update vite.config.js**
```javascript
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'

export default defineConfig({
  base: '/pr-unisex-salon/',  // ⚠️ Replace with YOUR repo name
  plugins: [react()],
})
```

**4. Add Deploy Scripts to package.json**
Add these lines to the "scripts" section:
```json
"predeploy": "npm run build",
"deploy": "gh-pages -d dist"
```

**5. Deploy!**
```bash
npm run deploy
```

**6. Enable GitHub Pages**
- Go to your repo on GitHub
- Settings → Pages
- Source: `gh-pages` branch
- Save

**🎉 Live URL:** `https://yourusername.github.io/pr-unisex-salon/`

---

## 🎯 Method 2: Netlify (RECOMMENDED - FREE)

### ✨ Best For: Automatic deployments, custom domains, SSL

### Option A: Drag & Drop (2 Minutes)

1. Build your project:
```bash
npm run build
```

2. Go to [Netlify Drop](https://app.netlify.com/drop)

3. Drag the `dist` folder onto the page

4. **Done!** Your site is live instantly

**✅ Pros:** Super fast, no configuration needed

### Option B: GitHub Integration (Automatic Updates)

1. Go to [Netlify](https://app.netlify.com)

2. Click **"Add new site"** → **"Import an existing project"**

3. Choose **GitHub** and authorize Netlify

4. Select your repository

5. Build settings:
   - **Build command:** `npm run build`
   - **Publish directory:** `dist`
   - **Node version:** 18

6. Click **"Deploy site"**

**✅ Pros:** Auto-deploys on every GitHub push

### Add Custom Domain (Optional)

1. Buy a domain (e.g., `prunisexsalon.com` from Namecheap - ₹600/year)

2. In Netlify: Site settings → Domain management

3. Click "Add custom domain"

4. Follow DNS configuration instructions

5. **Free SSL certificate** automatically included!

---

## ⚡ Method 3: Vercel (FREE)

### ✨ Best For: Next.js projects, global CDN

### Via Dashboard:

1. Go to [Vercel](https://vercel.com)

2. Click **"Add New"** → **"Project"**

3. Import from GitHub

4. Select your repository

5. Vercel auto-detects Vite settings

6. Click **"Deploy"**

**✅ Pros:** Fastest global CDN, preview deployments

### Via CLI:

```bash
npm install -g vercel
vercel login
vercel --prod
```

---

## 🔥 Method 4: Firebase Hosting (FREE)

### Step-by-Step:

**1. Install Firebase CLI**
```bash
npm install -g firebase-tools
```

**2. Login to Firebase**
```bash
firebase login
```

**3. Initialize Firebase**
```bash
firebase init
```
- Select: **Hosting**
- Public directory: `dist`
- Single-page app: **Yes**
- GitHub auto-deploy: **No** (unless you want it)

**4. Build & Deploy**
```bash
npm run build
firebase deploy
```

**🎉 Live URL:** `https://your-project.web.app`

---

## 📊 Comparison Table

| Feature | GitHub Pages | Netlify | Vercel | Firebase |
|---------|--------------|---------|--------|----------|
| **Cost** | FREE | FREE | FREE | FREE |
| **Custom Domain** | ✅ | ✅ | ✅ | ✅ |
| **SSL (HTTPS)** | ✅ | ✅ | ✅ | ✅ |
| **Auto Deploy** | Manual | ✅ | ✅ | Manual |
| **Build Time** | Slow | Fast | Fastest | Fast |
| **CDN** | Basic | Global | Global | Global |
| **Setup Difficulty** | Medium | Easy | Easiest | Medium |
| **Best For** | Simple sites | Most cases | All projects | Google users |

**🏆 Recommendation:** Use **Netlify** for best experience!

---

## 🎨 After Deployment

### 1. Test Everything

- ✅ Click all phone numbers (should open dialer)
- ✅ Click WhatsApp button (should open WhatsApp)
- ✅ Click Google Maps (should open directions)
- ✅ Test on mobile phone
- ✅ Check loading speed

### 2. Submit to Google

**Google Search Console:**
1. Go to [Google Search Console](https://search.google.com/search-console)
2. Add your website URL
3. Verify ownership
4. Submit sitemap (optional)

**Google My Business:**
1. Update business website URL
2. Add to "Website" field in Google Business Profile

### 3. Share on Social Media

Update these platforms:
- [ ] WhatsApp Status
- [ ] Facebook Page
- [ ] Instagram Bio
- [ ] Google My Business
- [ ] Business cards

---

## 🔧 Troubleshooting

### Problem: Build fails
**Solution:**
```bash
# Clear cache
rm -rf node_modules
rm package-lock.json
npm install
npm run build
```

### Problem: 404 error on deployment
**Solution:** Ensure `vite.config.js` has correct `base` path

### Problem: Styles not loading
**Solution:** Check that Tailwind CSS is properly configured in `index.css`

### Problem: WhatsApp link not working
**Solution:** Ensure format is: `https://wa.me/918414916341`

---

## 📱 Post-Deployment Optimization

### 1. Add Google Analytics (Optional)
1. Create GA4 property
2. Add tracking code to `index.html`

### 2. Enable HTTPS
All platforms provide free SSL - just enable it in settings

### 3. Monitor Performance
Use tools:
- Google PageSpeed Insights
- GTmetrix
- Lighthouse (Chrome DevTools)

### 4. Regular Updates
- Update services/prices as needed
- Add real customer photos
- Update testimonials

---

## 🎯 Custom Domain Setup (If You Buy One)

### For Netlify:
1. Buy domain from Namecheap/GoDaddy (₹600-800/year)
2. In Netlify: Settings → Domain management
3. Add custom domain: `prunisexsalon.com`
4. Update nameservers at your domain provider:
   - `dns1.p01.nsone.net`
   - `dns2.p01.nsone.net`
   - `dns3.p01.nsone.net`
   - `dns4.p01.nsone.net`

**Wait 24-48 hours for DNS propagation**

---

## 🆘 Need Help?

Contact for deployment support:
- 📞 **Phone:** +91 84149 16341
- 💬 **WhatsApp:** +91 84149 16341

---

**🎉 Congratulations! Your premium salon website is now LIVE!**

Share it with your customers and watch your bookings grow! 🚀
