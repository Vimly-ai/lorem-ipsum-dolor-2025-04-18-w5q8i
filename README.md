# Landing Page Maintenance Guide

This guide will help you maintain and customize your landing page. Follow these detailed instructions to make common updates while preserving the design and functionality.

## Table of Contents
- [Updating Text and Styling](#updating-text-and-styling)
- [Managing Links](#managing-links)
- [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
- [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your logo and navigation menu. To update:

1. **Logo Text**
```html
<div class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
    Logo <!-- Replace "Logo" with your company name -->
</div>
```

2. **Navigation Menu Items**
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Features</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Benefits</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Contact</a>
</div>
```
To add or modify menu items, copy an existing `<a>` tag and update the text between the tags.

### Hero Section
Located at the top of the page:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8 bg-gradient-to-r from-purple-600 to-pink-600 bg-clip-text text-transparent">
    Lorem ipsum dolor <!-- Replace with your main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12 leading-relaxed">
    Lorem ipsum dolor sit amet <!-- Replace with your subheading -->
</p>
```

### Understanding Tailwind Classes
Common classes used in this template:
- `text-[size]`: Controls text size (e.g., `text-xl`, `text-2xl`)
- `mb-[size]`: Adds margin bottom (e.g., `mb-8`, `mb-12`)
- `py-[size]`: Adds padding top and bottom
- `px-[size]`: Adds padding left and right
- `bg-[color]`: Sets background color
- `text-[color]`: Sets text color

Example of updating text size:
```html
<!-- Original -->
<p class="text-xl">Your text</p>

<!-- Larger text -->
<p class="text-2xl">Your text</p>
```

## Managing Links

### Current Link Locations

1. **Navigation Menu Links**
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600">Features</a> <!-- Update href -->
    <a href="#" class="text-gray-600">Benefits</a> <!-- Update href -->
    <a href="#" class="text-gray-600">Contact</a> <!-- Update href -->
</div>
```

To update links:
1. Replace `#` with your target URL
2. For internal pages: `href="about.html"`
3. For external sites: `href="https://example.com"`

### Footer Links
```html
<!-- Company Section -->
<ul class="space-y-2">
    <li><a href="#" class="text-gray-600">About</a></li>
    <li><a href="#" class="text-gray-600">Careers</a></li>
    <li><a href="#" class="text-gray-600">Contact</a></li>
</ul>
```

To update footer links:
1. Locate the relevant section (Company, Resources, or Legal)
2. Find the `<a>` tag
3. Update the `href="#"` attribute
4. Verify the text between the tags matches your link destination

## Adding Privacy and Terms Pages

### Updating Footer Legal Links
```html
<!-- Original Legal Section -->
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Privacy</a></li>
        <li><a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Terms</a></li>
        <li><a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Security</a></li>
    </ul>
</div>
```

To link privacy and terms pages:
1. Create `privacy.html` and `terms.html` in your project folder
2. Update the links:
```html
<li><a href="privacy.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Privacy</a></li>
<li><a href="terms.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Terms</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Links**
- Check for typos in `href` attributes
- Verify file names match exactly (including case)
- Ensure files are in the correct folder

2. **Styling Problems**
- Check for missing class names
- Verify Tailwind CSS is properly loaded
- Compare with original classes when making changes

3. **Responsive Issues**
- Keep responsive classes (e.g., `md:text-2xl`)
- Test on different screen sizes
- Don't remove `viewport` meta tag

### Need Help?
- Review the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Check browser developer tools (F12) for errors
- Verify all files are in the correct location
- Double-check HTML syntax and closing tags

Remember to test all changes across different devices and browsers to ensure consistency.