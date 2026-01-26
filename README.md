# Spokane Valley AI Website

A modern, single-page website for Spokane Valley AI - an AI consulting business serving local small and medium businesses.

## 🚀 Quick Start

### Deploying to GitHub Pages

1. Push this repository to GitHub
2. Go to your repository's **Settings** → **Pages**
3. Under "Source", select **Deploy from a branch**
4. Select **main** branch and **/ (root)** folder
5. Click **Save**
6. Your site will be live at `https://yourusername.github.io/repositoryname`

### Custom Domain (Optional)

To use a custom domain like `spokanevalleyai.com`:

1. In GitHub Pages settings, enter your custom domain
2. Add these DNS records at your domain registrar:
   - **A records** pointing to GitHub's IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - **CNAME record**: `www` → `yourusername.github.io`

## 📁 File Structure

```
spokaneai/
├── index.html      # Main website page
├── styles.css      # All styling
├── .nojekyll       # Tells GitHub Pages to skip Jekyll processing
├── CNAME           # Custom domain (create if needed)
└── README.md       # This file
```

## ✏️ Customization

### Contact Form

The contact form uses [Formspree](https://formspree.io/) for handling submissions. To set it up:

1. Create a free account at formspree.io
2. Create a new form and copy your form ID
3. In `index.html`, replace `YOUR_FORM_ID` in the form action:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

### Update Contact Information

Edit these sections in `index.html`:
- Email address: Search for `hello@spokanevalleyai.com`
- Phone number: Search for `(509) 123-4567`
- Location: Search for `Spokane Valley, WA`

### Pricing

Pricing tiers are in the `#pricing` section. Each tier is a `.pricing-card` div that you can modify.

### Colors

All colors are defined as CSS variables at the top of `styles.css`. Key variables:
- `--color-accent`: Main brand color (teal/cyan)
- `--color-bg-dark`: Background color
- `--gradient-primary`: Button/accent gradients

## 📱 Features

- ✅ Fully responsive (mobile, tablet, desktop)
- ✅ Smooth scroll navigation
- ✅ Animated sections on scroll
- ✅ Mobile hamburger menu
- ✅ SEO-optimized meta tags
- ✅ Contact form ready for integration
- ✅ Modern dark theme design

## 🛠️ Local Development

To preview locally, simply open `index.html` in your browser, or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js (npx)
npx serve
```

Then visit `http://localhost:8000`

## 📄 License

© 2026 Spokane Valley AI. All rights reserved.
