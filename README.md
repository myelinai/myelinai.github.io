# Myelin Smart Reply Website

A beautiful, modern website for the Myelin Smart Reply Chrome extension - an AI-powered email assistant that generates intelligent, context-aware email replies for Gmail and Outlook.

## 🌟 Features

### Design & User Experience
- **Modern, Responsive Design** - Beautiful gradient backgrounds and smooth animations
- **Mobile-First Approach** - Fully responsive across all devices
- **Smooth Animations** - Intersection Observer animations and hover effects
- **Accessibility Focused** - WCAG compliant with keyboard navigation and screen reader support

### Interactive Elements
- **Floating Email Demo** - Animated email interface showing the extension in action
- **Counter Animations** - Animated statistics that count up when scrolled into view
- **Typing Effect** - Email reply content types out dynamically
- **Parallax Scrolling** - Subtle parallax effects for visual depth
- **Hover Effects** - Interactive cards and buttons with smooth transitions

### Sections
1. **Hero Section** - Compelling headline with call-to-action buttons
2. **Features** - Six key features with icons and descriptions
3. **How It Works** - Three-step process explanation
4. **Pricing** - Three-tier pricing structure (Free, Pro, Enterprise)
5. **Support** - Documentation, FAQ, and contact options
6. **Download** - Final call-to-action for Chrome extension
7. **Footer** - Links, social media, and legal information

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- A web server (for local development)

### Installation

1. **Navigate to the website folder**
2. **Start a local server** (recommended for development)

#### Using Python (if installed):
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

#### Using Node.js (if installed):
```bash
# Install a simple server
npm install -g http-server

# Start the server
http-server
```

#### Using VS Code:
Install the "Live Server" extension and right-click `index.html` → "Open with Live Server"

3. **Open your browser** and navigate to `http://localhost:8000`

## 📁 File Structure

```
website/
├── index.html          # Main HTML file
├── styles.css          # CSS styles and animations
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## 🎨 Customization

### Colors
The website uses a consistent color palette defined in CSS variables. Main colors:
- **Primary**: `#667eea` (Blue)
- **Secondary**: `#764ba2` (Purple)
- **Background**: `#f8fafc` (Light gray)
- **Text**: `#1a202c` (Dark gray)

### Fonts
- **Primary**: Inter (Google Fonts)
- **Fallback**: System fonts (San Francisco, Segoe UI, etc.)

### Animations
- **Duration**: 0.3s for hover effects, 0.6s for scroll animations
- **Easing**: `ease` for smooth transitions
- **Parallax**: Subtle movement on scroll for visual interest

## 🔧 Technical Details

### Performance Optimizations
- **Lazy Loading** - Images load only when needed
- **Intersection Observer** - Efficient scroll-based animations
- **CSS Transforms** - Hardware-accelerated animations
- **Minimal Dependencies** - Only Font Awesome for icons

### Browser Support
- **Modern Browsers**: Chrome 60+, Firefox 55+, Safari 12+, Edge 79+
- **Mobile**: iOS Safari 12+, Chrome Mobile 60+
- **Fallbacks**: Graceful degradation for older browsers

### Accessibility Features
- **Keyboard Navigation** - Full keyboard support
- **Screen Reader Support** - Proper ARIA labels and semantic HTML
- **Focus Management** - Visible focus indicators
- **Skip Links** - Quick navigation for assistive technology users
- **Color Contrast** - WCAG AA compliant color ratios

## 📱 Mobile Responsiveness

The website is fully responsive with breakpoints at:
- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px
- **Small Mobile**: Below 480px

### Mobile Features
- **Hamburger Menu** - Collapsible navigation
- **Touch-Friendly** - Large touch targets
- **Optimized Layout** - Single-column layout on mobile
- **Fast Loading** - Optimized for slower connections

## 🎯 SEO Optimization

### Meta Tags
- **Title**: "Myelin Smart Reply - AI-Powered Email Assistant"
- **Description**: Comprehensive meta description for search engines
- **Viewport**: Responsive viewport settings
- **Charset**: UTF-8 encoding

### Semantic HTML
- **Proper Headings** - H1, H2, H3 hierarchy
- **Landmark Elements** - nav, main, section, footer
- **Alt Text** - Descriptive alt attributes for images

## 🚀 Deployment

### GitHub Pages
1. Push your code to a GitHub repository
2. Go to Settings → Pages
3. Select source branch (usually `main`)
4. Your site will be available at `https://username.github.io/repository-name`

### Netlify
1. Drag and drop the website folder to Netlify
2. Or connect your GitHub repository
3. Automatic deployment on every push

### Vercel
1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your project directory
3. Follow the prompts for deployment

## 🔍 Analytics & Tracking

### Google Analytics (Optional)
Add Google Analytics by including the tracking code in the `<head>` section:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🛠️ Development

### Adding New Sections
1. Add HTML structure in `index.html`
2. Style the section in `styles.css`
3. Add animations in `script.js` if needed

### Modifying Colors
Update the CSS custom properties in `styles.css`:

```css
:root {
  --primary-color: #667eea;
  --secondary-color: #764ba2;
  --background-color: #f8fafc;
  --text-color: #1a202c;
}
```

### Adding Animations
Use the existing Intersection Observer pattern:

```javascript
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if (entry.isIntersecting) {
      entry.target.classList.add('animate');
    }
  });
});

document.querySelectorAll('.your-element').forEach(el => {
  observer.observe(el);
});
```

## 📞 Support

For questions or issues with the website:
- **Documentation**: Check this README file
- **Issues**: Create an issue in the repository
- **Contact**: Reach out through the website's contact form

## 📄 License

This website is part of the Myelin Smart Reply project. Please refer to the main project license for usage terms.

## 🙏 Acknowledgments

- **Font Awesome** - Icons
- **Google Fonts** - Inter font family
- **Modern CSS** - Grid, Flexbox, and CSS animations
- **Intersection Observer API** - Scroll-based animations

---

**Built with ❤️ for the Myelin Smart Reply Chrome extension** 