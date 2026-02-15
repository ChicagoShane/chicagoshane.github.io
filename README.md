# The Data Adventurer - Interactive Portfolio Website

## Overview
This is a fully-functional "Choose Your Own Adventure" style portfolio website that tells your professional story through an interactive book metaphor. All pages are interconnected and navigation flows smoothly between sections.

## 📁 File Structure

```
/
├── landing_page.html      # Main entry point with desk scene
├── index.html            # Redirects to landing_page.html
├── story.html            # Chapter 1 - The Crossroads (main navigation hub)
├── projects.html         # Page 12 - Data Projects Laboratory
├── leadership.html       # Page 28 - Leadership Chamber
├── leadership-profile.html # Page 35 - Complete Leadership Profile
├── publications.html     # Page 45 - Publications Archive
├── styles.css            # All styling for the book-style pages
├── deskfull.png          # Landing page desk scene image
└── postit.png            # Post-it note image (optional)
```

## 🔗 Navigation Flow

### Entry Points
1. **index.html** → Redirects to **landing_page.html**
2. **landing_page.html** → Interactive desk scene with two clickable areas:
   - **Book** → Goes to **story.html**
   - **Pink Eraser ("SKIP THE STORY")** → Goes directly to **projects.html**

### Internal Navigation
From **story.html** (The Crossroads), users can navigate to:
- **projects.html** (Data Projects Laboratory)
- **leadership.html** (Leadership Chamber)
- **leadership-profile.html** (Complete Leadership Profile)
- **publications.html** (Publications Archive)

Each interior page has navigation links at the bottom to:
- Other main sections
- Return to **story.html** (The Crossroads)

## 🎨 Customization Guide

### 1. Landing Page (landing_page.html)
- **Update clickable area positions** if your desk image differs:
  ```css
  .book-button {
      left: 26%;    /* Adjust horizontal position */
      top: 8%;      /* Adjust vertical position */
      width: 38%;   /* Adjust width */
      height: 84%;  /* Adjust height */
  }
  ```

### 2. Projects Page (projects.html)
Replace placeholder project cards with your actual projects:
```html
<div class="project-card">
    <div class="project-header">
        <h3 class="project-title">Your Project Name</h3>
        <div class="project-tags">
            <span class="tag">Python</span>
            <span class="tag">SQL</span>
        </div>
    </div>
    <div class="project-description">
        <p>Brief description of your project and its impact...</p>
    </div>
    <div class="project-details">
        <div class="detail-item">
            <span class="detail-label">Impact:</span>
            <span class="detail-value">Your impact metric</span>
        </div>
    </div>
    <div class="project-links">
        <a href="YOUR_GITHUB_URL" class="project-link" target="_blank">
            <span>View on GitHub →</span>
        </a>
    </div>
</div>
```

### 3. Leadership Page (leadership.html)
Add your actual assessment results:
```html
<div class="assessment-card">
    <div class="assessment-header">
        <h4 class="assessment-name">Assessment Name</h4>
        <div class="assessment-date">Completed: Month Year</div>
    </div>
    <div class="assessment-result">
        <div class="result-badge">Your Result</div>
    </div>
    <div class="assessment-insights">
        <p><strong>Key Findings:</strong> Your insights...</p>
    </div>
</div>
```

### 4. Publications Page (publications.html)
Update with your actual publications:
```html
<div class="publication-entry">
    <div class="publication-header">
        <h4 class="publication-title">Your Publication Title</h4>
        <div class="publication-meta">
            <span class="pub-type">Article/Paper/Post</span>
            <span class="pub-date">Month Year</span>
            <span class="pub-venue">Where Published</span>
        </div>
    </div>
    <div class="publication-abstract">
        <p>Brief summary of your publication...</p>
    </div>
    <div class="publication-footer">
        <a href="URL" class="pub-link">Read Article →</a>
    </div>
</div>
```

