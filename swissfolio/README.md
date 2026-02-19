# Swissfolio

## Overview

Swissfolio is inspired by Swiss design principles - clean typography, grid-based layouts, and minimalist aesthetics. Perfect for designers and creatives who appreciate timeless, elegant design. Features a modern take on classic Swiss style.

## Tech Stack

- **Framework:** Astro 5.x
- **Styling:** Tailwind CSS 4
- **Language:** JavaScript
- **Features:** Sitemap, Compressed HTML

## Quick Start

### Prerequisites

- Node.js 18+ installed
- Git installed
- A code editor (VS Code recommended)

### Installation

1. Navigate to this folder:
   ```bash
   cd swissfolio
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

#### 1. **astro.config.mjs** - Site URL
Update your site URL:
```javascript
site: 'https://yourdomain.com',
```

#### 2. **src/pages/index.astro** - Homepage
Your main page:
- Update your name and title
- Modify the introduction
- Add your bio
- Update links and contact info

#### 3. **src/pages/** - Additional Pages
Customize other pages:
- About page
- Work/Projects page
- Contact page
- Any custom pages

#### 4. **src/components/** - Reusable Components
Modify components:
- Header/Navigation
- Footer
- Project cards
- Contact forms

#### 5. **public/** - Static Assets
Replace with your own:
- Profile photo
- Project images
- `favicon.svg` - Your site icon
- Any other static files

### Step-by-Step Customization

1. **Update Site Configuration**
   - Edit `astro.config.mjs`
   - Change the site URL to your domain

2. **Personalize Homepage**
   - Edit `src/pages/index.astro`
   - Update your name and title
   - Add your introduction and bio
   - Include your contact information

3. **Add Your Work**
   - Create or edit project pages
   - Add project images to `public/`
   - Include descriptions and case studies
   - Link to live projects

4. **Customize Navigation**
   - Edit header component
   - Add or remove menu items
   - Update links

5. **Update Images**
   - Add your profile photo
   - Include project screenshots
   - Replace favicon

6. **Adjust Typography (Optional)**
   - Modify Tailwind config for fonts
   - Adjust spacing and sizing
   - Customize the Swiss-inspired grid

## Deploy to Vercel

This template is pre-configured for Vercel deployment!

### Deployment Steps

1. **Keep only this template**
   ```bash
   # Go back to the root directory
   cd ..
   
   # Delete other templates
   rm -rf astro-sphere astrofy minimal-bento-portfolio litefolio devolio astro-terminal
   
   # Move files to root (optional)
   mv swissfolio/* .
   rm -rf swissfolio
   ```

2. **Push to your GitHub**
   ```bash
   git add .
   git commit -m "My Swissfolio portfolio"
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
- [Swiss Design Principles](https://www.smashingmagazine.com/2009/07/lessons-from-swiss-style-graphic-design/)
- [Original Template](https://github.com/michael-andreuzza/swissfolio)
- [Vercel Deployment Guide](https://vercel.com/docs)

## Troubleshooting

**Issue: npm install fails**
- Ensure you have Node.js 18+ installed
- Try deleting `node_modules` and `package-lock.json`, then run `npm install` again

**Issue: Port 4321 already in use**
- Kill the existing process or use a different port: `npm run dev -- --port 3000`

**Issue: Tailwind styles not applying**
- Make sure Tailwind 4 is properly configured
- Check that the Vite plugin is loaded

## Features

- ✅ Swiss design principles
- ✅ Clean typography
- ✅ Grid-based layout
- ✅ Minimalist aesthetic
- ✅ Tailwind CSS 4
- ✅ Compressed HTML
- ✅ Sitemap generation
- ✅ SEO optimized
- ✅ Fast performance
- ✅ Vercel-ready

Happy coding! 🚀
