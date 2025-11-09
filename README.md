# SmartSpend - Pure HTML/CSS Landing Page

## 🎨 Overview

A complete, production-ready landing page for SmartSpend UPI Expense Tracker built with **pure HTML and CSS only** - no JavaScript frameworks or libraries required.

## 📁 Files

```
public/
├── index.html    # Main HTML file with all sections
├── styles.css    # Complete CSS styling and animations
└── README-HTML.md # This file
```

## ✨ Features

### Complete Sections
- ✅ Sticky Navigation with CSS-only mobile menu
- ✅ Hero section with animated phone mockup
- ✅ 3-step "How It Works" section
- ✅ 6 feature cards with hover effects
- ✅ Interactive demo with sample transactions and charts
- ✅ Pricing cards (Free & Premium)
- ✅ Trust & Security section
- ✅ FAQ with CSS-only accordion
- ✅ Footer with links and social media
- ✅ CSS-only modal for "Connect UPI"

### Design System
- **Colors**: Electric blue (#0066FF), Coral (#FF6B6B), Mint green (#00C48C)
- **Fonts**: Poppins (headings), Inter (body text)
- **Animations**: Float, slide-up, fade-in, scale-in
- **Responsive**: Mobile-first design with breakpoints

### Pure CSS Features
- ✓ Hamburger menu (no JavaScript)
- ✓ Accordion FAQ (using `<details>`)
- ✓ Modal dialog (using `:target` pseudo-class)
- ✓ Smooth animations and transitions
- ✓ Hover effects and micro-interactions
- ✓ Progress bars and charts (CSS gradients)

## 🚀 How to Use

### Option 1: Direct File Access
1. Open `public/index.html` directly in your browser
2. All styles are linked from `styles.css`

### Option 2: Local Server (Recommended)
```bash
# Using Python 3
cd public
python -m http.server 8000

# Using PHP
cd public
php -S localhost:8000

# Using Node.js (http-server)
npx http-server public -p 8000
```

Then visit: `http://localhost:8000`

### Option 3: Deploy to Any Static Host
Upload the `public` folder to:
- **Netlify**: Drag & drop the folder
- **Vercel**: Deploy via CLI or dashboard
- **GitHub Pages**: Push to a repo and enable Pages
- **Any web server**: Upload via FTP/SFTP

## 🎯 Key Interactions

### Navigation
- Desktop: Standard horizontal menu
- Mobile: Click hamburger icon (pure CSS checkbox hack)

### FAQ Section
- Click any question to expand/collapse
- Uses native `<details>` and `<summary>` elements

### Modal
- Click "Get Started" or pricing buttons
- Modal opens with `#modal` anchor
- Click X or outside to close (link to `#`)

### Charts
- Static CSS-based visualizations
- Pie chart: CSS conic-gradient
- Bar chart: Flex layout with height percentages
- Progress bars: Animated width transitions

## 🎨 Customization

### Colors
Edit CSS variables in `styles.css`:
```css
:root {
    --primary: #0066FF;      /* Main brand color */
    --secondary: #FF6B6B;    /* Accent/alerts */
    --success: #00C48C;      /* Success states */
    --background: #FFF8F0;   /* Page background */
}
```

### Fonts
Change Google Fonts import in `index.html` `<head>`:
```html
<link href="https://fonts.googleapis.com/css2?family=YourFont:wght@400;700&display=swap" rel="stylesheet">
```

Then update CSS:
```css
--font-display: 'YourFont', sans-serif;
```

### Content
All text is directly in `index.html` - simply find and replace:
- Hero headline: Line ~60
- Feature descriptions: Lines ~180-280
- Pricing details: Lines ~500-600
- FAQ questions: Lines ~680-750

## 📊 Charts & Data

### Transaction Data
Edit in `index.html` lines ~340-390:
```html
<div class="transaction-row">
    <strong>Merchant Name</strong>
    <span class="badge">Category</span>
    <span class="amount-primary">₹Amount</span>
</div>
```

### Budget Bars
Adjust progress width in `index.html` lines ~450-480:
```html
<div class="progress-fill" style="width: 75%;"></div>
```

### Pie Chart
Modify conic-gradient percentages in `styles.css`:
```css
.pie-chart {
    background: conic-gradient(
        from 0deg,
        #FF6B6B 0% 67%,    /* Housing */
        #00C48C 67% 83%,   /* Savings */
        #0066FF 83% 96%,   /* Shopping */
        #FF9800 96% 100%   /* Food */
    );
}
```

## 📱 Responsive Breakpoints

```css
/* Desktop: Default styles */
/* Tablet: max-width: 1024px */
/* Mobile: max-width: 768px */
/* Small: max-width: 640px */
```

## ♿ Accessibility

- ✓ Semantic HTML5 elements
- ✓ ARIA labels for icons
- ✓ Keyboard navigation support
- ✓ Focus states on interactive elements
- ✓ Sufficient color contrast (WCAG AA)
- ✓ Alt text for important visuals

## 🔧 Browser Support

Tested and working on:
- ✅ Chrome/Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

Note: Older browsers may need prefixes for:
- CSS Grid
- Flexbox
- CSS Variables
- `backdrop-filter`

## 📦 File Size

- `index.html`: ~25KB (uncompressed)
- `styles.css`: ~30KB (uncompressed)
- **Total**: ~55KB (compresses to ~15KB with gzip)

## 🎓 Learning Resources

This project demonstrates:
1. **CSS Grid & Flexbox** for responsive layouts
2. **CSS Variables** for maintainable design systems
3. **CSS Animations** without JavaScript
4. **Semantic HTML** for better SEO and accessibility
5. **CSS-only interactions** (modals, accordions, menus)

## 📝 License

This code is provided as a template for the SmartSpend project.

## 🆘 Troubleshooting

**Styles not loading?**
- Check that `styles.css` is in the same folder as `index.html`
- Verify the `<link>` tag path in HTML

**Fonts not showing?**
- Ensure internet connection (Google Fonts loads from CDN)
- Check browser console for errors

**Mobile menu not working?**
- Ensure checkbox input and label are present
- Check that `menu-toggle` ID matches

**Charts not displaying?**
- Verify CSS gradient syntax
- Check browser support for `conic-gradient`

## 📞 Support

For questions or issues with this HTML/CSS version:
- Check the inline HTML comments
- Review CSS class names in `styles.css`
- Inspect elements in browser DevTools

---

**Built with ❤️ using pure HTML & CSS**