### 5. Contact Information
Update the contact section in **publications.html**:
```html
<div class="contact-links">
    <a href="https://github.com/YOUR_USERNAME" target="_blank">GitHub</a>
    <a href="https://linkedin.com/in/YOUR_PROFILE" target="_blank">LinkedIn</a>
    <a href="mailto:YOUR_EMAIL@example.com">Email</a>
    <a href="https://yourwebsite.com" target="_blank">Website</a>
</div>
```

## 🎯 Features

### Landing Page
- ✨ Interactive clickable regions over desk photo
- 🎨 Hover effects and tooltips
- 💫 Subtle pulsing animations
- 📱 Fully responsive

### Story Pages
- 📖 Authentic vintage book aesthetic
- 📄 Textured paper background
- 🔤 Multiple typography styles (Merriweather, Crimson Text, Special Elite)
- 🎨 Sepia-toned color scheme
- ⚡ Smooth page transitions
- 📱 Mobile-responsive layout

## 🚀 Deployment Instructions

### Option 1: GitHub Pages
1. Create a new repository
2. Upload all files to the repository
3. Go to Settings → Pages
4. Select "Deploy from branch" and choose your main branch
5. Your site will be live at: `https://yourusername.github.io/repository-name/`

### Option 2: Netlify
1. Create account at netlify.com
2. Drag and drop the entire folder
3. Site deploys automatically
4. Custom domain available

### Option 3: Your Own Server
1. Upload all files to your web hosting
2. Ensure index.html is in the root directory
3. Files should maintain their relative paths

## 🔧 Technical Requirements

- **No server-side code** - pure HTML/CSS/JavaScript
- **No external dependencies** except Google Fonts
- **Works offline** once loaded
- **Cross-browser compatible**

## ✅ Testing Checklist

Before deploying, verify:
- [ ] Landing page clickable areas align with book and eraser
- [ ] Book click goes to story.html
- [ ] Eraser click goes to projects.html
- [ ] All navigation links work between pages
- [ ] All images load properly
- [ ] Mobile layout looks good
- [ ] All external links (GitHub, LinkedIn, etc.) are updated
- [ ] Contact information is correct
- [ ] Project descriptions are personalized
- [ ] Publication links work

## 🎨 Color Scheme (CSS Variables)

```css
--paper-cream: #f4e8d0;      /* Main background */
--paper-aged: #e8dcc4;       /* Aged paper effect */
--ink-dark: #2c1810;         /* Dark text */
--ink-brown: #4a3728;        /* Brown text */
--accent-sepia: #8b4513;     /* Accent color */
--accent-gold: #b8860b;      /* Gold highlights */
```

## 📝 Content Guidelines

### Projects Section
- Focus on **impact** and **outcomes**
- Include **metrics** where possible
- Use **action verbs** (built, designed, developed, deployed)
- Keep descriptions **concise** (2-3 sentences)

### Leadership Section
- Include **real assessment results**
- Show **application** of insights
- Demonstrate **growth mindset**

### Publications Section
- Link to **actual articles**
- Include **citation counts** if relevant
- Note **impact** or **reach**

## 🐛 Troubleshooting

**Issue:** Images not loading
- Check that image files are in the same directory as HTML files
- Verify file names match exactly (case-sensitive)

**Issue:** Fonts not loading
- Ensure internet connection (fonts load from Google)
- Check browser console for errors

**Issue:** Clickable areas on landing page misaligned
- Adjust CSS percentages in landing_page.html
- Test on different screen sizes

## 📱 Mobile Responsiveness

The site automatically adapts to:
- Desktop (>1024px)
- Tablet (768px - 1024px)
- Mobile (<768px)

## 🔄 Future Enhancements

Consider adding:
- [ ] Dark mode toggle
- [ ] Print-friendly version
- [ ] Downloadable PDF resume
- [ ] Blog integration
- [ ] Project filtering/search
- [ ] Analytics tracking
- [ ] Contact form

## 📄 License

This template is free to use and modify for your personal portfolio.

## 🤝 Support

For questions or issues, please update the GitHub/LinkedIn links in publications.html with your actual contact information.

---

**Ready to deploy?** Make sure you've personalized all placeholder content, updated all links, and tested navigation between all pages!
