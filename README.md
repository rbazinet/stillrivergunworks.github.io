# Still River Gun Works Landing Page

## Setup Instructions

### Adding Your Logo
Save your Still River Gun Works logo image as `logo.png` in the `/assets/images/` directory.

### Form Setup
The contact form requires a form handler service. You have a few options:

1. **Formspree** (Recommended for simplicity):
   - Go to https://formspree.io
   - Sign up for a free account
   - Create a new form
   - Replace `YOUR_FORM_ID` in index.markdown with your Formspree form ID

2. **Netlify Forms** (If hosting on Netlify):
   - Add `data-netlify="true"` to the form tag
   - Remove the action attribute

3. **GitHub Pages** (If using GitHub Pages):
   - Consider using Formspree or another third-party service

### Running Locally
```bash
bundle exec jekyll serve
```
Then visit http://localhost:4000

### Deployment
- Push to GitHub and enable GitHub Pages in repository settings
- Or deploy to Netlify, Vercel, or any static hosting service