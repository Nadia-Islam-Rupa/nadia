# 🌟 Nadia's Portfolio Website

A modern, responsive, and dynamic portfolio website built with pure HTML5, CSS3, and vanilla JavaScript. Features dark mode, smooth animations, and JSON-based content management.

## ✨ Features

### 🎨 Design & UI
- **Fully Responsive**: Optimized for all devices (mobile, tablet, desktop)
- **Dark Mode**: Toggle between light and dark themes with localStorage persistence
- **Modern Aesthetics**: Clean design with gradient accents and smooth transitions
- **Interactive Animations**: Scroll animations, hover effects, and smooth transitions
- **Accessible**: Semantic HTML and ARIA labels for better accessibility

### 📋 Sections
1. **Hero Section**: Eye-catching introduction with social links and CV download
2. **About**: Personal introduction and background
3. **Skills**: Interactive skill tags with category filtering (Mobile, Backend, Tools)
4. **Education**: Beautiful timeline view of educational background
5. **Experience**: Professional experience cards with detailed responsibilities
6. **Projects**: Portfolio showcase with detailed modal popups
7. **Achievements**: Showcase of accomplishments with icons
8. **Blog**: Latest articles and blog posts
9. **Contact**: Functional contact form with validation and social links

### 🚀 Dynamic Features
- **JSON-Based Content**: All content loaded from JSON files for easy updates
- **Skill Filtering**: Filter skills by category with smooth animations
- **Project Modals**: Detailed project view in beautiful popup modals
- **Theme Toggle**: Persistent dark/light mode with smooth transitions
- **Form Validation**: Contact form with email validation
- **Mobile Menu**: Responsive hamburger menu
- **Scroll Animations**: Elements fade in as you scroll
- **Back to Top**: Quick navigation button

## 📁 Project Structure

```
nadia_portfolio_web/
├── index.html              # Main HTML file with all sections
├── css/
│   └── styles.css         # Complete styling with dark mode
├── js/
│   └── script.js          # All JavaScript functionality
├── data/                   # JSON data files
│   ├── skills.json        # Skills with categories
│   ├── education.json     # Education timeline
│   ├── experience.json    # Work experience
│   ├── projects.json      # Portfolio projects
│   └── achievements.json  # Achievements and awards
├── assets/
│   ├── images/            # Project screenshots, logos
│   └── cv/               # CV/Resume files
└── README.md             # This file
```

## 🚀 Quick Start

### Prerequisites
- A modern web browser
- A local web server (for proper JSON file loading)

### Installation

1. **Clone or download** the repository

2. **Start a local web server** (choose one):

   **Python 3:**
   ```bash
   python3 -m http.server 8000
   ```

   **Node.js (http-server):**
   ```bash
   npx http-server -p 8000
   ```

   **PHP:**
   ```bash
   php -S localhost:8000
   ```

   **VS Code Live Server:**
   - Install "Live Server" extension
   - Right-click `index.html` → "Open with Live Server"

3. **Open browser** and navigate to `http://localhost:8000`

## 📝 Content Management

### Why JSON Files?

All content is stored in JSON files for easy maintenance:
- ✅ Update content without touching code
- ✅ Separate data from presentation
- ✅ Easy to maintain and version control
- ✅ Reusable data structure
- ✅ Simple to add/remove items

### Data Files Structure

#### Skills (`data/skills.json`)
```json
{
  "skills": [
    {
      "name": "Flutter",
      "category": "mobile"
    }
  ]
}
```
**Categories**: `mobile`, `backend`, `tools`, `all`

#### Education (`data/education.json`)
```json
{
  "education": [
    {
      "degree": "Bachelor of Science in Computer Science",
      "institution": "University Name",
      "duration": "2018 - 2022",
      "description": "Brief description of studies"
    }
  ]
}
```

#### Experience (`data/experience.json`)
```json
{
  "experience": [
    {
      "title": "Senior Flutter Developer",
      "company": "Tech Company Inc.",
      "duration": "Jan 2022 - Present",
      "responsibilities": [
        "Led development of mobile applications",
        "Mentored junior developers"
      ]
    }
  ]
}
```

#### Projects (`data/projects.json`)
```json
{
  "projects": [
    {
      "id": "project1",
      "title": "E-Commerce App",
      "description": "Short description for card",
      "detailedDescription": "Full description for modal popup",
      "tags": ["Flutter", "Firebase", "Stripe"],
      "features": [
        "User authentication",
        "Payment integration"
      ],
      "technologies": [
        "Flutter",
        "Firebase",
        "Stripe API"
      ],
      "demoUrl": "https://demo.example.com",
      "sourceUrl": "https://github.com/user/repo"
    }
  ]
}
```

#### Achievements (`data/achievements.json`)
```json
{
  "achievements": [
    {
      "icon": "🏆",
      "title": "Achievement Title",
      "description": "Description of the achievement"
    }
  ]
}
```

## 🎨 Customization

### Changing Colors

Edit CSS variables in `css/styles.css`:

```css
/* Light mode colors */
:root {
    --primary-color: #667eea;
    --secondary-color: #764ba2;
    --text-color: #333;
    --bg-color: #ffffff;
    --card-bg: #ffffff;
}

/* Dark mode colors */
[data-theme="dark"] {
    --text-color: #e0e0e0;
    --bg-color: #1a1a2e;
    --card-bg: #16213e;
}
```

### Adding New Content

1. **Skills**: Add to `data/skills.json`
2. **Education**: Add to `data/education.json`
3. **Experience**: Add to `data/experience.json`
4. **Projects**: Add to `data/projects.json`
5. **Achievements**: Add to `data/achievements.json`

