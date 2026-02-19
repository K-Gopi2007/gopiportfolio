# Astro Sphere

## Overview

Astro Sphere is a feature-rich portfolio and blog template designed for designers and developers. It includes a modern design with dark mode support, blog functionality, project showcase, work experience section, and a built-in search feature.

## Tech Stack

- **Framework:** Astro 4.x
- **Styling:** Tailwind CSS
- **UI Framework:** Solid.js
- **Language:** TypeScript
- **Features:** MDX support, RSS feed, Sitemap

## Quick Start

### Prerequisites

- Node.js 18+ installed
- Git installed
- A code editor (VS Code recommended)

### Installation

1. Navigate to this folder:
   ```bash
   cd astro-sphere
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

#### 1. **src/consts.ts** - Your Personal Information
This is the main configuration file where you'll update:
- Your name and site title
- Site description
- Author information
- Navigation links
- Social media links (Email, GitHub, LinkedIn, Twitter)

```typescript
export const SITE: Site = {
  TITLE: "Your Name",
  DESCRIPTION: "Your portfolio description",
  AUTHOR: "Your Name",
}
```

#### 2. **src/content/work/** - Work Experience
Add your work experience as Markdown files:
- Create files like `company-name.md`
- Include company, role, dates, and description
- Add your achievements and responsibilities

#### 3. **src/content/blog/** - Blog Posts
Write blog posts in Markdown/MDX format:
- Create files in this directory
- Include frontmatter (title, date, description, tags)
- Write your content in Markdown

#### 4. **src/content/projects/** - Your Projects
Showcase your projects:
- Create Markdown files for each project
- Include project name, description, technologies used
- Add links to live demos and GitHub repos

#### 5. **public/** - Static Assets
Replace these files with your own:
- `favicon.svg` - Your site icon
- `og-image.png` - Social media preview image
- Add project screenshots and images here

#### 6. **src/pages/index.astro** - Homepage
Customize your homepage content:
- Update the hero section with your introduction
- Modify the about section
- Adjust the layout as needed

### Step-by-Step Customization

1. **Update Personal Info**
   - Open `src/consts.ts`
   - Change SITE.TITLE to your name
   - Update SITE.DESCRIPTION with your tagline
   - Add your social media links in SOCIALS array

2. **Add Your Work Experience**
   - Go to `src/content/work/`
   - Create new `.md` files for each job
   - Follow the existing format

3. **Create Blog Posts**
   - Navigate to `src/content/blog/`
   - Create new `.md` or `.mdx` files
   - Add frontmatter and content

4. **Showcase Projects**
   - Go to `src/content/projects/`
   - Add your projects as Markdown files
   - Include descriptions and links

5. **Update Images**
   - Replace `public/favicon.svg` with your logo
   - Add your profile photo
   - Update `public/og-image.png` for social sharing

6. **Customize Colors (Optional)**
   - Edit `tailwind.config.cjs` for theme colors
   - Modify `src/styles/global.css` for custom styles

## Deploy to Vercel

This template is pre-configured for Vercel deployment!

### Method 1: Deploy from this Repository

1. **Keep only this template**
   ```bash
   # Go back to the root directory
   cd ..
   
   # Delete other templates
   rm -rf astrofy minimal-bento-portfolio litefolio swissfolio devolio astro-terminal
   
   # Move Astro Sphere files to root (optional)
   mv astro-sphere/* .
   rm -rf astro-sphere
   ```

2. **Push to your GitHub**
   ```bash
   git add .
   git commit -m "My Astro Sphere portfolio"
   git push
   ```

3. **Deploy on Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository
   - Vercel will auto-detect Astro settings
   - Click "Deploy"

### Method 2: Deploy as Subdirectory

1. **Push the entire collection to GitHub**

2. **Deploy on Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your repository
   - Set "Root Directory" to `astro-sphere`
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
- [Solid.js Documentation](https://www.solidjs.com/docs/latest)
- [Original Template](https://github.com/markhorn-dev/astro-sphere)
- [Vercel Deployment Guide](https://vercel.com/docs)

## Troubleshooting

**Issue: npm install fails**
- Ensure you have Node.js 18+ installed
- Try deleting `node_modules` and `package-lock.json`, then run `npm install` again

**Issue: Port 4321 already in use**
- Kill the existing process or use a different port: `npm run dev -- --port 3000`

**Issue: Images not loading**
- Make sure images are in the `public/` folder
- Use correct paths (e.g., `/image.png` for files in public/)

## Features

- ✅ Modern, responsive design
- ✅ Dark mode support
- ✅ Blog with MDX support
- ✅ Project showcase
- ✅ Work experience section
- ✅ Built-in search functionality
- ✅ RSS feed
- ✅ Sitemap generation
- ✅ SEO optimized
- ✅ Fast performance
- ✅ Vercel-ready

Happy coding! 🚀
