# Orbital Systems Website - Team Guide 🚀

Welcome! This guide will help you understand and update the Orbital Systems website, even if you've never worked with GitHub before.

---

## 📚 Table of Contents
1. [What You Need to Know (Basics)](#what-you-need-to-know-basics)
2. [Getting Started](#getting-started)
3. [How to Update the Website](#how-to-update-the-website)
4. [Understanding the Website Structure](#understanding-the-website-structure)
5. [Common Tasks](#common-tasks)
6. [Troubleshooting](#troubleshooting)

---

## What You Need to Know (Basics)

### What is GitHub?
Think of GitHub as **Google Drive for code**. Instead of storing Word documents or PDFs, it stores website files (HTML, CSS, JavaScript).

### Key Terms (Simple Explanations)

**Repository (Repo)** 📦
- A folder containing all your website files
- Like a project folder on your computer, but online
- Example: `orbital-systems-website` is your repository

**Branch** 🌿
- A copy of your website where you can make changes safely
- Think of it like "Save As..." - you can experiment without breaking the live site
- `main` branch = the live website everyone sees
- Other branches = your workspace for testing changes

**Commit** 💾
- Saving your changes with a description
- Like clicking "Save" + writing a note about what you changed
- Example: "Updated team member photo" or "Fixed contact email"

**Push** ⬆️
- Uploading your saved changes to GitHub
- Like uploading a file to Google Drive

**Pull** ⬇️
- Downloading the latest version from GitHub
- Like downloading a file from Google Drive

**GitHub Pages** 🌐
- Free website hosting from GitHub
- Your website URL: `https://yourusername.github.io/repo-name`

---

## Getting Started

### Step 1: Create a GitHub Account
1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Follow the instructions
4. **Share your username with the website owner so they can add you as a collaborator**

### Step 2: Get Added to the Repository
The website owner needs to:
1. Go to the repository on GitHub
2. Click **Settings** → **Collaborators**
3. Click **Add people**
4. Enter your GitHub username

You'll receive an email invitation - accept it!

### Step 3: Install GitHub Desktop (Easiest Method)
**For beginners, we recommend GitHub Desktop - it's much easier than typing commands!**

1. Download from [desktop.github.com](https://desktop.github.com)
2. Install it on your computer
3. Sign in with your GitHub account

### Step 4: Clone (Download) the Repository
1. Open GitHub Desktop
2. Click **File** → **Clone repository**
3. Find `orbital-systems-website` in the list
4. Choose where to save it on your computer
5. Click **Clone**

Now you have a copy of the website on your computer! 🎉

---

## How to Update the Website

### Method 1: GitHub Desktop (Recommended for Beginners)

#### Making Changes
1. **Open your local folder** where you cloned the website
2. **Edit the files** using any text editor (Notepad, VS Code, etc.)
3. **Save your changes**

#### Uploading Changes
1. **Open GitHub Desktop**
2. You'll see your changes listed on the left
3. **Write a summary** in the box at bottom-left
   - Example: "Updated contact email address"
4. Click **Commit to main**
5. Click **Push origin** (top right)

**That's it!** Your changes are now live! 🎊

Wait 1-2 minutes, then refresh your website to see the changes.

---

### Method 2: Editing Directly on GitHub (Quick Edits)

For small changes like fixing typos:

1. Go to your repository on GitHub.com
2. Navigate to the file you want to edit
3. Click the **pencil icon** (✏️) at the top right
4. Make your changes
5. Scroll down and click **Commit changes**
6. Click **Commit changes** again in the popup

Changes go live in 1-2 minutes!

---

## Understanding the Website Structure

Your website has **2 pages**:

```
your-repo/
├── index.html          ← Home page (main page)
├── contact.html        ← Contact page
├──styles.css           ← Visual styling (colors, fonts, spacing)
├── script.js           ← Interactive features (scroll effects, animations)
└── images/             ← All Custom images used on the site(create such a folder if not already there)
    ├── logo-image.png
    ├── team-member1-photo.jpg
    └── ...
```

### Navigation Structure
The navbar has 4 options:
- **Home** - Scrolls to top of page
- **Capabilities** - Scrolls down to capabilities section (same page)
- **About** - Scrolls down to about section (same page)
- **Contact** - Takes you to `contact.html` (separate page)

---

## Common Tasks

### 1. Changing Text Content

**Finding what to change:**
- Open `index.html` or `contact.html` in a text editor
- Press `Ctrl+F` (Windows) or `Cmd+F` (Mac) to search
- Type the text you want to change
- Update it and save

**Example:**
```html
<!-- Before -->
<h1>Designed to discover.</h1>

<!-- After -->
<h1>Innovation Through Research.</h1>
```

### 2. Updating Team Member Information

Look for the "Our Team" section in `index.html`:

```html
<div class="team-member">
    <h3>O P Karwande</h3>
    <p>Electronics Department Lead</p>
</div>
```

Change the name and title as needed.

### 3. Changing Contact Information

Open `contact.html` and look for:

```html
<p>Email: info@mysite.com</p>
<p>Call: 123-456-7890</p>
```

Update these to your actual contact details.

### 4. Adding or Replacing Images

**Step 1:** Add your new image to the `images/` folder

**Step 2:** Update the HTML:
```html
<!-- Before -->
<img src="images/old-photo.jpg" alt="Description">

<!-- After -->
<img src="images/new-photo.jpg" alt="Description">
```

**Image tips:**
- Use `.jpg` for photos
- Use `.png` for graphics with transparency
- Keep file sizes under 500KB for fast loading
- Use descriptive names: `team-photo-2024.jpg` not `IMG_1234.jpg`

### 5. Changing Colors

Open `css/styles.css`:

```css
/* Yellow accent color */
:root {
    --primary-color: #F5C842;  /* Change this hex code */
}

/* Or change specific elements */
.footer {
    background-color: #F5C842;  /* Change footer color */
}
```

Use [Google's color picker](https://g.co/kgs/colors) to find color codes.

### 6. Updating Links

```html
<!-- Email link -->
<a href="mailto:operations.orbitalsystems@gmail.com">Email Us</a>

<!-- Phone link -->
<a href="tel:+91-411-046">Call Us</a>

<!-- External website -->
<a href="https://example.com" target="_blank">Visit Website</a>
```

---

## Working with Branches (Advanced)

If you want to test changes before making them live:

### Creating a Branch (GitHub Desktop)
1. Click **Current Branch** at the top
2. Click **New Branch**
3. Name it (e.g., "update-team-page")
4. Click **Create Branch**

### Making Changes
- Make your edits
- Commit as usual
- Push to GitHub

### Merging Your Changes (Making Them Live)
1. Go to your repository on GitHub.com
2. Click **Pull requests** tab
3. Click **New pull request**
4. Select your branch
5. Click **Create pull request**
6. Add a description
7. Click **Merge pull request**

**Your changes are now live!**

---

## Troubleshooting

### "My changes aren't showing up!"

**Solution 1:** Clear your browser cache
- Press `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)

**Solution 2:** Wait a few minutes
- GitHub Pages can take 1-5 minutes to update

**Solution 3:** Check if you pushed your changes
- Open GitHub Desktop
- Make sure it says "Fetch origin" not "Push origin"
- If it says "Push origin", click it!

### "I broke something!"

**Don't panic!** GitHub keeps history of all changes.

**To undo your last commit:**

*GitHub Desktop:*
1. Click **History** tab
2. Right-click your last commit
3. Click **Revert this commit**
4. Push the revert

*Or, ask the website owner to help restore from an earlier version.*

### "I can't push my changes"

**Possible reasons:**
1. You don't have permission → Ask the owner to add you as a collaborator
2. Someone else made changes → Click **Pull origin** first, then **Push origin**
3. Merge conflict → Ask for help (this is rare)

### "Where do I get help?"

1. **GitHub Desktop Help:** Click **Help** menu → **Show User Guides**
2. **GitHub Docs:** [docs.github.com](https://docs.github.com)
3. **YouTube:** Search "GitHub Desktop tutorial for beginners"
4. **Ask your team:** Create a group chat for questions

---

## Quick Reference Cheat Sheet

### Daily Workflow
```
1. Open GitHub Desktop
2. Click "Fetch origin" (get latest changes)
3. Open your local files
4. Make changes
5. Save files
6. Go to GitHub Desktop
7. Write commit message
8. Click "Commit to main"
9. Click "Push origin"
10. Done! ✓
```

### Keyboard Shortcuts (GitHub Desktop)
- `Ctrl+Shift+F` - Fetch latest changes
- `Ctrl+Enter` - Commit
- `Ctrl+P` - Push to GitHub

---

## Safety Tips ⚠️

✅ **DO:**
- Always fetch/pull before making changes
- Write clear commit messages
- Test your changes locally before pushing
- Ask if you're unsure about something
- Keep backups of important images before replacing them

❌ **DON'T:**
- Delete files unless you're sure they're not needed
- Make changes directly on the `main` branch for major updates
- Forget to save files before committing
- Be afraid to ask questions!

---

## Useful Resources

### Learning Resources
- [GitHub Skills](https://skills.github.com/) - Interactive tutorials
- [GitHub Desktop Documentation](https://docs.github.com/en/desktop)
- [W3Schools HTML Tutorial](https://www.w3schools.com/html/) - Learn HTML basics
- [MDN Web Docs](https://developer.mozilla.org/) - Complete web development guide

### Tools
- **Text Editors:**
  - [VS Code](https://code.visualstudio.com/) - Free, popular, lots of features
  - [Notepad++](https://notepad-plus-plus.org/) - Simple, lightweight
  - [Sublime Text](https://www.sublimetext.com/) - Fast and clean

- **Image Editing:**
  - [TinyPNG](https://tinypng.com/) - Compress images for faster loading
  - [Remove.bg](https://www.remove.bg/) - Remove image backgrounds
  - [Canva](https://www.canva.com/) - Design graphics and edit images

- **Color Pickers:**
  - [Coolors.co](https://coolors.co/) - Generate color palettes
  - [HTML Color Codes](https://htmlcolorcodes.com/) - Find hex codes

---

## Contact & Support

If you get stuck:
1. Check this README first
2. Google your error message
3. Ask in your team chat
4. Contact the website owner

---

## Remember! 

**You can't really break anything permanently.** 

GitHub keeps a complete history of all changes. If something goes wrong, you can always restore an earlier version. So don't be afraid to experiment and learn!

Happy updating! 🎉

---

*Last updated: November 2025*