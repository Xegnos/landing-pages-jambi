# Landing Pages Jambi

A collection of professionally designed landing page templates for various businesses in Jambi, Indonesia. All templates are fully responsive, single-file HTML with embedded CSS and JavaScript - no build tools required.

## Live Demo

Visit the live demo: [https://yourusername.github.io/landing-pages-jambi](https://yourusername.github.io/landing-pages-jambi)

## Templates Included

| Template | Industry | Color Palette |
|----------|----------|---------------|
| **Serenity Spa** | Wellness & Beauty | Forest green, gold, cream |
| **Notaris & PPAT** | Legal & Professional | Navy, brass, ivory |
| **GOGIYO Korean BBQ** | Food & Restaurant | Red, black, gold |
| **Eternia Wedding Studio** | Photography & Events | Blush, champagne, sage |
| **APEX Fitness** | Gym & Health | Black, electric cyan, lime |

## Features

- **Fully Responsive** - Works on all devices from mobile to desktop
- **Single File** - Each template is a self-contained HTML file
- **No Dependencies** - No build tools, frameworks, or external libraries required
- **Indonesian Language** - All content localized for Indonesian market
- **Modern Design** - Contemporary aesthetics with smooth animations
- **Easy to Customize** - CSS variables for easy color/font changes

## Quick Start

### Option 1: Direct Use
1. Download the HTML file you need
2. Open in any code editor
3. Customize the content, colors, and images
4. Upload to your hosting provider

### Option 2: GitHub Pages (Free Hosting)
1. Fork this repository
2. Go to Settings > Pages
3. Set source to "main" branch
4. Your site will be live at `https://yourusername.github.io/landing-pages-jambi`

## Customization Guide

### Changing Colors
Each template uses CSS custom properties (variables) at the top of the `<style>` section:

```css
:root {
    --primary: #00F0FF;
    --secondary: #CCFF00;
    --background: #0A0A0A;
    /* ... */
}
```

Simply change these values to match your brand colors.

### Changing Fonts
Fonts are loaded from Google Fonts. To change:
1. Visit [Google Fonts](https://fonts.google.com)
2. Select your fonts
3. Replace the `<link>` tag in the `<head>`
4. Update the `font-family` in CSS

### Adding Real Images
Replace the gradient placeholders with actual images:

```css
/* Before (placeholder) */
background: linear-gradient(135deg, #1A3329, #0D1F17);

/* After (real image) */
background: url('your-image.jpg') center/cover;
```

## File Structure

```
landing-pages-jambi/
├── index.html      # Portfolio/showcase page
├── spa.html        # Serenity Spa template
├── notaris.html    # Notaris & PPAT template
├── kbbq.html       # GOGIYO Korean BBQ template
├── wedding.html    # Eternia Wedding Studio template
├── gym.html        # APEX Fitness template
└── README.md       # This file
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

Free to use for personal and commercial projects. Attribution appreciated but not required.

## Credits

Designed and developed as templates for businesses in Jambi, Indonesia.

---

**Note:** These are template files with placeholder content. Replace all business information, contact details, and images with your actual content before publishing.
