# LiteFolio

## Overview

LiteFolio is a lightweight and minimal portfolio template perfect for developers and designers who want a clean, fast-loading site. Built with simplicity in mind, it focuses on showcasing your work without unnecessary complexity.

## Tech Stack

- **Framework:** Astro 4.x
- **Styling:** Tailwind CSS
- **Language:** JavaScript
- **Features:** MDX support, Icon system

## Quick Start

### Prerequisites

- Node.js 18+ installed
- Git installed
- A code editor (VS Code recommended)

### Installation

1. Navigate to this folder:
   ```bash
   cd litefolio
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Open your browser to `http://localhost:4321`

## Customization Guide

### Key Files to Edit

#### 1. **src/pages/index.astro** - Homepage
Your main landing page:
- Update your name and title
- Modify the hero section
- Add your bio and introduction
- Update social links

#### 2. **src/pages/** - Other Pages
Customize additional pages:
- About page
- Projects page
- Contact page
- Any other pages you need

#### 3. **src/content/** - Content Files
If the template uses content collections:
- Add your projects
- Write about yourself
- Include case studies

#### 4. **public/** - Static Assets
Replace with your own:
- Profile photo
- Project images
- `favicon.svg` - Your site icon
- Resume/CV PDF

### Step-by-Step Customization

1. **Update Homepage**
   - Edit `src/pages/index.astro`
   - Change your name and title
   - Update bio and introduction
   - Add your social media links

2. **Add Projects**
   - Create project pages or data files
   - Add project images to `public/`
   - Include descriptions and technologies used
   - Link to live demos and GitHub repos

3. **Customize About Page**
   - Edit the about page
   - Add your story and background
   - Include skills and expertise
   - Add your photo

4. **Update Contact Info**
   - Add your email
   - Include social media links
   - Add contact form if needed

5. **Replace Images**
   - Add your profile photo
   - Update project screenshots
   - Replace favicon

6. **Customize Styling (Optional)**
   - Edit `tailwind.config.cjs` for colors
   - Modify component styles as needed

## Deploy to Vercel

This template is pre-configured for Vercel deployment!

### Deployment Steps

1. **Keep only this template**
   ```bash
   # Go back to the root directory
   cd ..
   
   # Delete other templates
   rm -rf astro-sphere astrofy minimal-bento-portfolio swissfolio devolio astro-terminal
   
   # Move files to root (optional)
   mv litefolio/* .
   rm -rf litefolio
   ```

2. **Push to your GitHub**
   ```bash
   git add .
   git commit -m "My LiteFolio portfolio"
   git push
   ```

3. **Deploy on Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository
   - Vercel will auto-detect Astro settings
   - Click "Deploy"

Your site will be live in minutes!

## Build for Production

To create a production build locally:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

## Resources

- [Astro Documentation](https://docs.astro.build)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Original Template](https://github.com/veranikabarel/astro-portfolio)
- [Vercel Deployment Guide](https://vercel.com/docs)

## Troubleshooting

**Issue: npm install fails**
- Ensure you have Node.js 18+ installed
- Try deleting `node_modules` and `package-lock.json`, then run `npm install` again

**Issue: Port 4321 already in use**
- Kill the existing process or use a different port: `npm run dev -- --port 3000`

**Issue: Icons not showing**
- Make sure astro-icon is properly installed
- Check icon names in components

## Features

- ✅ Lightweight and fast
- ✅ Minimal, clean design
- ✅ Easy to customize
- ✅ Responsive layout
- ✅ Icon system
- ✅ MDX support
- ✅ SEO optimized
- ✅ Fast performance
- ✅ Vercel-ready

Happy coding! 🚀
