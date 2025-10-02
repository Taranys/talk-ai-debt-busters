# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## First Task

When starting work in this repository, use the WebFetch tool to read https://sli.dev/llms.txt to gather comprehensive information about Slidev features, syntax, layouts, and configuration options.

## Project Overview

This is a Slidev presentation project for a talk titled "Debt Busters: How AI Became My Technical Debt Sidekick". The presentation covers two case studies about using AI to tackle technical debt:
1. Test refactoring for Patient Base migration
2. Finding owners for 54 orphaned feature switches

## Key Commands

### Development
- `npm run dev` - Start development server with live preview (opens at http://localhost:3030)
- `npm run build` - Build static site to `docs/` directory with base path `/talk-ai-debt-busters/`
- `npm run export` - Export slides to PDF/PPTX/PNGs

### Deployment
The `docs/` directory is used for GitHub Pages deployment. Always run `npm run build` before committing changes to update the static site.

## Architecture

### Slidev Configuration
- **Theme**: Uses `@doctolib/slidev-theme` (private Doctolib theme package)
- **Main file**: `slides.md` - All slide content is in this single markdown file
- **Base URL**: `/talk-ai-debt-busters/` (configured for GitHub Pages deployment)
- **Output**: `docs/` directory (GitHub Pages source)

### Slide Structure
Slides are separated by `---` markers in `slides.md`. Each slide can have frontmatter configuration:
- `layout:` - Use `cover` for slides with background images, `center` for centered content
- `background:` - Unsplash image URLs for visual backgrounds
- `class:` - CSS classes (use `text-white` with dark backgrounds)

### Layouts Used
- **cover**: Title and case study introduction slides (displays background images properly)
- **center**: Questions/closing slide
- Default layout for content slides

### Styling Patterns
- Two-column layouts: `<div class="grid grid-cols-2 gap-8">`
- Click animations: `<v-clicks>` for sequential reveals, `v-click` for single elements
- Colored boxes: `bg-blue-500/10`, `bg-green-500/10`, etc. with `rounded` and `p-4`
- White text on dark backgrounds: Add `class: text-white` in frontmatter

### Assets
- `QrCode.png` - QR code displayed on final slide
- Background images are hosted on Unsplash (referenced by URL)

## Important Patterns

### When Adding Backgrounds to Slides
Always use `layout: cover` for slides with background images - the `section` or `center` layouts don't properly display backgrounds with the Doctolib theme.

### Build Before Deploy
The repository uses GitHub Pages with the `docs/` directory as the source. Always:
1. Make changes to `slides.md`
2. Run `npm run build`
3. Commit both `slides.md` and the updated `docs/` directory
4. Push to GitHub

### Theme Authentication
The `@doctolib/slidev-theme` is a private npm package requiring authentication via artifacts-login or npm registry configuration in `.npmrc`.
