# Astro Terminal (Astro Paper)

## Overview

Astro Paper is a minimal, accessible, and SEO-friendly blog theme with a clean, paper-like aesthetic. Perfect for developers and writers who want a distraction-free reading experience. Features excellent typography, dark mode, and accessibility features.

## Tech Stack

- **Framework:** Astro 5.x
- **Styling:** Tailwind CSS 4
- **Language:** TypeScript
- **Features:** Blog, RSS feed, Sitemap, Search, Dark mode

## Quick Start

### Prerequisites

- Node.js 18+ installed
- Git installed
- A code editor (VS Code recommended)

### Installation

1. Navigate to this folder:
   ```bash
   cd astro-terminal
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
Update your site's information:
```typescript
export const SITE = {
  website: "https://your-site.com",
  author: "Your Name",
  profile: "https://your-profile-url.com",
  desc: "Your site description",
  title: "Your Site Title",
  // ... other settings
}
```

#### 2. **src/content/blog/** - Blog Posts
Write blog posts in Markdown:
- Create `.md` files for each post
- Include frontmatter (title, description, pubDatetime, tags)
- Write your content with Markdown
- Add code snippets with syntax highlighting

#### 3. **src/pages/about.md** - About Page
Tell your story:
- Update with your background
- Add your experience
- Include your interests
- Link to your social profiles

#### 4. **public/** - Static Assets
Replace with your own:
- `assets/` - Your images and media
- `favicon.svg` - Your site icon
- `robots.txt` - SEO configuration
- Social media preview images

### Step-by-Step Customization

1. **Update Site Configuration**
   - Edit `src/config.ts`
   - Change SITE.title to your name or site name
   - Update SITE.desc with your tagline
   - Add your social media links in SOCIALS array

2. **Customize About Page**
   - Edit `src/pages/about.md`
   - Write your bio and background
   - Add your skills and expertise
   - Include contact information

3. **Write Blog Posts**
   - Go to `src/content/blog/`
   - Create new `.md` files
   - Use frontmatter for metadata:
     ```markdown
     ---
     title: "Your Post Title"
     description: "Post description"
     pubDatetime: 2024-01-01T00:00:00Z
     tags: ["tag1", "tag2"]
     ---
     
     Your content here...
     ```

4. **Customize Theme Colors**
   - Edit `tailwind.config.cjs`
   - Modify color scheme
   - Adjust typography settings

5. **Update Social Links**
   - Edit `src/config.ts`
   - Add your GitHub, LinkedIn, Twitter, etc.
   - Configure which links to display

6. **Add Your Photo**
   - Add profile image to `public/assets/`
   - Update references in about page
   - Replace favicon

## Deploy to Vercel

This template is pre-configured for Vercel deployment!

### Deployment Steps

1. **Keep only this template**
   ```bash
   # Go back to the root directory
   cd ..
   
   # Delete other templates
   rm -rf astro-sphere astrofy minimal-bento-portfolio litefolio swissfolio devolio
   
   # Move files to root (optional)
   mv astro-terminal/* .
   rm -rf astro-terminal
   ```

2. **Push to your GitHub**
   ```bash
   git add .
   git commit -m "My Astro Paper blog"
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
- [Markdown Guide](https://www.markdownguide.org)
- [Original Template](https://github.com/satnaing/astro-paper)
- [Vercel Deployment Guide](https://vercel.com/docs)

## Troubleshooting

**Issue: npm install fails**
- Ensure you have Node.js 18+ installed
- Try deleting `node_modules` and `package-lock.json`, then run `npm install` again

**Issue: Port 4321 already in use**
- Kill the existing process or use a different port: `npm run dev -- --port 3000`

**Issue: Blog posts not showing**
- Check frontmatter format in your `.md` files
- Ensure pubDatetime is in correct ISO format
- Verify files are in `src/content/blog/` directory

**Issue: Syntax highlighting not working**
- Make sure code blocks use proper markdown syntax
- Check Shiki configuration in astro.config.ts

## Features

- ✅ Minimal, paper-like design
- ✅ Excellent typography
- ✅ Dark mode support
- ✅ Accessible (WCAG compliant)
- ✅ SEO optimized
- ✅ Blog with Markdown
- ✅ Syntax highlighting
- ✅ Search functionality
- ✅ RSS feed
- ✅ Sitemap generation
- ✅ Fast performance
- ✅ Vercel-ready

Happy coding! 🚀
