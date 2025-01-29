# Landing Page Maintenance Guide

This guide will help you maintain and customize your landing page. Follow these instructions carefully to make updates while preserving the design and functionality.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<div class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-blue-500 bg-clip-text text-transparent">
    Logo <!-- Replace "Logo" with your company name -->
</div>
```

#### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-extrabold text-gray-900 mb-8">
    Lorem ipsum dolor <!-- Replace with your main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Lorem ipsum dolor sit amet <!-- Replace with your subheadline -->
</p>
```

To update text:
1. Locate the section you want to change
2. Replace the placeholder text between the opening and closing tags
3. Keep the HTML tags intact
4. Save and refresh to see changes

### Tailwind CSS Classes Explained

Key classes used in this landing page:

- Container and spacing:
  - `container mx-auto`: Centers content and sets max-width
  - `px-6`: Adds horizontal padding
  - `py-4`: Adds vertical padding

- Responsive design:
  - `md:`: Applies styles on medium screens (768px+)
  - `lg:`: Applies styles on large screens (1024px+)
  - Example: `text-4xl md:text-5xl lg:text-6xl`

- Colors and gradients:
  - `bg-white`: White background
  - `text-gray-600`: Gray text
  - `from-purple-600 to-blue-500`: Gradient colors

To modify classes:
1. Find the element you want to change
2. Add or remove classes within the `class=""` attribute
3. Maintain responsive classes (md:, lg:) to preserve mobile-friendly design

## 2. Fixing Broken Links

### Navigation Menu Links
Current placeholder links in the header:
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900">Features</a>
    <a href="#" class="text-gray-600 hover:text-gray-900">Benefits</a>
    <a href="#" class="text-gray-600 hover:text-gray-900">About</a>
    <a href="#" class="text-gray-600 hover:text-gray-900">Contact</a>
</div>
```

To update links:
1. Replace `#` with your actual URL
2. Example: `<a href="about.html">` for internal pages
3. Example: `<a href="https://example.com">` for external links

### Footer Links
```html
<ul class="space-y-3">
    <li><a href="#" class="hover:text-white">About</a></li>
    <li><a href="#" class="hover:text-white">Careers</a></li>
    <li><a href="#" class="hover:text-white">Contact</a></li>
</ul>
```

Follow the same process to update footer links.

## 3. Adding Privacy and Terms Pages

### Footer Modification
Add these links to your footer column:

```html
<div>
    <h3 class="text-white text-lg font-semibold mb-4">Legal</h3>
    <ul class="space-y-3">
        <li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

Insert this code within the footer's grid:
```html
<div class="grid grid-cols-1 md:grid-cols-4 gap-12">
    <!-- Add the Legal section here -->
</div>
```

## Troubleshooting Tips

1. If styles aren't applying:
   - Check for typos in class names
   - Ensure Tailwind CSS is properly loaded
   - Verify closing tags match opening tags

2. If links aren't working:
   - Confirm file paths are correct
   - Check for proper URL formatting
   - Verify files exist in the specified location

3. If layout breaks:
   - Don't remove responsive classes (md:, lg:)
   - Maintain the container structure
   - Keep the grid system intact

## Best Practices

1. Always test changes on multiple screen sizes
2. Back up files before making changes
3. Maintain consistent spacing and formatting
4. Keep the responsive design intact
5. Test all links after updating

Need more help? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).