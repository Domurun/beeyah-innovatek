# Beeyah InnovaTek Website

A modern, fully responsive **Single Page Application (SPA)** showcasing Beeyah InnovaTek's innovative technology solutions.

**Live Site:** [your-domain.com](https://your-domain.com)  
**Status:** ✅ Production Ready

---

## 🎯 Features

✨ **Multi-Page Navigation** - 9 seamless pages (Home, Portfolio, Services, About, Blog, Careers, Privacy, Terms, Support)  
📱 **Fully Responsive** - Mobile-first design with Tailwind CSS  
🎨 **Modern UI/UX** - Clean, professional, accessible interface  
🔍 **Portfolio Filtering** - Dynamic project filtering by category (Web & App, Branding, Cloud/DevOps, System Design)  
📝 **Blog Filtering** - Article filtering by topic (Technology, Sustainability, Design, Cloud)  
📋 **Interactive Forms** - Contact, Newsletter, and Support forms with validation  
🎭 **Mobile-Optimized Menu** - Smooth hamburger navigation for mobile devices  
♿ **Accessible** - WCAG compliant with semantic HTML  
⚡ **Zero Dependencies** - No build tools required, pure HTML/CSS/JS  

---

## 🛠 Tech Stack

| Technology | Purpose |
|-----------|---------|
| **HTML5** | Semantic markup |
| **Tailwind CSS** | Utility-first styling via CDN |
| **Vanilla JavaScript** | Dynamic navigation & filtering |
| **Google Fonts** | Montserrat & Open Sans typography |

---

## 📁 Project Structure

```
beeyah-innovatek/
├── index.html              # Main SPA file (all pages included)
├── .gitignore              # Git ignore rules
├── README.md               # This file
├── LICENSE                 # MIT License
└── assets/
    └── img/
        ├── BEEYAH.png      # Company logo
        └── the team/
            └── IMG_9956p.jpg  # Team photo
```

---

## 🚀 Getting Started

### Option 1: Local Development

```bash
# Clone the repository
git clone https://github.com/yourusername/beeyah-innovatek.git
cd beeyah-innovatek

# Open in browser (simple method)
# Windows: start index.html
# Mac: open index.html
# Linux: xdg-open index.html
```

### Option 2: Local Server

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (npx)
npx serve

# Then visit: http://localhost:8000
```

---

## 📄 Pages & Features

| Page | Purpose | Key Features |
|------|---------|--------------|
| **Home** | Landing page | Hero, Services overview, Portfolio highlights, Featured blog post, Newsletter signup |
| **Portfolio** | Work showcase | 6+ projects with category filtering (All, Web & App, Branding, Cloud/DevOps, System Design) |
| **Services** | Solution details | 3 core services with descriptions, process flow (Discover → Design → Develop → Deploy) |
| **About Us** | Company info | Mission & Vision, Core values, Leadership team |
| **Blog** | Thought leadership | 4+ articles with category filtering (Technology, Sustainability, Design, Cloud) |
| **Careers** | Job board | Company culture, 3 open positions with "Apply Now" buttons |
| **Privacy Policy** | Legal | Data handling & user rights |
| **Terms of Use** | Legal | Usage terms & IP rights |
| **Support** | Help center | FAQs (5+ questions) + Support ticket form |

---

## 🎨 Design System

### Brand Colors

```css
Primary Color (Charcoal): #34495E
Accent Color (Light Blue): #3498DB
```

### Typography

- **Headings:** Montserrat (400, 600, 700)
- **Body:** Open Sans (400, 600)
- **Font Loading:** Google Fonts CDN

### Components

- ✅ Sticky Header with Mobile Menu
- ✅ Hero Section with CTA
- ✅ Feature Cards (3-4 column grid)
- ✅ Portfolio/Blog Cards with Images
- ✅ Filter Buttons (active state styling)
- ✅ Forms (Contact, Newsletter, Support)
- ✅ Accordion/Collapsible FAQs
- ✅ Footer with Quick Links & Social Icons
- ✅ Responsive Grid Layouts

---

## 🎯 Form Integration

Forms currently show **local success messages**. To send real submissions:

### Option A: Formspree (Recommended)
```javascript
// In contactForm submit handler, replace the setTimeout with:
fetch('https://formspree.io/f/YOUR_FORM_ID', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify(formData)
})
.then(response => response.json())
.then(data => {
    showStatus(formStatus, 'Success! We'll be in touch soon.', true);
    contactForm.reset();
})
.catch(error => {
    showStatus(formStatus, 'Error sending form. Please try again.', false);
});
```

### Option B: EmailJS
```javascript
emailjs.init('YOUR_PUBLIC_KEY');
emailjs.send('SERVICE_ID', 'TEMPLATE_ID', formData);
```

### Option C: Your Backend API
```javascript
fetch('/api/contact', {
    method: 'POST',
    body: JSON.stringify(formData)
})
```

---

## 📱 Mobile Responsiveness

- ✅ Breakpoints: 640px (sm), 768px (md), 1024px (lg)
- ✅ Mobile Menu Overlay (slides from right)
- ✅ Touch-friendly buttons & spacing
- ✅ Optimized images & typography scaling
- ✅ Tested on: iPhone, Android, iPad, Desktop

---

## ♿ Accessibility Features

- ✅ Semantic HTML (`<header>`, `<main>`, `<footer>`, `<nav>`)
- ✅ ARIA labels for screen readers
- ✅ `sr-only` class for hidden text
- ✅ Color contrast ratios (WCAG AA compliant)
- ✅ Keyboard navigation support
- ✅ Form labels properly associated with inputs

---

## 🚢 Deployment Options

### GitHub Pages (Free)
```bash
# Push to GitHub, then enable Pages in repository settings
# Site will be live at: https://yourusername.github.io/beeyah-innovatek
```

### Netlify (Recommended)
1. Sign up at [netlify.com](https://netlify.com)
2. Connect your GitHub repo
3. Auto-deploys on every push
4. Custom domain support

### Vercel
1. Sign up at [vercel.com](https://vercel.com)
2. Import your GitHub repo
3. Instant deployment

### Traditional Hosting
- Upload `index.html` + `assets/` folder to any web host
- Works on Apache, Nginx, IIS, etc.

---

## 📊 Performance

- ⚡ **No build step required** - Single HTML file
- 🎯 **Lightweight** - Only Tailwind CDN dependency
- 🚀 **Fast navigation** - Client-side routing
- 📦 **Optimized images** - Using placeholder service for prototypes

---

## 🛣 Browser Support

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | Latest | ✅ Full support |
| Firefox | Latest | ✅ Full support |
| Safari | Latest | ✅ Full support |
| Edge | Latest | ✅ Full support |
| Mobile Safari | iOS 12+ | ✅ Full support |
| Chrome Mobile | Android 5+ | ✅ Full support |

---

## 📝 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 👥 Team

**Beeyah InnovaTek**
- **CEO:** Emmanuel Beeyah
- **Locations:** Lagos, Nigeria 🇳🇬 | Dallas, USA 🇺🇸

---

## 📧 Contact & Support

**General Inquiries**  
📧 info@beeyahinnovatek.com

**Careers**  
📧 careers@beeyahinnovatek.com

**Privacy & Legal**  
📧 privacy@beeyahinnovatek.com

**Support Portal**  
🔗 [Support Page](https://yourdomain.com/#support)

---

## 🔗 Social Media

- 🐦 [X/Twitter](https://x.com/beeyahinnovatek)
- 💼 [LinkedIn](https://www.linkedin.com/in/beeyah-innovatek-707557378)
- 📸 [Instagram](https://www.instagram.com/beeyahinnovatek)

---

## 📈 Roadmap

- [ ] Blog CMS integration
- [ ] Contact form backend API
- [ ] Analytics dashboard
- [ ] Dark mode toggle
- [ ] Multi-language support (EN, FR, YO)
- [ ] Video testimonials
- [ ] Case study detail pages

---

**Last Updated:** November 13, 2025  
**Built with ❤️ by Beeyah InnovaTek**