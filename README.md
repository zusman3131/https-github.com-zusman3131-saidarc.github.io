# Arc Raiders Guide Website

A comprehensive, beginner-friendly guide website for Arc Raiders - featuring weapons database, maps, crafting recipes, extraction strategies, and more.

## 🚀 Live Demo

Visit the live site: [https://arcraiders.guide](https://arcraiders.guide)

## 📁 Project Structure

```
arc-raiders-website/
├── index.html          # Homepage with quick links and overview
├── weapons.html        # Complete weapons database (21 weapons)
├── maps.html           # Detailed map guides for all 4 locations
├── crafting.html       # Crafting recipes and material sources
├── extraction.html     # Extraction strategies and tips
├── guides.html         # Beginner guides, combat tips, FAQ
├── css/
│   ├── style.css       # Source stylesheet (development)
│   └── style.min.css   # Minified stylesheet (production)
├── js/
│   └── main.js         # Interactive features and filtering
├── data/
│   └── weapons.json    # Weapon data for dynamic features
├── images/             # Image assets folder
└── README.md           # This file
```

## ✨ Features

- **📱 Fully Responsive**: Works seamlessly on desktop, tablet, and mobile devices
- **⚡ Performance Optimized**: Minified CSS, preconnect hints, font-display swap
- **🔍 SEO Ready**: Complete meta tags, Open Graph, Twitter Cards, canonical URLs
- **♿ Accessible**: Semantic HTML, ARIA labels, keyboard navigation
- **🎨 Modern Design**: Dark theme with accent colors, smooth animations
- **🔧 Interactive**: Weapon filtering, mobile navigation, smooth scrolling

## 🛠️ Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom properties, Grid, Flexbox
- **Vanilla JavaScript** - No frameworks required
- **Google Fonts** - Inter & Rajdhani

## 🚀 Deployment

### Option 1: Static Hosting (Recommended)

Deploy to any static hosting service:

- **Vercel**: `vercel --prod`
- **Netlify**: Drag and drop the folder or use `netlify deploy --prod`
- **GitHub Pages**: Push to a repository and enable Pages
- **Cloudflare Pages**: Connect your Git repository
- **AWS S3 + CloudFront**: Upload files to S3 bucket with static hosting

### Option 2: Traditional Web Hosting

1. Upload all files to your web server's public directory
2. Ensure `.html` files are served with correct MIME type
3. Configure gzip compression for text files

### Option 3: Local Development

```bash
# Clone or download the project
cd arc-raiders-website

# Serve with Python
python3 -m http.server 8000

# Or with Node.js
npx serve .

# Or with PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## 📋 Pre-Deployment Checklist

- [ ] Update canonical URLs in all HTML files to your actual domain
- [ ] Replace Open Graph image URLs (`og-image.jpg`, etc.) with actual images
- [ ] Add favicon.ico or update the SVG favicon data URI
- [ ] Test all internal links work correctly
- [ ] Verify mobile responsiveness
- [ ] Run Lighthouse audit for performance
- [ ] Enable gzip compression on your server
- [ ] Set up HTTPS (SSL certificate)

## 🎨 Customization

### Colors

Edit CSS custom properties in `css/style.css`:

```css
:root {
    --color-primary: #ff6b35;      /* Orange accent */
    --color-bg-primary: #0a0b0f;    /* Dark background */
    --color-text-primary: #f5f5f5;  /* White text */
    /* ... more variables */
}
```

### Content

- **Weapons**: Edit `weapons.html` to add/remove weapons
- **Maps**: Edit `maps.html` to update map information
- **Crafting**: Edit `crafting.html` for new recipes
- **Guides**: Edit `guides.html` for tips and FAQ

## 🔍 SEO Configuration

Each page includes comprehensive SEO meta tags:

- Title and description optimized for search engines
- Open Graph tags for social sharing
- Twitter Card tags
- Canonical URLs to prevent duplicate content
- Robots meta for indexing control

Update the following in each HTML file:
1. `content` attributes in Open Graph meta tags
2. `href` in canonical link tags
3. Image URLs for social sharing

## ⚡ Performance Optimizations

- ✅ Minified CSS (23% size reduction)
- ✅ Preconnect to Google Fonts domain
- ✅ DNS prefetch for external resources
- ✅ Font-display swap for faster text rendering
- ✅ CSS preloading for critical path
- ✅ Semantic HTML for faster parsing
- ✅ No render-blocking JavaScript

## 🌐 Browser Support

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+
- iOS Safari 13+
- Chrome for Android 80+

## 📝 Content Updates

To update weapon data or add new content:

1. Edit the relevant HTML file
2. Follow existing CSS class naming conventions
3. Test responsiveness at 320px, 768px, and 1200px+ breakpoints
4. Validate HTML at [validator.w3.org](https://validator.w3.org/)

## 📄 License

This project is a fan-made guide and is **not affiliated with Embark Studios**.

Arc Raiders is a trademark of Embark Studios. All game content belongs to their respective owners.

## 🤝 Contributing

This is a community guide. Suggestions and improvements are welcome!

## 📧 Contact

For questions or suggestions about this guide, please open an issue or contact the maintainer.

---

**Built with ❤️ for the Arc Raiders community**
