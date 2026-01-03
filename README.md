# Portfolio Website - Setup Instructions

## Folder Structure

Your portfolio website consists of:

```
portfolio.html          (your main website file)
images/
  └── artworks/
      ├── artwork1.jpg
      ├── artwork2.jpg
      └── artwork3.jpg
  └── designs/
      (add your design images here)
  └── sketches/
      (add your sketch images here)
```

## How to Use

### Option 1: View Locally
1. Keep the `portfolio.html` file and `images` folder in the same directory
2. Open `portfolio.html` in your web browser
3. Your artworks should display correctly

### Option 2: Host on a Website
You can host this on various platforms:

**Free Hosting Options:**
- **GitHub Pages** (recommended for portfolios)
- **Netlify** 
- **Vercel**
- **Google Drive** (with sharing settings)

**Steps for GitHub Pages:**
1. Create a GitHub account (free)
2. Create a new repository
3. Upload `portfolio.html` and the entire `images` folder
4. In repository settings, enable GitHub Pages
5. Your site will be live at: `https://yourusername.github.io/repository-name`

**Steps for Netlify (easiest):**
1. Create a Netlify account (free)
2. Drag and drop your folder containing `portfolio.html` and `images` folder
3. Your site will be live instantly with a custom URL

### Option 3: Send as a Package
If you want to send this to someone:
1. Put `portfolio.html` and the `images` folder in a single folder
2. Zip/compress that folder
3. Send it to them - they can unzip and open `portfolio.html`

## Adding More Images

### For Artworks:
1. Add your image files to the `images/artworks/` folder
2. Open `portfolio.html` in a text editor
3. Find the `galleries` object in the JavaScript section
4. Add your image paths like this:

```javascript
artworks: [
    'images/artworks/artwork1.jpg',
    'images/artworks/artwork2.jpg',
    'images/artworks/artwork3.jpg',
    'images/artworks/artwork4.jpg',  // Add your new images here
    'images/artworks/artwork5.jpg',
]
```

### For Designs and Sketches:
Same process - add images to the respective folders and update the JavaScript arrays.

## Customization

To personalize your portfolio:
1. Replace "YOUR NAME" with your actual name (appears in 3 places)
2. Update email: `your.email@example.com`
3. Update phone: `+1 (234) 567-890`
4. Update footer year if needed: `© 2026`

## Image Format Notes

- **Supported formats:** JPG, PNG, GIF, WebP
- **Not supported in this setup:** HEIC files (convert to JPG first)
- **Recommended:** Keep images under 2MB each for fast loading

## Troubleshooting

**Images not showing?**
- Make sure the `images` folder is in the same location as `portfolio.html`
- Check that image filenames in the code match the actual filenames exactly (case-sensitive)
- Make sure image paths use forward slashes: `images/artworks/photo.jpg`

**Need help?**
- All major browsers should work (Chrome, Firefox, Safari, Edge)
- Works on mobile devices too
- No server or coding knowledge required!
