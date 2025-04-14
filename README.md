# Plumbing Local SEO Directory Website

![Plumbing Local SEO](assets/images/hero-banner.jpg)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Support & Resources](#support--resources)

## Overview
Plumbing Local SEO is a modern directory website showcasing plumbing services and experts. Built with a responsive 3-column grid layout, the site offers seamless navigation and optimal viewing across all devices.

## Features
- Responsive 3-column grid layout
- Search functionality
- Category filtering
- Interactive directory cards
- SEO-optimized structure
- Mobile-friendly design
- Fast loading performance
- Contact form integration

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Basic knowledge of HTML/CSS

### Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/plumbing-local-seo.git

# Navigate to project directory
cd plumbing-local-seo

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure
```
plumbing-local-seo/
├── assets/
│   ├── images/
│   ├── css/
│   └── js/
├── components/
│   ├── Header/
│   ├── Footer/
│   └── DirectoryGrid/
├── data/
│   └── directory-items.json
├── pages/
└── config/
```

## Customization Guide

### Adding Directory Items
1. Navigate to `data/directory-items.json`
2. Add new items following this format:
```json
{
  "id": "unique-id",
  "title": "Business Name",
  "category": "Category",
  "description": "Business description",
  "contact": {
    "phone": "555-0123",
    "email": "contact@example.com"
  },
  "image": "path/to/image.jpg"
}
```

### Modifying Category Labels
1. Open `config/categories.js`
2. Update the category array:
```javascript
export const categories = [
  "Residential",
  "Commercial",
  "Emergency",
  "Maintenance"
];
```

### Updating Hero Section
1. Locate `components/Hero/index.js`
2. Modify the content:
```javascript
<div className="hero">
  <h1>Your New Heading</h1>
  <p>Your new subheading text</p>
</div>
```

### Customizing Colors
1. Navigate to `assets/css/variables.css`
2. Update color variables:
```css
:root {
  --primary-color: #007bff;
  --secondary-color: #6c757d;
  --accent-color: #28a745;
}
```

## Deployment

### Build for Production
```bash
# Generate production build
npm run build

# Preview production build
npm run preview
```

### Deployment Platforms
- Vercel
- Netlify
- GitHub Pages

## Custom Domain Setup

1. Purchase domain from preferred registrar
2. Add DNS records:
```
A     @     76.76.21.21
CNAME www   yourdomain.com
```
3. Configure domain in deployment platform
4. Wait for DNS propagation (24-48 hours)

## Troubleshooting

### Common Issues

#### Images Not Loading
- Verify file paths are correct
- Check image format compatibility
- Ensure images are properly optimized

#### Build Errors
```bash
# Clear cache and node modules
rm -rf .next node_modules
npm install
```

#### Performance Issues
- Optimize images
- Minimize JavaScript bundles
- Enable caching
- Use CDN for assets

## Support & Resources

### Documentation
- [Component Documentation](docs/components.md)
- [API Reference](docs/api.md)
- [Style Guide](docs/style-guide.md)

### Support Channels
- GitHub Issues
- Email Support: support@plumbinglocalseo.com
- Community Forum: [Link]

### Useful Links
- [Contributing Guidelines](CONTRIBUTING.md)
- [License Information](LICENSE.md)
- [Change Log](CHANGELOG.md)

## License
MIT License - see LICENSE.md for details

---

**Note:** Keep this documentation updated as the project evolves. For additional support or custom modifications, contact our support team.