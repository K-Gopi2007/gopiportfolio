# Minimal Bento Portfolio

## Overview

Minimal Bento Portfolio features a trendy bento-box layout with a modern, grid-based design. Perfect for creatives who want a unique, eye-catching portfolio that stands out. Includes smooth animations and interactive elements powered by GSAP and Solid.js.

## Tech Stack

- **Framework:** Astro 5.x
- **Styling:** UnoCSS
- **UI Frameworks:** Solid.js + Svelte
- **Language:** TypeScript
- **Animations:** GSAP, Motion
- **Features:** Blog, RSS feed, Sitemap

## Quick Start

### Prerequisites

- Node.js 18+ installed
- Git installed
- A code editor (VS Code recommended)

### Installation

1. Navigate to this folder:
   ```bash
   cd minimal-bento-portfolio
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

#### 1. **src/data/** - Your Information
Look for data files or configuration in the src directory:
- Personal information (name, bio, title)
- Social media links
- Project data
- Skills and experience

#### 2. **src/pages/index.astro** - Homepage
The main bento-grid layout:
- Update bento boxes with your content
- Modify grid layout
- Add your introduction and bio

#### 3. **src/content/blog/** - Blog Posts
Write blog posts in Markdown:
- Create `.md` files for each post
- Include frontmatter
- Add your content

#### 4. **public/** - Static Assets
Replace with your own:
- Profile images
- Project screenshots
- `favicon.svg` - Your site icon
- Social media preview images

### Step-by-Step Customization

1. **Update Personal Info**
   - Find configuration files in `src/data/` or similar
   - Update your name, title, and bio
   - Add your social media links

2. **Customize Bento Grid**
   - Edit `src/pages/index.astro`
   - Modify bento box content
   - Adjust grid layout to your preference

3. **Add Projects**
   - Update project data files
   - Add project images to `public/`
   - Include descriptions and links

4. **Write Blog Posts**
   - Go to `src/content/blog/`
   - Create new `.md` files
   - Follow the existing format

5. **Update Images**
   - Add your photos to `public/`
   - Replace favicon
   - Update image references

## Deploy to Vercel

This template is configured for Vercel deployment with SSR support!

### Deployment Steps

1. **Keep only this template**
   ```bash
   # Go back to the root directory
   cd ..
   
   # Delete other templates
   rm -rf astro-sphere astrofy litefolio swissfolio devolio astro-terminal
   
   # Move files to root (optional)
   mv minimal-bento-portfolio/* .
   rm -rf minimal-bento-portfolio
   ```

2. **Push to your GitHub**
   ```bash
   git add .
   git commit -m "My Bento Portfolio"
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
- [UnoCSS Documentation](https://unocss.dev)
- [GSAP Documentation](https://gsap.com/docs)
- [Original Template](https://github.com/Ladvace/astro-bento-portfolio)
- [Vercel Deployment Guide](https://vercel.com/docs)

## Troubleshooting

**Issue: npm install fails**
- Ensure you have Node.js 18+ installed
- Try deleting `node_modules` and `package-lock.json`, then run `npm install` again

**Issue: Animations not working**
- Make sure GSAP is properly installed
- Check browser console for errors

**Issue: Build fails**
- This template uses SSR - ensure Vercel adapter is installed
- Check that all dependencies are in package.json

## Features

- ✅ Modern bento-box layout
- ✅ Smooth animations (GSAP)
- ✅ Interactive elements
- ✅ Blog support
- ✅ SSR with Vercel adapter
- ✅ RSS feed
- ✅ Sitemap generation
- ✅ SEO optimized
- ✅ Responsive design
- ✅ Vercel-ready

Happy coding! 🚀
