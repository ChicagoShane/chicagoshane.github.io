# The Data Adventure - Vintage Portfolio

A unique Choose Your Own Adventure-style portfolio website with vintage book aesthetics. Perfect for data professionals who want to stand out from generic portfolios.

## 🎨 Features

- **Authentic CYOA Aesthetic**: Orange series banner, blue block title, illustrated scene frame - just like the original 1980s books
- **Vintage Book Design**: Aged paper textures, serif typography, and classic Choose Your Own Adventure styling
- **Interactive Navigation**: Recruiters explore your story by choosing different paths
- **Skip Link**: "Skip to Projects" button for recruiters who want to get straight to your work
- **Fully Responsive**: Works beautifully on desktop, tablet, and mobile
- **Easy Customization**: Simple HTML structure makes it easy to add your content
- **GitHub Pages Ready**: Deploy in minutes with zero configuration

## 📚 Structure

The portfolio has five main pages:

1. **index.html** - The book cover (landing page)
2. **story.html** - The main navigation page with story intro
3. **projects.html** - Showcase your data projects
4. **leadership.html** - Display your management assessments
5. **publications.html** - Archive your articles and publications

## 🚀 Quick Start

### Option 1: Deploy to GitHub Pages

1. Create a new repository named `[your-username].github.io`
2. Upload all files to the repository
3. Go to Settings > Pages
4. Select "Deploy from a branch" and choose "main" branch
5. Your site will be live at `https://[your-username].github.io`

### Option 2: Local Development

1. Download all files to a folder
2. Open `index.html` in your browser
3. That's it! No build process needed.

## ✏️ Customization Guide

### 1. Update Your Name and Info

**In `index.html`:**
```html
<!-- Line 48 -->
<div class="author-name">BY [YOUR NAME]</div>
```

**In `publications.html`:**
```html
<!-- Lines 162-167 - Update contact links -->
<a href="https://github.com/yourusername">GitHub</a>
<a href="https://linkedin.com/in/yourprofile">LinkedIn</a>
<a href="mailto:your.email@example.com">Email</a>
```

### 2. Add Your Data Projects

**In `projects.html`:**

Find the project card template (lines 35-67) and duplicate it:

```html
<div class="project-card">
    <div class="project-header">
        <h3 class="project-title">YOUR PROJECT NAME</h3>
        <div class="project-tags">
            <span class="tag">Python</span>
            <span class="tag">Tech Stack</span>
        </div>
    </div>
    <div class="project-description">
        <p>Brief description highlighting impact and results...</p>
    </div>
    <div class="project-details">
        <div class="detail-item">
            <span class="detail-label">Impact:</span>
            <span class="detail-value">$X saved</span>
        </div>
        <div class="detail-item">
            <span class="detail-label">Timeline:</span>
            <span class="detail-value">X weeks</span>
        </div>
    </div>
    <div class="project-links">
        <a href="https://github.com/yourusername/project" class="project-link">
            View on GitHub →
        </a>
    </div>
</div>
```

**Tips for great project cards:**
- Lead with business impact (revenue saved, efficiency gained)
- Keep descriptions to 2-3 sentences
- Include relevant metrics
- Link to live demos or GitHub repos

### 3. Add Your Leadership Assessments

**In `leadership.html`:**

Find the assessment card template (lines 30-47) and customize:

```html
<div class="assessment-card">
    <div class="assessment-header">
        <h4 class="assessment-name">Assessment Name</h4>
        <div class="assessment-date">Completed: Month Year</div>
    </div>
    <div class="assessment-result">
        <div class="result-badge">YOUR RESULT</div>
    </div>
    <div class="assessment-insights">
        <p><strong>Key Strengths:</strong> What this reveals...</p>
        <p><strong>Application:</strong> How you've used this...</p>
    </div>
</div>
```

**Popular assessments to include:**
- MBTI (Myers-Briggs)
- StrengthsFinder/CliftonStrengths
- DISC Assessment
- Emotional Intelligence (EQ)
- Leadership Practices Inventory
- Situational Leadership

### 4. Add Your Publications

**In `publications.html`:**

Find the publication template (lines 30-44) and duplicate:

```html
<div class="publication-entry">
    <div class="publication-header">
        <h4 class="publication-title">Article Title</h4>
        <div class="publication-meta">
            <span class="pub-type">Blog Post</span>
            <span class="pub-date">Month Year</span>
            <span class="pub-venue">Medium</span>
        </div>
    </div>
    <div class="publication-abstract">
        <p>Brief summary of the article and its impact...</p>
    </div>
    <div class="publication-footer">
        <a href="https://link-to-article.com" class="pub-link">Read Article →</a>
        <span class="citation-count">X citations</span>
    </div>
</div>
```

**Publication types:**
- Journal Article
- Conference Paper
- Blog Post
- White Paper
- Technical Documentation
- Case Study

### 5. Customize the Story Narrative

**In `story.html`:**

Edit the story text (lines 21-38) to tell YOUR unique journey. The current text is a template - make it personal:

```html
<p class="first-paragraph">
    <span class="dropcap">Y</span>our story here...
</p>
```

**Writing tips:**
- Use the second person ("You") to draw readers in
- Mention specific accomplishments or turning points
- Keep it concise but evocative
- Match the vintage adventure book tone

