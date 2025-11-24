# Orbital Systems Website

A modern, professional website for Orbital Systems - designed to discover and turn ideas into technologies through focused research and engineering.

## Features

- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile devices
- **Smooth Scrolling**: Navigation links smoothly scroll to sections
- **Modern Animations**: Subtle fade-in animations as you scroll
- **Two Pages**: Main landing page and dedicated contact/team page
- **GitHub Pages Ready**: Optimized for easy deployment

## File Structure

```
├── index.html          # Main homepage
├── contact.html        # Contact and team page
├── styles.css          # All styling
├── script.js           # JavaScript functionality
└── README.md          # This file
```

## Deployment to GitHub Pages

### Method 1: Using GitHub Web Interface

1. Create a new repository on GitHub (e.g., `orbital-systems-website`)
2. Upload all files (index.html, contact.html, styles.css, script.js)
3. Go to Settings → Pages
4. Under "Source", select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click Save
7. Your site will be live at: `https://yourusername.github.io/orbital-systems-website`

### Method 2: Using Git Command Line

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit - Orbital Systems website"

# Add your GitHub repository as remote
git remote add origin https://github.com/yourusername/orbital-systems-website.git

# Push to GitHub
git branch -M main
git push -u origin main

# Then enable GitHub Pages in repository settings
```

## Customization Guide

### Adding Your Logo

1. Save your logo image in the same folder as index.html
2. In both `index.html` and `contact.html`, replace:
   ```html
   <div class="logo">Orbital Systems</div>
   ```
   with:
   ```html
   <div class="logo">
       <img src="your-logo.png" alt="Orbital Systems" height="40">
   </div>
   ```

### Replacing Placeholder Images

The site currently uses simple SVG placeholders. To add real images:

1. Save your images in an `images/` folder
2. Replace SVG placeholders with:
   ```html
   <img src="images/your-image.jpg" alt="Description">
   ```

Recommended images:
- Hero illustration (500x500px)
- Team photos (4 images, square format)
- Capability icons (4 images)
- Additional decorative illustrations

### Updating Colors

All colors are defined in `styles.css` at the top:

```css
:root {
    --primary-yellow: #FDB927;    /* Main brand color */
    --dark-text: #1a1a1a;         /* Text color */
    --light-bg: #ffffff;          /* Background */
    --gray-text: #666666;         /* Secondary text */
    --pink-accent: #FFB3D9;       /* Accent color */
    --blue-accent: #A8D8E8;       /* Accent color */
}
```

### Updating Contact Information

In both HTML files, find the footer section and update:
- Address
- Email addresses
- Phone numbers
- Social media links

## Browser Compatibility

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Performance

- Lightweight: ~10KB total (HTML + CSS + JS)
- No external dependencies
- Fast loading times
- SEO-friendly structure

## Future Enhancements

Suggestions for expanding the site:
- Add a blog section
- Include project portfolio
- Add contact form with backend
- Integrate analytics
- Add more team member profiles
- Create case studies section

## License

This is a custom website design for Orbital Systems.

## Support

For questions or issues, contact: operations.orbitalsystems@gmail.com
