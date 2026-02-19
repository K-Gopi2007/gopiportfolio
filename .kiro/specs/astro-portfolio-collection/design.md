# Design Document: Astro Portfolio Collection

## Overview

This design outlines the implementation of a curated collection of 7 Astro portfolio templates organized in a single repository. Each template will be cloned into its own folder with custom documentation to help students quickly customize and deploy their portfolios to Vercel.

## Architecture

The repository will follow a flat structure with each template in its own folder:

```
astro-portfolio-collection/
├── README.md (main welcome guide)
├── .gitignore
├── astro-sphere/
│   ├── README.md (custom deployment guide)
│   └── [template files]
├── astrofy/
│   ├── README.md (custom deployment guide)
│   └── [template files]
├── minimal-bento-portfolio/
│   ├── README.md (custom deployment guide)
│   └── [template files]
├── litefolio/
│   ├── README.md (custom deployment guide)
│   └── [template files]
├── swissfolio/
│   ├── README.md (custom deployment guide)
│   └── [template files]
├── devolio/
│   ├── README.md (custom deployment guide)
│   └── [template files]
└── astro-terminal/
    ├── README.md (custom deployment guide)
    └── [template files]
```

## Components and Interfaces

### Template Selection Component

**Selected Templates (Top 7):**

1. **Astro Sphere** (TypeScript + Tailwind)
   - Modern, feature-rich portfolio with blog support
   - Professional design with dark mode

2. **Astrofy** (JavaScript + Tailwind)
   - Clean, minimalist design
   - Easy to customize for beginners

3. **Minimal Bento Portfolio** (JavaScript + Tailwind)
   - Trendy bento-box layout
   - Modern aesthetic

4. **LiteFolio** (TypeScript + Tailwind)
   - Lightweight and fast
   - Simple structure for easy learning

5. **Swissfolio** (TypeScript + Tailwind)
   - Swiss design principles
   - Clean typography

6. **Devolio** (JavaScript + Tailwind)
   - Developer-focused design
   - Project showcase emphasis

7. **Astro Terminal** (JavaScript + Tailwind)
   - Unique terminal-style interface
   - Fun, interactive design

**Selection Criteria:**
- Mix of TypeScript and JavaScript templates
- All use Tailwind CSS for consistency
- Range of design styles (minimal to feature-rich)
- Beginner-friendly codebases
- Active maintenance and good documentation

### Cloning Component

**Process:**
1. Use `degit` or `git clone` to fetch each template
2. Remove any nested `.git` folders to avoid conflicts
3. Rename folders to match template names (kebab-case)
4. Ensure each template has proper Astro configuration for Vercel

**Template URLs:**
- Astro Sphere: `https://github.com/markhorn-dev/astro-sphere`
- Astrofy: `https://github.com/manuelernestog/astrofy`
- Minimal Bento Portfolio: `https://github.com/Ladvace/astro-bento-portfolio`
- LiteFolio: `https://github.com/BryceRussell/astro-litefolio`
- Swissfolio: `https://github.com/BryceRussell/astro-swissfolio`
- Devolio: `https://github.com/TomDoesTech/devolio`
- Astro Terminal: `https://github.com/gndx/astro-terminal`

**Vercel Compatibility:**
Each template's `astro.config.mjs` (or `astro.config.ts`) must be configured for Vercel deployment to prevent CSS loading issues:

```javascript
import { defineConfig } from 'astro/config';
import vercel from '@astrojs/vercel/serverless';

export default defineConfig({
  output: 'server',
  adapter: vercel(),
  // ... other config
});
```

Or for static sites:
```javascript
import { defineConfig } from 'astro/config';

export default defineConfig({
  output: 'static',
  // ... other config
});
```

**Student Workflow:**
1. Clone the entire repository
2. Browse all 7 templates locally
3. Choose their favorite template
4. Delete all other template folders
5. Move chosen template files to root (or keep in folder)
6. Push to their GitHub
7. Deploy to Vercel

### Documentation Component