### 6. Customize the Cover Illustration

The cover features a vintage-style painted illustration showing a data professional at work. The image is `cyoadata.png` and displays:
- Person working at a vintage computer
- Data visualizations on screen (bar charts, pie chart, line graphs)
- Coffee mug on desk
- Bookshelf with warm lighting
- Starry night window
- Classic 1980s painted illustration aesthetic

**To use your own illustration:**

1. **Create or commission your artwork** (recommended size: 600x800px or similar portrait ratio)
2. **Save it** as `cover-image.png` or `cover-image.jpg`
3. **Update the image reference** in `index.html`:
```html
<img src="cover-image.png" alt="Your description" />
```

**Tips for creating cover art:**
- Use AI tools like DALL-E 3, Midjourney, or Stable Diffusion
- Request "1980s choose your own adventure book illustration style"
- Include data-specific elements: computers, charts, graphs, dashboards
- Warm lighting and painted/illustrated style work best
- The rounded border frame is built into this image, but you can add it via CSS if needed

**Alternative: Use the SVG version**
If you prefer a simple SVG illustration instead of a painted image, see the git history for the original SVG code, or create your own simple icon-based illustration.

## 🎨 Styling Customization

All visual styling is in `styles.css`. Here are common customizations:

### Change Color Scheme

Edit the CSS variables (lines 7-15):

```css
:root {
    --paper-cream: #f4e8d0;      /* Main background */
    --ink-dark: #2c1810;          /* Primary text */
    --accent-sepia: #8b4513;      /* Accent color */
    --accent-gold: #b8860b;       /* Secondary accent */
}
```

### Change Fonts

The portfolio uses three font families:
- **Titles**: IM Fell DW Pica (classic serif)
- **Body**: Crimson Text (readable serif)
- **Special**: Special Elite (typewriter)

To change fonts, update the Google Fonts import in each HTML file and the CSS variables.

### Adjust Page Size

Edit the `.book-page` width (line 299 in CSS):

```css
.book-page {
    width: 850px;  /* Adjust this */
    max-width: 95vw;
}
```

## 📱 Mobile Optimization

The portfolio is fully responsive with breakpoints at 768px. Mobile users see:
- Stacked navigation choices
- Simplified layouts
- Optimized font sizes
- Touch-friendly buttons

## ♿ Accessibility Features

- Semantic HTML structure
- High contrast ratios (WCAG AA compliant)
- Keyboard navigation support
- Screen reader friendly
- Reduced motion support for users with vestibular disorders

## 🔧 Advanced Customization

### Add More Pages

1. Create a new HTML file (e.g., `testimonials.html`)
2. Copy the structure from any existing page
3. Update page numbers and content
4. Add navigation links from other pages

### Add Project Images

Include screenshots in your project cards:

```html
<div class="project-card">
    <!-- Add after project-header -->
    <img src="images/project-screenshot.png" 
         alt="Project screenshot" 
         style="width: 100%; margin: 1rem 0; border: 2px solid var(--ink-brown);">
    <!-- Rest of card... -->
</div>
```

### Create a Blog Section

Duplicate the publications page structure and customize for blog posts:
- Change page number
- Update title to "The Chronicles" or similar
- Add blog post cards instead of publications

## 📊 SEO Tips

1. Update the `<title>` tags in each HTML file
2. Add meta descriptions:
```html
<meta name="description" content="Your portfolio description">
```
3. Include Open Graph tags for social sharing
4. Add an `alt` text to the cover SVG illustration

## 🐛 Troubleshooting

**Fonts not loading?**
- Check your internet connection (fonts load from Google Fonts)
- Verify the Google Fonts link in each HTML file

**Page numbers feel wrong?**
- Page numbers are decorative - adjust them to whatever feels right for your story

**Colors look different on my screen?**
- This is normal - the aged paper effect is designed to look vintage
- Adjust color values in CSS variables if needed

## 📝 License

This portfolio template is free to use for personal and commercial projects. No attribution required, but always appreciated!

## 💡 Tips for Success

1. **Keep it updated**: Add new projects and publications as you complete them
2. **Tell a story**: Each project should have a narrative arc (challenge → solution → impact)
3. **Use real metrics**: Concrete numbers are more impressive than vague descriptions
4. **Test on multiple devices**: Check how it looks on desktop, tablet, and mobile
5. **Get feedback**: Share with friends or mentors before going live
6. **Make it yours**: Don't be afraid to deviate from the template
7. **The skip link is your friend**: Not everyone enjoys novelty. The "Skip to Projects" link ensures busy recruiters can get straight to your work while still offering the full experience to those who want it

## 🎯 What Makes This Portfolio Stand Out

- **Unique concept** that's memorable and fun to explore
- **Professional yet creative** - shows personality without sacrificing credibility
- **Balances novelty with pragmatism** - skip link ensures it works for all recruiters
- **Interactive storytelling** - engages recruiters instead of boring them
- **Technical polish** - demonstrates attention to detail and frontend skills
- **Easy to navigate** - clear structure despite the creative approach

## 📮 Support & Feedback

Found a bug? Have a suggestion? Want to share your customized version?

Feel free to open an issue or reach out!

---

**Ready to begin your adventure?** Start customizing and good luck with your job search! 🚀
