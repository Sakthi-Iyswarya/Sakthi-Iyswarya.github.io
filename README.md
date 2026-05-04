# 🎨 Personal Portfolio Website

A modern, interactive, and colorful portfolio website to showcase your resume, projects, and skills.

## ✨ Features

- **Responsive Design** - Works perfectly on all devices (desktop, tablet, mobile)
- **Interactive Animations** - Smooth scrolling, hover effects, and scroll animations
- **Colorful Gradients** - Eye-catching color schemes and gradient backgrounds
- **Downloadable Resume** - PDF resume download functionality
- **Project Showcase** - Display your key projects with images and descriptions
- **Skills Visualization** - Animated skill bars and tech stack icons
- **Contact Form** - Interactive contact form for visitors to reach you
- **Smooth Navigation** - Fixed navbar with active section highlighting
- **Social Media Links** - Connect to your GitHub, LinkedIn, Twitter, etc.

## 🚀 Quick Start

### 1. Customize Your Information

Edit the `index.html` file and replace the placeholder content with your own:

- **Line 33**: Replace "Your Name" with your actual name
- **Line 34**: Update your title/role
- **Lines 37-40**: Update social media links
- **Lines 42-44**: Add your profile picture (see instructions below)
- **Lines 68-80**: Update your about section text
- **Lines 82-94**: Update your statistics (years of experience, projects, etc.)
- **Lines 130-280**: Update your skills and percentages
- **Lines 310-420**: Add your actual projects with descriptions
- **Lines 480-560**: Update your work experience and education
- **Lines 590-620**: Update your contact information

### 2. Add Your Images

Create an `images` folder and add the following images:

```
portfolio/
├── images/
│   ├── profile.jpg          (Your profile picture - 500x500px recommended)
│   ├── project1.jpg         (Project screenshot - 800x600px recommended)
│   ├── project2.jpg
│   ├── project3.jpg
│   ├── project4.jpg
│   ├── project5.jpg
│   └── project6.jpg
```

Then update the image paths in `index.html`:
- Line 44: `<img src="images/profile.jpg" alt="Profile Picture">`
- Lines 315, 330, 345, etc.: Update project image paths

### 3. Create Your Resume PDF

1. Create your resume using any tool (Word, Google Docs, Canva, etc.)
2. Export it as a PDF file named `resume.pdf`
3. Place it in the root directory of your portfolio

### 4. Customize Colors (Optional)

Edit `styles.css` to change the color scheme (lines 9-18):

```css
:root {
    --primary-color: #6366f1;      /* Main brand color */
    --secondary-color: #ec4899;    /* Secondary accent */
    --accent-color: #10b981;       /* Success/highlight color */
    /* ... more colors ... */
}
```

## 📁 File Structure

```
portfolio/
├── index.html           # Main HTML file
├── styles.css          # All styling and animations
├── script.js           # Interactive functionality
├── resume.pdf          # Your downloadable resume
├── README.md           # This file
└── images/             # Folder for all images
    ├── profile.jpg
    ├── project1.jpg
    ├── project2.jpg
    └── ...
```

## 🌐 Deploying to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right and select "New repository"
3. Name it: `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
4. Make it public
5. Don't initialize with README (we already have one)
6. Click "Create repository"

### Step 2: Upload Your Files

**Option A: Using GitHub Web Interface**

1. On your repository page, click "uploading an existing file"
2. Drag and drop all your files:
   - index.html
   - styles.css
   - script.js
   - resume.pdf
   - README.md
   - All images from the images folder
3. Click "Commit changes"

**Option B: Using Git Command Line**

```bash
# Navigate to your portfolio folder
cd /path/to/your/portfolio

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial portfolio commit"

# Add remote repository
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings"
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"
6. Wait a few minutes for deployment

### Step 4: Access Your Website

Your portfolio will be live at: `https://yourusername.github.io`

## 📋 Complete File Checklist for GitHub Upload

Make sure you have all these files before uploading:

- ✅ `index.html` - Main HTML file
- ✅ `styles.css` - Styling file
- ✅ `script.js` - JavaScript file
- ✅ `resume.pdf` - Your resume (create this)
- ✅ `README.md` - Documentation
- ✅ `images/profile.jpg` - Your profile picture (add this)
- ✅ `images/project1.jpg` - Project screenshots (add these)
- ✅ `images/project2.jpg`
- ✅ `images/project3.jpg`
- ✅ `images/project4.jpg`
- ✅ `images/project5.jpg`
- ✅ `images/project6.jpg`

## 🎨 Customization Tips

### Change Gradient Colors

Find gradient definitions in `styles.css` (lines 13-16) and modify:

```css
--gradient-1: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
--gradient-2: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
```

### Add More Projects

Copy a project card block in `index.html` (lines 310-330) and paste it with your new project details.

### Modify Skills

Update the skills section in `index.html` (lines 130-280) with your actual skills and proficiency levels.

### Change Fonts

Add Google Fonts to the `<head>` section of `index.html`:

```html
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
```

Then update `styles.css`:

```css
body {
    font-family: 'Poppins', sans-serif;
}
```

## 🔧 Troubleshooting

### Images Not Showing?
- Check that image paths are correct
- Ensure images are in the `images` folder
- Verify image file names match exactly (case-sensitive)

### Resume Not Downloading?
- Make sure `resume.pdf` is in the root directory
- Check the file name is exactly `resume.pdf`

### Website Not Loading on GitHub Pages?
- Wait 5-10 minutes after first deployment
- Check that your repository is named `yourusername.github.io`
- Ensure GitHub Pages is enabled in repository settings

### Animations Not Working?
- Clear your browser cache
- Make sure `script.js` is properly linked in `index.html`
- Check browser console for JavaScript errors (F12)

## 📱 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers

## 🎯 Performance Tips

- Optimize images (use tools like TinyPNG)
- Keep images under 500KB each
- Use WebP format for better compression
- Minimize custom fonts

## 📞 Need Help?

If you encounter any issues:
1. Check the browser console for errors (F12)
2. Verify all files are uploaded correctly
3. Ensure file names match exactly
4. Check that paths are correct

## 📄 License

Feel free to use this template for your personal portfolio. No attribution required!

## 🌟 Credits

Built with HTML, CSS, and JavaScript
Icons from Font Awesome
Inspired by modern web design trends

---

**Good luck with your portfolio! 🚀**

Remember to:
- ⭐ Star the repository if you found it helpful
- 🔄 Keep your portfolio updated with new projects
- 📧 Update your contact information
- 🎨 Make it your own with custom colors and content
