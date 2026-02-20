# The Good Thyme Co 🧀

Artisan charcuterie & cheese board website — clean, minimal, modern.

## Quick Start

Just open `index.html` in your browser. No build tools needed.

## Deploy to GitHub + Netlify

### 1. Create a GitHub Repository

```bash
# Navigate to this project folder
cd the-good-thyme-co

# Initialize git
git init
git add .
git commit -m "Initial commit - The Good Thyme Co website"

# Create repo on GitHub (using GitHub CLI, or do it at github.com/new)
gh repo create the-good-thyme-co --public --source=. --push

# OR if you created the repo on github.com manually:
git remote add origin https://github.com/YOUR_USERNAME/the-good-thyme-co.git
git branch -M main
git push -u origin main
```

### 2. Deploy on Netlify

1. Go to [netlify.com](https://app.netlify.com) and sign in with GitHub
2. Click **"Add new site"** → **"Import an existing project"**
3. Select **GitHub** and pick `the-good-thyme-co`
4. Settings (leave defaults):
   - **Build command:** _(leave blank)_
   - **Publish directory:** `.`
5. Click **"Deploy site"**

Your site will be live at `https://random-name.netlify.app` within seconds.

### 3. Custom Domain (Optional)

In Netlify → **Site settings** → **Domain management** → **Add custom domain**

## Customization

### Adding Your Photos

Replace the placeholder `<div>` elements in the gallery and about sections with `<img>` tags:

```html
<!-- Replace this -->
<div class="gallery-placeholder">🧀</div>

<!-- With this -->
<img src="images/board-1.jpg" alt="Cheese board" style="width:100%;height:100%;object-fit:cover;" />
```

Create an `images/` folder and add your photos there.

### Updating Content

- **Prices & menu items:** Edit the `.menu-card` sections in `index.html`
- **Contact info:** Update email and location in the contact section
- **Social links:** Update Instagram/Facebook URLs in the footer
- **Colors:** Modify CSS variables in `:root` at the top of the `<style>` block

### Contact Form

The form currently shows a "Sent!" confirmation but doesn't actually send data. To make it functional:

- **Netlify Forms** (easiest): Add `netlify` attribute to the `<form>` tag:
  ```html
  <form class="contact-form" id="contactForm" netlify name="contact">
  ```
- **Formspree**: Replace the form action with your Formspree endpoint

## Tech Stack

- Plain HTML, CSS, JS — no build tools
- Google Fonts (Cormorant Garamond + Outfit)
- Intersection Observer for scroll animations
- Fully responsive (mobile-first)

## License

© 2026 The Good Thyme Co. All rights reserved.
