# Machine Learning Portfolio Website

A modern, responsive portfolio website showcasing Machine Learning projects, built with pure HTML, CSS, and JavaScript.

## 🌟 Features

- **Stunning Video Background**: Dynamic background with animated gradients
- **Fully Responsive**: Works seamlessly on desktop, tablet, and mobile devices
- **Modern UI/UX**: Glass-morphism design with smooth animations
- **Project Showcase**: Dedicated section for ML/DL projects
- **Interactive Navigation**: Smooth scrolling and active link highlighting
- **Professional Layout**: Hero section, about, skills, projects, journey timeline, and contact sections

## 🎨 Design Highlights

- Custom color scheme with purple and green accents
- Animated gradient overlays
- Scroll reveal animations
- Hover effects and transitions
- Mobile-friendly hamburger menu
- Glass-morphism card designs

## 📋 Sections

1. **Hero Section**: Introduction with CTA buttons and profile card
2. **About**: Personal background and academic details
3. **Skills**: Tech stack and ML capabilities
4. **Projects**: 6 featured ML/DL projects with descriptions
5. **Journey**: Timeline of learning progression
6. **Internship**: Details about industry experience
7. **Contact**: Contact information and social links

## 🚀 Projects Featured

1. **Student Performance Prediction** - Linear Regression
2. **Breast Cancer Detection (Logistic Regression)** - Healthcare Classification
3. **Customer Segmentation** - K-Means Clustering
4. **Breast Cancer Detection (Random Forest)** - Advanced Classification
5. **Spam Detection** - Naive Bayes & TF-IDF
6. **Credit Card Fraud Detection** - Random Forest & XGBoost

## 🛠️ Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Custom properties, Grid, Flexbox, animations
- **JavaScript**: Vanilla JS for interactivity
- **Google Fonts**: Poppins font family
- **Video Background**: Embedded video for dynamic effect

## 📱 Responsive Breakpoints

- Desktop: > 900px
- Tablet: 720px - 900px
- Mobile: < 720px
- Small Mobile: < 480px

## 🎯 Quick Start

### Option 1: Direct Usage
1. Copy the HTML code
2. Save as `index.html`
3. Open in any modern web browser

### Option 2: GitHub Pages
1. Create a new repository
2. Upload `index.html`
3. Go to Settings → Pages
4. Select main branch as source
5. Your site will be live at `https://username.github.io/repo-name`

### Option 3: Local Development
```bash
# Simply open the file
open index.html

# Or use a local server (recommended)
python -m http.server 8000
# Visit http://localhost:8000
```

## 📝 Customization Guide

### Update Personal Information

1. **Name & Details** (Line 182):
```html
<h1>
  Hi, I'm <span class="highlight">YOUR NAME</span><br/>
  CSE 8th Semester · ML Enthusiast
</h1>
```

2. **Email** (Line 692):
```html
<div class="contact-item">📧 your.email@gmail.com</div>
```

3. **Social Links** (Lines 699-702):
```html
<a href="YOUR_GITHUB_URL">💻 GitHub</a>
<a href="YOUR_LINKEDIN_URL">🔗 LinkedIn</a>
```

### Change Colors

Update CSS variables in `:root` (Lines 13-24):
```css
:root {
  --accent: #7c3aed;        /* Primary purple */
  --accent-2: #22c55e;      /* Secondary green */
  --bg: #050816;            /* Background */
  --text: #e5e7eb;          /* Text color */
}
```

### Add/Remove Projects

Project cards start at line 524. Use this template:
```html
<article class="project-card">
  <div class="project-pill">Category · Domain</div>
  <h3 class="project-title">Project Name</h3>
  <p class="project-desc">Description here...</p>
  <div class="project-meta">
    <div class="project-tech">
      <span>Tech1</span>
      <span>Tech2</span>
    </div>
    <div class="project-links">
      <a href="GITHUB_URL">🔗 GitHub Repo</a>
    </div>
  </div>
</article>
```

### Change Video Background

Replace video source (Line 651):
```html
<video class="video-bg" autoplay muted loop playsinline>
  <source src="YOUR_VIDEO_URL.mp4" type="video/mp4">
</video>
```

