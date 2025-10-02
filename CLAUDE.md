# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a documentation website for "Let's Map" (previously HarcMap), a mobile application for organizing dynamic city and outdoor games, such as scavenger hunts, rallies, or field activities. The documentation is built using Docsify, a dynamic documentation site generator that serves markdown files directly without the need for static site generation.

## Development Commands

The project uses npm for package management. Navigate to the `docs/` directory to run commands:

```bash
cd docs/
npm install              # Install dependencies
npm run serve           # Start development server (serves documentation locally)
```

The development server will typically run on http://localhost:3000 and provides live reload for content changes.

## Architecture

- **Docsify Framework**: The site uses Docsify v4 for dynamic documentation rendering
- **Main Entry Point**: `docs/index.html` configures the Docsify application
- **Navigation**: `docs/_sidebar.md` defines the site navigation structure
- **Content Structure**:
  - `docs/quick-start.md` - Main getting started guide
  - `docs/features/` - Feature documentation directory
  - `docs/tutorials/` - Tutorial content directory
  - `docs/assets/` - Images and other static assets

## Content Organization

- Documentation is written in Polish and focuses on the Let's Map mobile application
- Features are documented in separate markdown files under `docs/features/`
- The sidebar navigation is manually maintained in `_sidebar.md`
- Static assets (logos, screenshots) are stored in `docs/assets/`

## Docsify Configuration

Key configuration in `docs/index.html`:
- Repository link points to GitHub repo
- Search functionality enabled
- Tab plugin for content organization
- Custom CSS styling in `docs/index.css`

## GitHub Integration

- Issue templates are configured in `.github/ISSUE_TEMPLATE/` for content contributions
- The site is hosted at https://guide.letsmap.pl/
- CNAME file configures the custom domain

## Working with Content

When adding new documentation:
1. Create markdown files in appropriate directories (`features/`, `tutorials/`)
2. Update `_sidebar.md` to include new pages in navigation
3. Use Polish language for content consistency
4. Include relevant screenshots in `assets/` directory when needed