**Individual Template README Structure:**
```markdown
# [Template Name]

## Overview
Brief description of the template and its features.

## Tech Stack
- Astro
- Tailwind CSS
- TypeScript/JavaScript

## Quick Start

### Prerequisites
- Node.js 18+ installed
- Git installed

### Installation
1. Navigate to this folder
2. Install dependencies: `npm install`
3. Run dev server: `npm run dev`

## Customization Guide

### Key Files to Edit
1. **src/config.ts** or **src/data/config.json**
   - Your name, bio, social links
   
2. **src/pages/index.astro**
   - Homepage content
   
3. **src/content/** or **src/data/**
   - Projects, blog posts, experience

4. **public/**
   - Images, favicon, resume

### Step-by-Step Customization
[Specific instructions for this template]

## Deploy to Vercel

1. **Choose your favorite template and clean up**
   ```bash
   # Keep only your chosen template, delete the others
   # For example, if you chose astro-sphere:
   rm -rf astrofy minimal-bento-portfolio litefolio swissfolio devolio astro-terminal
   
   # Optional: Move template files to root
   mv astro-sphere/* .
   rm -rf astro-sphere
   ```

2. **Verify Astro config for Vercel**
   - Check that `astro.config.mjs` is properly configured (should already be set up)
   - Ensure `@astrojs/vercel` adapter is in dependencies if using SSR

3. **Push to your GitHub**
   ```bash
   git add .
   git commit -m "My portfolio"
   git push
   ```

4. **Deploy to Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import your GitHub repository
   - Vercel will auto-detect Astro settings
   - Click "Deploy"

Your site will be live in minutes!

## Resources
- [Astro Documentation](https://docs.astro.build)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Vercel Deployment Guide](https://vercel.com/docs)
- [Original Template](link)
```

**Main README Structure:**
```markdown
# Astro Portfolio Collection 🚀

Welcome to the Astro Portfolio Collection! This repository contains 7 carefully selected portfolio templates to help you create your professional portfolio website.

## 🎯 About This Collection

This collection was created for [Event Name] to help students quickly build and deploy beautiful portfolio websites using Astro.

## 📚 Available Templates

### TypeScript Templates
1. **Astro Sphere** - Feature-rich with blog support
2. **LiteFolio** - Lightweight and minimal
3. **Swissfolio** - Swiss design principles

### JavaScript Templates
4. **Astrofy** - Clean and beginner-friendly
5. **Minimal Bento Portfolio** - Modern bento layout
6. **Devolio** - Developer-focused
7. **Astro Terminal** - Unique terminal interface

## 🚀 Getting Started

### Prerequisites
- Node.js 18 or higher
- Git
- A code editor (VS Code recommended)
- A GitHub account
- A Vercel account (free)

### Choose Your Template
1. Browse the templates above
2. Navigate to the template folder
3. Follow the README inside for customization

### General Workflow
1. Clone this repository to your computer
2. Browse all 7 templates locally
3. Choose your favorite template
4. Delete the other 6 template folders
5. Customize your chosen template
6. Test locally: `npm install` then `npm run dev`
7. Push to your GitHub
8. Deploy to Vercel

## 🎨 Choosing Your Template

Each template folder contains:
- A complete, working Astro site
- A detailed README with customization instructions
- Pre-configured for Vercel deployment

Try running each template locally to see which one you like best!

```bash
cd astro-sphere
npm install
npm run dev
```

## 🚀 Quick Deploy

Once you've chosen your template:

1. **Keep only your chosen template**
   ```bash
   # Delete the templates you don't want
   # Keep only your favorite!
   ```

2. **Optional: Move to root**
   ```bash
   # Move your template files to the repository root
   mv your-chosen-template/* .
   ```

3. **Push and deploy**
   ```bash
   git add .
   git commit -m "My portfolio"
   git push
   ```

4. **Deploy on Vercel** - Import your repo and click deploy!

Detailed deployment instructions are in each template's README.

## 📖 Resources

- [Astro Documentation](https://docs.astro.build)
- [Tailwind CSS Docs](https://tailwindcss.com/docs)
- [Vercel Deployment Guide](https://vercel.com/docs)

## 🆘 Troubleshooting

**Issue: npm install fails**
- Make sure you have Node.js 18+ installed
- Try deleting `node_modules` and `package-lock.json`, then run `npm install` again

**Issue: Port already in use**
- The dev server runs on port 4321 by default
- Kill the process or use a different port: `npm run dev -- --port 3000`

**Issue: Build fails on Vercel**
- Check that all dependencies are in `package.json`
- Ensure Node.js version is set correctly in Vercel settings

## 🤝 Support

Need help? Reach out to the event organizers or check the Astro Discord community.

Happy coding! 🎉
```

## Data Models

### Template Metadata
```typescript
interface Template {
  name: string;
  folderName: string;
  repoUrl: string;
  techStack: {
    language: 'TypeScript' | 'JavaScript';
    styling: string;
    framework: string;
  };
  description: string;
  keyFiles: string[];
}
```

### Documentation Structure
```typescript
interface TemplateDoc {
  templateName: string;
  overview: string;
  techStack: string[];
  prerequisites: string[];
  installSteps: string[];
  customizationGuide: {
    keyFiles: Array<{
      path: string;
      purpose: string;
    }>;
    stepByStep: string[];
  };
  deploymentSteps: string[];
  resources: string[];
}
```

## Correctness Properties

*A property is a characteristic or behavior that should hold true across all valid executions of a system—essentially, a formal statement about what the system should do. Properties serve as the bridge between human-readable specifications and machine-verifiable correctness guarantees.*

### Property 1: Template Folder Organization
*For any* template folder in the repository root (excluding .git, .kiro, node_modules), the folder name should follow kebab-case convention and contain a valid Astro project structure with package.json and src directory.
**Validates: Requirements 1.2, 2.1, 2.4**

### Property 2: Template Diversity
*For any* collection of templates, there should exist at least one TypeScript-based template and at least one JavaScript-based template, verifiable through package.json dependencies.
**Validates: Requirements 1.4**

### Property 3: Template Integrity
*For any* template folder, the essential Astro project files (package.json, astro.config.mjs or astro.config.ts, src folder) should be present and valid.
**Validates: Requirements 2.2**

### Property 4: Template README Completeness
*For any* template folder, the README.md file should contain all required sections: overview, tech stack, installation steps, customization guide with key files, and Vercel deployment instructions.
**Validates: Requirements 3.1, 3.2, 3.3, 3.4, 3.5**

### Property 5: Main README Completeness
*For any* main README.md at repository root, it should reference all 7 templates by name, include prerequisites section, and provide links to individual template documentation.
**Validates: Requirements 4.3, 4.4, 4.5**

### Property 6: Gitignore Patterns
*For any* .gitignore file in the repository, it should contain essential Astro project patterns including node_modules, dist, and .env to prevent committing build artifacts and sensitive data.
**Validates: Requirements 5.2**

## Error Handling

### Cloning Failures
- If a template repository is unavailable or moved, log the error and skip that template
- Provide alternative template suggestions if a primary choice fails
- Validate repository URLs before attempting to clone

### File System Errors
- Handle permission errors when creating directories or files
- Verify disk space before cloning large repositories
- Provide clear error messages for file operation failures

### Git Operations
- Handle cases where Git is not installed or configured
- Provide guidance if GitHub authentication fails
- Validate repository initialization before attempting commits

### Documentation Generation
- Handle missing or malformed package.json files gracefully
- Provide default documentation structure if template analysis fails
- Validate README content before writing to ensure completeness

## Testing Strategy

This project will use a combination of unit tests and property-based tests to ensure correctness.

### Unit Testing
Unit tests will verify specific examples and edge cases:
- Verify exactly 7 template folders exist (excluding special folders)
- Verify main README.md exists at repository root
- Verify .git folder exists after initialization
- Verify .gitignore file exists and is not empty
- Verify each template folder contains a README.md
- Verify troubleshooting section exists in main README

### Property-Based Testing
Property tests will verify universal properties across all templates:
- **Property 1**: Test folder naming conventions across all template folders
- **Property 2**: Test tech stack diversity by analyzing all package.json files
- **Property 3**: Test Astro project structure integrity for all templates
- **Property 4**: Test README completeness for all template READMEs
- **Property 5**: Test main README references all templates
- **Property 6**: Test .gitignore contains required patterns

### Testing Configuration
- Use a property-based testing library appropriate for the implementation language
- Configure each property test to run minimum 100 iterations
- Tag each test with format: **Feature: astro-portfolio-collection, Property N: [property text]**
- Each property test should reference its corresponding design document property

### Integration Testing
- Test the complete workflow: clone → document → commit → push
- Verify templates can be installed and run locally
- Test that generated documentation is accurate and complete
- Verify Vercel deployment process works with generated templates

