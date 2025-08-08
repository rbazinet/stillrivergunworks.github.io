# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
This is a Jekyll-based static website for Still River Gun Works, a gunsmithing and gun repair shop located in Woodstock, CT. The site uses the Minima theme and is configured for deployment.

## Development Commands

### Local Development
```bash
# Install dependencies
bundle install

# Run local development server with auto-regeneration
bundle exec jekyll serve

# Build the site
bundle exec jekyll build
```

### Testing and Validation
```bash
# Check for broken links and HTML validation
bundle exec jekyll doctor

# Build site in production mode
JEKYLL_ENV=production bundle exec jekyll build
```

## Architecture

### Jekyll Structure
- **_posts/**: Blog posts following YYYY-MM-DD-title.markdown naming convention
- **_config.yml**: Main Jekyll configuration including site metadata, theme settings, and build options
- **index.markdown**: Homepage using the 'home' layout
- **about.markdown**: About page with permalink /about/
- **404.html**: Custom 404 error page

### Key Configuration
- Theme: minima (~> 2.5)
- Plugins: jekyll-feed for RSS feed generation
- Base URL: "/"
- Production URL: https://stillrivergunworks.com

### Content Management
Blog posts require front matter with layout, title, date, and categories. The site uses Liquid templating for dynamic content generation.