# Astrofy

## Overview

Astrofy is a clean and beginner-friendly portfolio template perfect for showcasing your work. It includes sections for blog posts, CV/resume, projects, services, and even a store section. The minimalist design puts your content front and center.

## Tech Stack

- **Framework:** Astro 3.x
- **Styling:** Tailwind CSS
- **Language:** JavaScript
- **Features:** MDX support, RSS feed, Sitemap

## Quick Start

### Prerequisites

- Node.js 18+ installed
- Git installed
- A code editor (VS Code recommended)

### Installation

1. Navigate to this folder:
   ```bash
   cd astrofy
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

#### 1. **src/config.ts** - Site Configuration
Update your site's basic information:
```typescript
export const SITE_TITLE = 'Your Name | Portfolio';
export const SITE_DESCRIPTION = 'Your portfolio description';
```

#### 2. **src/pages/index.astro** - Homepage
This is your main landing page:
- Update your name and introduction
- Modify the hero section
- Add your bio and about information
- Update social media links

#### 3. **src/pages/cv.astro** - Resume/CV Page
Customize your CV/resume:
- Add your education history
- List your work experience
- Include skills and certifications
- Add achievements

#### 4. **src/pages/projects.astro** - Projects Page
Showcase your work:
- Add project cards
- Include project descriptions
- Link to live demos and GitHub repos

#### 5. **src/content/blog/** - Blog Posts
Write blog posts in Markdown:
- Create `.md` files for each post
- Include frontmatter (title, description, pubDate, heroImage)
- Write your content

#### 6. **src/content/store/** - Store Items (Optional)
If you want to sell products or services:
- Add items as Markdown files
- Include pricing and descriptions
- Or remove this section if not needed

#### 7. **public/** - Static Assets
Replace with your own:
- `profile.jpg` or `profile.png` - Your photo
- `favicon.svg` - Your site icon
- Add project images and screenshots

### Step-by-Step Customization

1. **Update Site Info**
   - Open `src/config.ts`
   - Change SITE_TITLE and SITE_DESCRIPTION

2. **Personalize Homepage**
   - Edit `src/pages/index.astro`
   - Update your name, title, and bio
   - Add your social media links (GitHub, LinkedIn, Twitter, etc.)

3. **Create Your CV**
   - Open `src/pages/cv.astro`
   - Add your education and work experience
   - List your skills and achievements

4. **Add Projects**
   - Edit `src/pages/projects.astro`
   - Add project cards with descriptions
   - Include links to demos and source code

5. **Write Blog Posts**
   - Go to `src/content/blog/`
   - Create new `.md` files
   - Follow the existing format with frontmatter

6. **Update Images**
   - Add your profile photo to `public/`
   - Update image references in pages
   - Replace favicon

7. **Customize Services (Optional)**
   - Edit `src/pages/services.astro`
   - Add services you offer
   - Or remove this page if not needed

## Deploy to Vercel

This template is pre-configured for Vercel deployment!

### Deployment Steps

1. **Keep only this template**
   ```bash
   # Go back to the root directory
   cd ..
   
   # Delete other templates
   rm -rf astro-sphere minimal-bento-portfolio litefolio swissfolio devolio astro-terminal
   
   # Move Astrofy files to root (optional)
   mv astrofy/* .
   rm -rf astrofy
   ```

2. **Push to your GitHub**
   ```bash
   git add .
   git commit -m "My Astrofy portfolio"
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
- [Original Template](https://github.com/manuelernestog/astrofy)
- [Vercel Deployment Guide](https://vercel.com/docs)

## Troubleshooting

**Issue: npm install fails**
- Ensure you have Node.js 18+ installed
- Try deleting `node_modules` and `package-lock.json`, then run `npm install` again

**Issue: Port 4321 already in use**
- Kill the existing process or use a different port: `npm run dev -- --port 3000`

**Issue: Images not loading**
- Make sure images are in the `public/` folder
- Use correct paths (e.g., `/profile.jpg` for files in public/)

## Features

- ✅ Clean, minimalist design
- ✅ Blog with Markdown support
- ✅ CV/Resume page
- ✅ Project showcase
- ✅ Services page
- ✅ Store section (optional)
- ✅ RSS feed
- ✅ Sitemap generation
- ✅ SEO optimized
- ✅ Fast performance
- ✅ Vercel-ready

Happy coding! 🚀
