# Bryan Engel Photography Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Bryan Engel Photography landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## 1. Updating Text and Tailwind CSS Classes

### Text Content Updates

#### Header Section
```html
<header class="sticky top-0 z-50 bg-white shadow-md">
    <nav class="container mx-auto px-4 py-4 flex items-center justify-between">
        <div class="flex items-center space-x-10">
            <a href="#" class="text-2xl font-bold text-gray-900">Bryan Engel</a>
```
To update the business name:
1. Locate the `<a>` tag containing "Bryan Engel"
2. Replace the text between the opening and closing tags
3. Keep the existing classes to maintain styling

#### Hero Section
```html
<div class="max-w-4xl mx-auto text-center text-white">
    <h1 class="text-4xl md:text-6xl font-bold mb-6 leading-tight">Bryan Engel Photography</h1>
    <p class="text-xl md:text-2xl mb-8">Taking your photography to the next level</p>
```
To modify hero content:
1. Update the `<h1>` text for the main heading
2. Modify the `<p>` text for the subheading
3. Maintain the responsive text classes (`text-4xl md:text-6xl` and `text-xl md:text-2xl`)

### Tailwind CSS Class Modifications

#### Understanding Key Classes
- Responsive prefixes: `md:` applies styles on medium screens and larger
- Spacing utilities: `px-4` (horizontal padding), `py-4` (vertical padding), `mb-6` (margin bottom)
- Flex utilities: `flex`, `items-center`, `justify-between`
- Colors: `text-gray-900`, `bg-white`, `text-white`

#### Example: Modifying Button Styles
Original:
```html
<a href="#" class="inline-block bg-white text-gray-900 px-8 py-4 rounded-lg font-semibold text-lg hover:transform hover:scale-105 transition-all duration-300 shadow-lg">
```

To change button color:
1. Replace `bg-white` with `bg-blue-500`
2. Update `text-gray-900` to `text-white`
3. Keep hover effects and transition classes

## 2. Fixing Broken Links

### Navigation Menu Links
Current navigation structure:
```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Portfolio</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Services</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">About</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Contact</a>
</div>
```

To update navigation links:
1. Replace `#` with proper page URLs
2. Example:
```html
<a href="portfolio.html" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Portfolio</a>
```

### Footer Links
Current footer structure:
```html
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Home</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Services</a></li>
```

To update footer links:
1. Replace `#` with corresponding page URLs
2. Example:
```html
<li><a href="index.html" class="text-gray-400 hover:text-white transition-colors duration-300">Home</a></li>
<li><a href="services.html" class="text-gray-400 hover:text-white transition-colors duration-300">Services</a></li>
```

## 3. Adding Privacy and Terms Pages

### Footer Modification
Add privacy and terms links to the Quick Links section:
```html
<ul class="space-y-2">
    <!-- Existing links -->
    <li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
    <li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
</ul>
```

### Alternative Footer Layout
Create a dedicated legal links section:
```html
<div class="border-t border-gray-800 mt-12 pt-8 text-center text-gray-400">
    <p>&copy; 2024 Bryan Engel Photography. All rights reserved.</p>
    <div class="mt-4">
        <a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300 mr-4">Privacy Policy</a>
        <a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a>
    </div>
</div>
```

## Troubleshooting Tips

1. **Broken Styles**
   - Check for typos in Tailwind class names
   - Ensure responsive prefixes (`md:`, `lg:`) are correctly placed
   - Verify the Tailwind CDN link is working

2. **Link Issues**
   - Confirm file names match exactly (case-sensitive)
   - Use relative paths correctly (`./` for same directory)
   - Test all links after updating

3. **Mobile Response**
   - Test menu functionality on mobile devices
   - Verify responsive classes are working as expected
   - Check image scaling on different screen sizes

## Best Practices

1. Always backup files before making changes
2. Test changes in multiple browsers
3. Maintain consistent styling across all pages
4. Keep the responsive design intact when modifying classes
5. Update meta descriptions when changing page content

Remember to validate all links and test the site thoroughly after making any modifications.