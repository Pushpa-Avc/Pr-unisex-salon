# 🌟 PR Unisex Salon - Premium Website

**Ultra-premium, conversion-optimized website for PR Unisex Salon - Kharsang's finest grooming destination**

[![Made with React](https://img.shields.io/badge/Made%20with-React-61dafb?style=flat-square&logo=react)](https://reactjs.org/)
[![Styled with Tailwind](https://img.shields.io/badge/Styled%20with-Tailwind%20CSS-38bdf8?style=flat-square&logo=tailwind-css)](https://tailwindcss.com/)

---

## 📍 Business Information

**PR Unisex Salon - Kharsang**  
*"Premium Grooming. Trusted by Locals."*

- 📍 Near Kharsang Bridge (Left side), Kharsang, Changlang, Arunachal Pradesh - 792122
- 📞 **Phone:** +91 84149 16341
- 💬 **WhatsApp:** +91 84149 16341
- ⏰ **Hours:** Mon-Sun, 10:00 AM - 8:00 PM
- ⭐ **Rating:** 4.0★ on Google
- 🗺️ [Google Maps](https://maps.app.goo.gl/2addF8ZLpYViQHhi6)

---

## 🚀 Quick Start (3 Steps)

### 1️⃣ Install Dependencies
```bash
npm install
```

### 2️⃣ Run Locally
```bash
npm run dev
```
Opens at: **http://localhost:3000**

### 3️⃣ Build for Production
```bash
npm run build
```

---

## 🌐 Deploy to GitHub Pages (FREE)

### Method 1: Automatic Deployment

**Step 1:** Update `vite.config.js`
```javascript
export default defineConfig({
  base: '/pr-unisex-salon/',  // Your repo name
  plugins: [react()],
})
```

**Step 2:** Add deployment script to `package.json`
```json
{
  "scripts": {
    "predeploy": "npm run build",
    "deploy": "gh-pages -d dist"
  }
}
```

**Step 3:** Install gh-pages
```bash
npm install --save-dev gh-pages
```

**Step 4:** Deploy
```bash
npm run deploy
```

**Your site will be live at:** `https://yourusername.github.io/pr-unisex-salon/`

### Method 2: Manual Deployment

1. Build the project: `npm run build`
2. Go to GitHub repository → Settings → Pages
3. Source: Deploy from a branch
4. Branch: Select `gh-pages` and `/root` folder
5. Save

---

## 🌟 Deploy to Netlify (RECOMMENDED - FREE)

### Option A: Drag & Drop (Easiest)

1. Run `npm run build`
2. Go to [Netlify Drop](https://app.netlify.com/drop)
3. Drag the `dist` folder
4. Done! Your site is live

### Option B: Connect GitHub (Automatic Updates)

1. Go to [Netlify](https://app.netlify.com)
2. Click "Add new site" → "Import an existing project"
3. Choose "GitHub" and select your repository
4. Build settings:
   - **Build command:** `npm run build`
   - **Publish directory:** `dist`
5. Click "Deploy site"

**Custom Domain:** Netlify Settings → Domain management → Add custom domain

---

## 🎯 Deploy to Vercel (FREE)

### Via GitHub
1. Go to [Vercel](https://vercel.com)
2. Click "Add New" → "Project"
3. Import your GitHub repository
4. Vercel auto-detects Vite settings
5. Click "Deploy"

### Via CLI
```bash
npm install -g vercel
vercel login
vercel --prod
```

---

## 📂 Project Structure

```
pr-unisex-salon-website/
├── public/                          # Static files
├── src/
│   ├── components/
│   │   └── PRUnisexSalon.jsx       # Main component
│   ├── App.jsx                     # App entry
│   ├── main.jsx                    # React entry
│   └── index.css                   # Global styles
├── index.html                       # HTML template
├── package.json                     # Dependencies
├── vite.config.js                  # Vite config
├── tailwind.config.js              # Tailwind config
└── README.md                        # This file
```

---

## ✨ Features

### Design
- ✅ Luxury navy & gold color scheme
- ✅ Smooth scroll animations
- ✅ Fully responsive (mobile-first)
- ✅ Premium hover effects
- ✅ Glass-morphism elements

### Sections
1. Sticky Navigation
2. Full-screen Hero
3. Why Choose PR (6 features)
4. Services Showcase (14 services)
5. Gallery
6. Testimonials (auto-carousel)
7. Location & Hours (Google Maps)
8. Booking CTAs
9. Social Media
10. Premium Footer

### Technical
- ✅ SEO optimized
- ✅ Click-to-call & WhatsApp
- ✅ Fast loading
- ✅ Accessible
- ✅ Cross-browser compatible

---

## 🎨 Customization

### Update Contact Info
Edit `src/components/PRUnisexSalon.jsx`:
- Phone: Search `+918414916341`
- WhatsApp: Search `https://wa.me/918414916341`
- Address: Search `Near Kharsang Bridge`

### Change Colors
Edit `tailwind.config.js`:
```javascript
colors: {
  navy: '#0A1128',      // Primary
  gold: '#D4AF37',      // Accent
  cream: '#FAF9F6',     // Background
  'rose-gold': '#E0B0B0', // Secondary
}
```

### Add Real Images
Replace gradient placeholders in Gallery section with actual photos.

---

## 🔧 Scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run preview  # Preview production build
npm run lint     # Run ESLint
```

---

## 📱 Mobile Optimization

Optimized for all devices:
- 📱 Mobile (320px - 767px)
- 📱 Tablet (768px - 1023px)
- 💻 Desktop (1024px+)
- 🖥️ Large (1440px+)

---

## 🐛 Troubleshooting

### Issue: `npm install` fails
**Solution:** Use Node.js version 18 or higher
```bash
node --version  # Check version
```

### Issue: Port 3000 already in use
**Solution:** Change port in `vite.config.js`:
```javascript
server: { port: 3001 }
```

### Issue: Images not loading
**Solution:** Place images in `public` folder and reference as `/image.jpg`

---

## 📄 License

MIT License - Free to use for your business.

---

## 🙏 Built With

- **React 18** - UI Framework
- **Vite** - Build Tool
- **Tailwind CSS** - Styling
- **Lucide React** - Icons

---

## 📞 Support

Need help? Contact:
- 📧 Email: info@prunisexsalon.com
- 📞 Phone: +91 84149 16341
- 💬 WhatsApp: +91 84149 16341

---

**Made with ❤️ for PR Unisex Salon, Kharsang**