**Free Video Sources:**
- [Pexels Videos](https://www.pexels.com/videos/)
- [Pixabay Videos](https://pixabay.com/videos/)
- [Videvo](https://www.videvo.net/)

## 🎨 Color Schemes (Alternatives)

### Blue Theme
```css
--accent: #3b82f6;
--accent-2: #10b981;
```

### Orange Theme
```css
--accent: #f97316;
--accent-2: #06b6d4;
```

### Pink Theme
```css
--accent: #ec4899;
--accent-2: #8b5cf6;
```

## 📊 Performance Tips

1. **Optimize Video**:
   - Use compressed MP4 format
   - Max resolution: 1920x1080
   - Keep file size under 5MB

2. **Lazy Loading**:
```html
<video loading="lazy" preload="metadata">
```

3. **Font Optimization**:
```html
<link rel="preconnect" href="https://fonts.googleapis.com">
```

## 🔧 Browser Support

- ✅ Chrome (Latest)
- ✅ Firefox (Latest)
- ✅ Safari (Latest)
- ✅ Edge (Latest)
- ⚠️ IE11 (Limited support)

## 📱 Mobile Features

- Touch-friendly navigation
- Optimized card layouts
- Responsive typography
- Hamburger menu
- Smooth scroll behavior

## 🐛 Common Issues & Solutions

### Video Not Playing
```html
<!-- Add these attributes -->
<video autoplay muted loop playsinline webkit-playsinline>
```

### Animations Not Working
```javascript
// Ensure script runs after DOM load
window.addEventListener('DOMContentLoaded', function() {
  // Your code here
});
```

### Mobile Menu Not Closing
```javascript
// Already handled in lines 723-729
navMenu.querySelectorAll('a').forEach(link => {
  link.addEventListener('click', () => {
    navToggle.classList.remove('active');
    navMenu.classList.remove('open');
  });
});
```

## 📈 SEO Optimization

Add these meta tags in `<head>`:
```html
<meta name="description" content="Machine Learning portfolio showcasing projects in Python, Scikit-learn, and Deep Learning">
<meta name="keywords" content="Machine Learning, Data Science, Python, Portfolio, CSE">
<meta name="author" content="Your Name">
<meta property="og:title" content="ML Portfolio | Your Name">
<meta property="og:description" content="Portfolio showcasing ML/DL projects">
<meta property="og:image" content="preview-image.png">
<meta property="og:url" content="https://yourwebsite.com">
```

## 🚀 Deployment Options

### 1. GitHub Pages (Free)
- Push code to GitHub
- Enable Pages in Settings
- Live in minutes

### 2. Netlify (Free)
- Drag & drop HTML file
- Automatic HTTPS
- Custom domain support

### 3. Vercel (Free)
- Import from GitHub
- Automatic deployments
- Edge network CDN

### 4. Firebase Hosting (Free)
```bash
npm install -g firebase-tools
firebase init
firebase deploy
```

## 📄 File Structure

```
portfolio/
│
├── index.html          # Main HTML file (contains all code)
├── README.md           # This file
└── assets/            # Optional folder for images
    ├── profile.jpg
    └── projects/
```

## 🎓 Learning Resources

- **HTML/CSS**: [MDN Web Docs](https://developer.mozilla.org/)
- **JavaScript**: [JavaScript.info](https://javascript.info/)
- **Responsive Design**: [CSS-Tricks](https://css-tricks.com/)
- **Animations**: [Animate.css](https://animate.style/)

## 🤝 Contributing

This is a personal portfolio template. Feel free to:
- Fork and customize
- Use as inspiration
- Share with others
- Provide feedback

## 📝 License

This project is open source and available under the MIT License.

## 🙏 Credits

- **Design**: Custom design inspired by modern portfolio trends
- **Fonts**: Google Fonts (Poppins)
- **Video**: Vimeo (example video used)
- **Icons**: Unicode emojis

## 📞 Support

For questions or suggestions:
- Open an issue on GitHub
- Contact: sujansardar1068@gmail.com
- LinkedIn: [Your Profile]

## ⚡ Quick Tips

1. **Test Locally First**: Always test changes in browser before deploying
2. **Mobile Testing**: Use browser DevTools mobile view
3. **Performance**: Compress images and optimize video
4. **Accessibility**: Use semantic HTML and ARIA labels
5. **Version Control**: Use Git to track changes

## 🔄 Version History

- **v1.0** - Initial release with all sections
- **v1.1** - Added internship section
- **v1.2** - Mobile optimization improvements

---

**Made with ❤️ for Machine Learning enthusiasts and CSE students**

*Last Updated: December 2024*
