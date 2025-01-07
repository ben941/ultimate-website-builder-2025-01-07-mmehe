# Ultimate Website Builder - Landing Page Maintenance Guide

This guide will help you maintain and customize the Ultimate Website Builder landing page. Whether you're new to web development or just getting started, follow these instructions to make updates while preserving the design integrity.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the logo and navigation menu. To update:

1. Change the logo text:
```html
<!-- Find this line in the header -->
<div class="text-2xl font-bold text-blue-600">UWB</div>
```
Simply replace "UWB" with your desired text.

### Hero Section
Located at the top of the page with the main headline:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold tracking-tight mb-8">Ultimate Website Builder</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">Best AI Website Builder In The World</p>
```

To modify:
- Replace the h1 text for your main headline
- Update the paragraph text for your subheading
- Keep the existing classes to maintain responsive design

### Features Section
The features section uses a three-column grid. Each feature has:
- An icon
- A heading
- Description text

To update a feature:
```html
<div class="group p-8 rounded-2xl border border-gray-200 hover:shadow-xl transition-all duration-300">
    <div class="text-blue-600 mb-4">
        <i class="fas fa-robot text-3xl"></i> <!-- Change icon class here -->
    </div>
    <h3 class="text-xl font-semibold mb-4">AI Generated</h3> <!-- Update heading -->
    <p class="text-gray-600">Leverage cutting-edge AI technology...</p> <!-- Update description -->
</div>
```

### Understanding Tailwind Classes
Key classes explained:
- `text-[size]`: Controls text size (xl, 2xl, 3xl, etc.)
- `mb-[size]`: Adds margin bottom (4, 8, 12, etc.)
- `py-[size]`: Adds padding top and bottom
- `px-[size]`: Adds padding left and right
- `bg-[color]`: Sets background color
- `text-[color]`: Sets text color

## Managing Links

### Navigation Menu Links
Current navigation links are:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

To update:
1. Locate the link you want to change
2. Modify the `href` attribute
3. Update the link text

Example:
```html
<!-- From -->
<a href="#features">Features</a>
<!-- To -->
<a href="#services">Services</a>
```

### Call-to-Action Buttons
The main CTA buttons currently point to "https://uwb.com":
```html
<a href="https://uwb.com" class="inline-block px-8 py-4...">Start Building Now</a>
```

Update all instances of "https://uwb.com" to your actual website URL.

## Adding Privacy and Terms Pages

### Step 1: Create New Pages
Create two new files in your website directory:
- privacy.html
- terms.html

### Step 2: Update Footer Links
Locate the legal section in the footer:
```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

Update the links:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Layout**
   - Check that you haven't removed any essential Tailwind classes
   - Verify all opening tags have matching closing tags
   - Ensure container divs remain intact

2. **Missing Icons**
   - Confirm the Font Awesome CDN link is present in the head section
   - Verify icon class names are correct (e.g., `fa-robot`, `fa-bolt`)

3. **Links Not Working**
   - Check for typos in href attributes
   - Ensure file names match exactly (case-sensitive)
   - Verify file paths are correct

### Need Help?
If you encounter issues:
1. Check the HTML structure matches the original
2. Verify all required CSS classes are present
3. Test links in a web browser
4. Use browser developer tools (F12) to inspect elements

Remember to always backup your files before making changes!

For additional support, contact admin@uwb.com or refer to the documentation.