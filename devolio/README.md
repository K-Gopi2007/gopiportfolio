# Devolio

## Overview

Devolio is a modern, minimalist portfolio template built specifically for developers. It features a clean, professional design that puts your code and projects front and center. Perfect for showcasing your technical skills and development work.

## Tech Stack

- **Framework:** Astro 5.x
- **Styling:** Tailwind CSS 4
- **Language:** TypeScript
- **Features:** Modern Vite setup

## Quick Start

### Prerequisites

- Node.js 18+ installed
- Git installed
- A code editor (VS Code recommended)

### Installation

1. Navigate to this folder:
   ```bash
   cd devolio
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
- Add your developer bio
- Update tech stack and skills
- Add social links (GitHub, LinkedIn, etc.)

#### 2. **src/pages/** - Additional Pages
Customize other pages:
- Projects page - showcase your work
- About page - your developer journey
- Blog page (if included)
- Contact page

#### 3. **src/components/** - Reusable Components
Modify components:
- Project cards
- Skill badges
- Navigation
- Footer

#### 4. **public/** - Static Assets
Replace with your own:
- Profile photo
- Project screenshots
- `favicon.svg` - Your site icon
- Resume/CV PDF
- Project demo images

### Step-by-Step Customization

1. **Update Personal Info**
   - Edit `src/pages/index.astro`
   - Change your name and title
   - Update your developer bio
   - Add your tagline or motto

2. **Add Your Tech Stack**
   - List programming languages you use
   - Add frameworks and tools
   - Include technologies you're learning
   - Use icons or badges for visual appeal

3. **Showcase Projects**
   - Create project entries
   - Add project images to `public/`
   - Include:
     - Project name and description
     - Technologies used
     - GitHub repository link
     - Live demo link
     - Key features and challenges

4. **Update Social Links**
   - Add your GitHub profile
   - Include LinkedIn
   - Add Twitter/X if applicable
   - Include personal blog or website

5. **Add Resume/CV**
   - Upload your resume PDF to `public/`
   - Add a download link
   - Or create a dedicated CV page

6. **Customize Styling**
   - Edit Tailwind config for colors
   - Adjust typography
   - Modify spacing and layout

## Deploy to Vercel

This template is pre-configured for Vercel deployment!

### Deployment Steps

1. **Keep only this template**
   ```bash
   # Go back to the root directory
   cd ..
   
   # Delete other templates
   rm -rf astro-sphere astrofy minimal-bento-portfolio litefolio swissfolio astro-terminal
   
   # Move files to root (optional)
   mv devolio/* .
   rm -rf devolio
   ```

2. **Push to your GitHub**
   ```bash
   git add .
   git commit -m "My Devolio portfolio"
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
- [TypeScript Documentation](https://www.typescriptlang.org/docs)
- [Original Template](https://github.com/RyanFitzgerald/devportfolio)
- [Vercel Deployment Guide](https://vercel.com/docs)

## Troubleshooting

**Issue: npm install fails**
- Ensure you have Node.js 18+ installed
- Try deleting `node_modules` and `package-lock.json`, then run `npm install` again

**Issue: Port 4321 already in use**
- Kill the existing process or use a different port: `npm run dev -- --port 3000`

**Issue: TypeScript errors**
- Make sure all dependencies are installed
- Check tsconfig.json configuration
- Run `npm run build` to see detailed errors

## Features

- ✅ Developer-focused design
- ✅ Clean, professional layout
- ✅ Project showcase
- ✅ Tech stack display
- ✅ TypeScript support
- ✅ Tailwind CSS 4
- ✅ Modern Vite setup
- ✅ SEO optimized
- ✅ Fast performance
- ✅ Vercel-ready

Happy coding! 🚀
