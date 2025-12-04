# Quick Content Update Guide

This guide helps you quickly update your portfolio content without touching any code.

## 📝 Table of Contents
- [Updating Skills](#updating-skills)
- [Updating Education](#updating-education)
- [Updating Experience](#updating-experience)
- [Updating Projects](#updating-projects)
- [Updating Achievements](#updating-achievements)
- [Updating Blog Posts](#updating-blog-posts)
- [Updating Personal Info](#updating-personal-info)
- [Adding Images](#adding-images)

---

## 🎯 Updating Skills

**File**: `data/skills.json`

### Add a New Skill
```json
{
  "name": "React Native",
  "category": "mobile"
}
```

**Categories**: `mobile`, `backend`, `tools`

### Example
```json
{
  "skills": [
    {
      "name": "Flutter",
      "category": "mobile"
    },
    {
      "name": "Node.js",
      "category": "backend"
    },
    {
      "name": "Git",
      "category": "tools"
    }
  ]
}
```

---

## 🎓 Updating Education

**File**: `data/education.json`

### Add Education Entry
```json
{
  "degree": "Master of Science in Software Engineering",
  "institution": "MIT",
  "duration": "2022 - 2024",
  "description": "Specialized in mobile computing and distributed systems"
}
```

### Tips
- Keep descriptions concise (1-2 sentences)
- Use clear date ranges
- Most recent education first

---

## 💼 Updating Experience

**File**: `data/experience.json`

### Add Work Experience
```json
{
  "title": "Senior Mobile Developer",
  "company": "Tech Corp Inc.",
  "duration": "Jan 2023 - Present",
  "responsibilities": [
    "Led development of flagship mobile application",
    "Mentored team of 5 junior developers",
    "Implemented CI/CD pipeline reducing deployment time by 60%"
  ]
}
```

### Best Practices
- Start with most recent position
- Use action verbs (Led, Developed, Implemented)
- Include measurable achievements
- 3-5 responsibilities per role

---

## 🚀 Updating Projects

**File**: `data/projects.json`

### Add a New Project
```json
{
  "id": "project5",
  "title": "Fitness Tracking App",
  "description": "Mobile app for tracking workouts and nutrition",
  "detailedDescription": "A comprehensive fitness tracking application built with Flutter. Features include workout logging, nutrition tracking, progress analytics, social challenges, and integration with wearable devices. Uses Firebase for real-time data sync and ML Kit for exercise recognition.",
  "tags": ["Flutter", "Firebase", "ML Kit"],
  "features": [
    "Workout and exercise logging",
    "Nutrition and calorie tracking",
    "Progress charts and analytics",
    "Social challenges and leaderboards",
    "Wearable device integration",
    "Exercise form recognition using ML"
  ],
  "technologies": [
    "Flutter",
    "Firebase",
    "ML Kit",
    "HealthKit",
    "Google Fit API"
  ],
  "demoUrl": "https://demo.example.com",
  "sourceUrl": "https://github.com/username/fitness-app"
}
```

### Required Fields
- ✅ **id**: Unique identifier (project1, project2, etc.)
- ✅ **title**: Project name
- ✅ **description**: Short description (1-2 sentences) for card
- ✅ **detailedDescription**: Full description for modal
- ✅ **tags**: Technologies shown on card (3-5 max)
- ✅ **features**: List of key features (5-8 items)
- ✅ **technologies**: All technologies used
- ✅ **demoUrl**: Link to live demo (use "#" if none)
- ✅ **sourceUrl**: Link to GitHub repo

### Project ID Guidelines
- Use sequential numbering: project1, project2, project3...
- Must be unique
- No spaces or special characters
- Used in HTML `data-project` attribute

---

## 🏆 Updating Achievements

**File**: `data/achievements.json`

### Add Achievement
```json
{
  "icon": "🎖️",
  "title": "Google Certified Mobile Developer",
  "description": "Certified in Android and Flutter development best practices"
}
```

### Icon Ideas
- 🏆 Trophy - Major awards
- 🎖️ Medal - Certifications
- ⭐ Star - Recognition
- 🚀 Rocket - Milestones
- 💡 Bulb - Innovation
- 🎯 Target - Goals achieved
- 📱 Phone - App launches
- 👥 People - Community

---

## 🖼️ Adding Images

### Hero Section

**File**: `index.html`

Find and update:
```html
<h1 class="hero-title">
    Hi, I'm <span class="gradient-text">Your Name</span>
</h1>
<p class="hero-subtitle">Your Job Title</p>
<p class="hero-description">Your brief introduction...</p>
```

### About Section

**File**: `index.html`

Find and update:
```html
<div class="about-content">
    <p>Your about text here...</p>
</div>
```

### Social Media Links

**File**: `index.html`

Update URLs in:
```html
<!-- Hero Section Social Links -->
<a href="https://github.com/YOUR_USERNAME">

<!-- Contact Section Social Links -->
<a href="https://linkedin.com/in/YOUR_PROFILE">
```

### Contact Information

**File**: `index.html`

Update:
```html
<div class="contact-info-item">
    <div class="contact-icon">✉️</div>
    <div>
        <h3>Email</h3>
        <p>your.email@example.com</p>
    </div>
</div>
```

---

## 📝 Updating Blog Posts

**File**: `data/blog.json`

### Add Blog Post
```json
{
  "id": "post7",
  "title": "Advanced Flutter Animations",
  "date": "December 1, 2024",
  "category": "Tutorial",
  "excerpt": "Master complex animations in Flutter with practical examples and best practices.",
  "image": "assets/images/blog/animations.jpg",
  "readTime": "9 min read",
  "url": "#"
}
```

### Field Descriptions
- **id**: Unique identifier (post1, post2, etc.)
- **title**: Blog post title (max 60 characters recommended)
- **date**: Publication date
- **category**: Post category (Tutorial, Development, UI/UX, Backend, Performance, Deployment, etc.)
- **excerpt**: Short description (2-3 sentences)
- **image**: Path to blog post image
- **readTime**: Estimated reading time
- **url**: Link to full blog post (use "#" for placeholder)

### Categories Suggestions
- **Tutorial** - Step-by-step guides
- **Development** - General development topics
- **UI/UX** - Design and user experience
- **Backend** - Server-side development
- **Performance** - Optimization tips
- **Deployment** - Publishing and hosting
- **Tips & Tricks** - Quick tips
- **Case Study** - Project analysis

### Example Full Entry
```json
{
  "id": "post1",
  "title": "Getting Started with Flutter: A Beginner's Guide",
  "date": "November 28, 2024",
  "category": "Tutorial",
  "excerpt": "Learn the fundamentals of Flutter development and build your first mobile application with this comprehensive guide.",
  "image": "assets/images/blog/flutter-basics.jpg",
  "readTime": "5 min read",
  "url": "https://medium.com/@your-username/getting-started-with-flutter"
}
```

### Tips
- Keep excerpts concise (2-3 lines max)
- Use descriptive titles
- Add actual blog URLs when you publish articles
- Update dates in "Month Day, Year" format
- Use consistent category naming

---

## 🖼️ Adding Images

### Project Screenshots

1. Add image to `assets/images/`
2. Update project card in `index.html`:

```html
<div class="project-image">
    <img src="assets/images/your-project.png" alt="Project Name">
</div>
```

Or in `data/projects.json`:
```json
{
  "id": "project1",
  "image": "assets/images/ecommerce-app.png",
  "title": "E-Commerce App"
}
```

Then update `renderProjects()` in `js/script.js` to use the image field.

### Profile Picture

Add to `index.html` hero section:
```html
<div class="hero-image">
    <img src="assets/images/profile.jpg" alt="Your Name">
</div>
```

### Blog Post Images

Add to blog section in `index.html`:
```html
<div class="blog-image">
    <img src="assets/images/blog-post-1.jpg" alt="Blog Post Title">
</div>
```

### Image Guidelines
- **Format**: Use WebP for best compression, fallback to JPG/PNG
- **Size**: Optimize images (max 500KB per image)
- **Dimensions**: 
  - Project screenshots: 800x600px
  - Profile: 400x400px
  - Blog images: 600x400px
- **Names**: Use descriptive names (my-project-screenshot.png)

---

## 🎨 Changing Colors

**File**: `css/styles.css`

### Light Mode
```css
:root {
    --primary-color: #667eea;      /* Main brand color */
    --secondary-color: #764ba2;    /* Accent color */
    --text-color: #333;            /* Main text */
    --bg-color: #ffffff;           /* Background */
}
```

### Dark Mode
```css
[data-theme="dark"] {
    --primary-color: #667eea;
    --text-color: #e0e0e0;
    --bg-color: #1a1a2e;
}
```

### Quick Color Schemes

**Blue & Purple** (Current):
```css
--primary-color: #667eea;
--secondary-color: #764ba2;
```

**Green & Teal**:
```css
--primary-color: #38b2ac;
--secondary-color: #2c7a7b;
```

**Orange & Red**:
```css
--primary-color: #ed8936;
--secondary-color: #e53e3e;
```

**Pink & Purple**:
```css
--primary-color: #ed64a6;
--secondary-color: #9f7aea;
```

---

## ✅ Checklist Before Going Live

- [ ] Updated all JSON files with real data
- [ ] Replaced placeholder text in HTML
- [ ] Added real project screenshots
- [ ] Updated social media links
- [ ] Added your CV to `assets/cv/`
- [ ] Tested all links
- [ ] Checked responsive design on mobile
- [ ] Tested dark mode
- [ ] Proofread all content
- [ ] Tested contact form
- [ ] Checked browser console for errors
- [ ] Optimized all images

---

## 🆘 Common Issues

### Content Not Updating?
1. Clear browser cache (Ctrl+F5)
2. Check JSON syntax (use [JSONLint](https://jsonlint.com/))
3. Check browser console for errors

### Images Not Showing?
1. Check file path is correct
2. Ensure image is in `assets/images/`
3. Check file name spelling

### JSON Syntax Error?
- Missing comma between items
- Extra comma after last item
- Missing quote marks
- Use JSON validator

---

## 💡 Tips

1. **Keep it Simple**: Don't overcomplicate descriptions
2. **Be Specific**: Use concrete examples and numbers
3. **Proofread**: Check spelling and grammar
4. **Update Regularly**: Keep content fresh
5. **Test Everything**: Check all links and features
6. **Backup**: Keep a copy of working JSON files

---

## 📧 Need Help?

If you're stuck:
1. Check the main [README.md](README.md) for detailed documentation
2. Review [CHANGELOG.md](CHANGELOG.md) for recent changes
3. Check browser console for error messages
4. Validate JSON files at [JSONLint.com](https://jsonlint.com/)

---

**Happy Updating! 🚀**
