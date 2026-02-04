# Priyam Gupta - Personal GitHub.io Website

A modern, professional academic website showcasing research in machine learning, dynamical systems, and control theory.

## Features

- ✨ Modern, distinctive design with smooth animations
- 📱 Fully responsive (mobile, tablet, desktop)
- 🎨 Custom typography using Cormorant Garamond and Work Sans
- 📄 Integrated CV download
- 🔗 Social media integration (LinkedIn, GitHub, Google Scholar)
- 🎯 Sections: About, Research, Publications, Experience, Contact
- 🎭 Scroll-reveal animations for engaging user experience

## Deployment to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and create a new repository
2. Name it: `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
   - For example: `priyamg14.github.io`
3. Make sure it's set to **Public**
4. Do NOT initialize with README (we'll push our own files)

### Step 2: Upload Your Files

#### Option A: Using GitHub Web Interface (Easiest)

1. Go to your newly created repository
2. Click "uploading an existing file"
3. Drag and drop both `index.html` and `CV.pdf` files
4. Add a commit message like "Initial commit: Add website files"
5. Click "Commit changes"

#### Option B: Using Git Command Line

```bash
# Navigate to where you saved the files
cd /path/to/your/website/files

# Initialize git repository
git init

# Add files
git add index.html CV.pdf

# Commit
git commit -m "Initial commit: Add website files"

# Add remote (replace 'yourusername' with your GitHub username)
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **Pages** in the left sidebar
4. Under "Source", select **main** branch
5. Click **Save**
6. Wait 1-2 minutes for deployment

### Step 4: Visit Your Website

Your website will be live at: `https://yourusername.github.io`

## Customization Guide

### Adding Your Photo

Replace the placeholder image in `index.html`:

```html
<!-- Find this line (around line 580) -->
<img src="https://via.placeholder.com/500x600/2d4263/ffffff?text=Your+Photo+Here" alt="Priyam Gupta">

<!-- Replace with your image -->
<img src="your-photo.jpg" alt="Priyam Gupta">
```

Then upload your photo file to the repository.

### Updating Content

Edit `index.html` to update:
- **Publications**: Add new papers in the Publications section
- **Experience**: Add new positions in the Experience section
- **Research Areas**: Modify the research cards
- **Contact Information**: Update email and links

### Updating CV

Simply replace `CV.pdf` with your updated CV file and commit the changes.

### Changing Colors

Update the CSS variables at the top of the `<style>` section:

```css
:root {
    --color-primary: #1a2332;      /* Main dark color */
    --color-secondary: #2d4263;    /* Secondary dark */
    --color-accent: #c84b31;       /* Accent color (red-orange) */
    --color-accent-light: #ecdbba; /* Light accent */
    /* ... */
}
```

### Changing Fonts

The website uses:
- **Cormorant Garamond** for headings (serif)
- **Work Sans** for body text (sans-serif)

To change fonts, update the Google Fonts link and CSS variables.

## Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers

## Performance

- No external JavaScript libraries required
- Optimized CSS animations
- Fast loading times
- SEO-friendly structure

## Maintenance

### Regular Updates

1. Update publications as they're published
2. Add new experiences/positions
3. Refresh CV annually
4. Test links periodically

### Analytics (Optional)

To add Google Analytics:

1. Get your GA tracking code
2. Add before `</head>` in index.html:

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

## Troubleshooting

### Website not loading?
- Wait 2-3 minutes after enabling GitHub Pages
- Check that repository name is `yourusername.github.io`
- Verify files are in the root directory (not in a subfolder)
- Ensure repository is Public

### 404 Error?
- Make sure the file is named `index.html` (lowercase)
- Check that GitHub Pages is enabled in Settings
- Clear your browser cache

### CV not downloading?
- Ensure `CV.pdf` is in the same directory as `index.html`
- Check file name matches exactly (case-sensitive)

## Support

For issues with:
- **GitHub Pages**: [GitHub Pages Documentation](https://docs.github.com/en/pages)
- **Git**: [Git Documentation](https://git-scm.com/doc)
- **Web Development**: [MDN Web Docs](https://developer.mozilla.org/)

## License

This website template is free to use and modify for personal academic websites.

---

**Built with** ❤️ **for researchers and academics**