**No code changes needed!** The website automatically loads and displays new data.

### Adding Images

1. Add project screenshots to `assets/images/`
2. Add your CV to `assets/cv/`
3. Update image paths in JSON or HTML

### Updating Social Links

Edit social links in `index.html`:
- Search for "github.com", "linkedin.com", "medium.com"
- Replace with your profile URLs

## 🔧 Technical Details

### Technologies Used
- **HTML5**: Semantic markup, accessibility features
- **CSS3**: Custom properties, flexbox, grid, animations
- **JavaScript ES6+**: Async/await, Fetch API, DOM manipulation
- **JSON**: Data storage and management
- **SVG**: Inline icons (no external dependencies)

### JavaScript Features
- **Data Loading**: Async fetch from JSON files
- **Dynamic Rendering**: Content generated from JSON data
- **Event Handling**: Interactive features and animations
- **LocalStorage**: Theme preference persistence
- **Intersection Observer**: Scroll-based animations
- **Form Validation**: Email validation and feedback

### CSS Features
- **CSS Variables**: Easy theming and customization
- **Flexbox & Grid**: Modern layout techniques
- **Animations**: Keyframes, transitions, transforms
- **Media Queries**: Responsive breakpoints
- **Dark Mode**: Theme switching with CSS variables

## 📱 Responsive Breakpoints

```css
/* Desktop */
@media (min-width: 969px) { /* ... */ }

/* Tablet */
@media (max-width: 968px) { /* ... */ }

/* Mobile */
@media (max-width: 768px) { /* ... */ }

/* Small Mobile */
@media (max-width: 600px) { /* ... */ }
```

## 🌐 Browser Support

| Browser | Version |
|---------|---------|
| Chrome  | Latest ✅ |
| Firefox | Latest ✅ |
| Safari  | Latest ✅ |
| Edge    | Latest ✅ |
| Opera   | Latest ✅ |

## 🚀 Deployment

### Option 1: GitHub Pages
1. Push code to GitHub repository
2. Go to Settings → Pages
3. Select branch and `/root` folder
4. Save and wait for deployment

### Option 2: Netlify
1. Create Netlify account
2. Drag and drop the project folder
3. Site is live instantly!

### Option 3: Vercel
1. Create Vercel account
2. Import GitHub repository
3. Deploy with one click

### Option 4: Traditional Hosting
1. Upload all files via FTP
2. Ensure JSON MIME type is set correctly
3. Point domain to hosting

## 📊 Performance Optimization

- ✅ **No External Dependencies**: Pure vanilla JavaScript
- ✅ **Minimal HTTP Requests**: All code in 3 files + JSON
- ✅ **CSS Animations**: Hardware-accelerated transforms
- ✅ **Lazy Loading**: Images load as needed
- ✅ **Minification Ready**: Can minify CSS/JS for production

### Production Checklist
- [ ] Minify `css/styles.css`
- [ ] Minify `js/script.js`
- [ ] Optimize images (WebP format)
- [ ] Add favicon
- [ ] Update meta tags
- [ ] Test on all devices
- [ ] Check console for errors
- [ ] Validate HTML/CSS

## 🐛 Troubleshooting

### JSON Files Not Loading?
- **Issue**: CORS errors in browser console
- **Solution**: Use a local web server (not file:// protocol)

### Dark Mode Not Persisting?
- **Issue**: Theme resets on page reload
- **Solution**: Check browser localStorage is enabled

### Projects Not Showing?
- **Issue**: Empty project section
- **Solution**: Check JSON file syntax and console errors

### Modal Not Opening?
- **Issue**: Click on "View Details" does nothing
- **Solution**: Ensure project IDs match in JSON and HTML

## 🎯 Future Enhancements

- [ ] Add blog post content from JSON
- [ ] Implement project search/filter
- [ ] Add testimonials section
- [ ] Integrate analytics
- [ ] Add service worker for PWA
- [ ] Multi-language support
- [ ] Contact form backend integration
- [ ] Add more animation effects

## 🤝 Contributing

This is a personal portfolio template. Feel free to:
- Fork and customize for your own use
- Suggest improvements via issues
- Share with others

## 📄 License

This project is open source and available for personal and commercial use. No attribution required, but appreciated!

## 👤 Author

**Nadia Islam Rupa**
- GitHub: [Your GitHub Profile]
- LinkedIn: [Your LinkedIn Profile]
- Medium: [Your Medium Profile]
- Email: your.email@example.com

## 🙏 Acknowledgments

- Built with modern web technologies
- No frameworks or libraries required
- Pure vanilla JavaScript for maximum performance
- Responsive design principles
- Accessibility best practices

---

**Built with ❤️ using HTML, CSS & JavaScript**

**Last Updated**: December 2025

## 📖 Additional Resources

- [MDN Web Docs](https://developer.mozilla.org/)
- [CSS-Tricks](https://css-tricks.com/)
- [JavaScript.info](https://javascript.info/)

## 💡 Tips for Customization

1. **Start with Data**: Update all JSON files with your information
2. **Replace Placeholders**: Update social links and contact info
3. **Add Images**: Replace project screenshots and profile images
4. **Test Locally**: Always test with a local server before deploying
5. **Customize Colors**: Match your personal brand colors
6. **Review Content**: Proofread all text before going live

---

**Need Help?** Check the troubleshooting section or open an issue!

**Enjoying this template?** Give it a ⭐ on GitHub!
