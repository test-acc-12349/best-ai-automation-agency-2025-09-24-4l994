# AI Agency Landing Page - Maintenance Guide

This guide will help you maintain and customize the AI Agency landing page. Whether you're new to web development or need a quick reference, follow these instructions to make common updates safely and effectively.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains your company name and navigation menu. To update:

```html
<!-- Company Name -->
<div class="text-2xl font-bold bg-gradient-to-r from-purple-600 to-blue-500 bg-clip-text text-transparent">
    AI Agency  <!-- Change this text to your company name -->
</div>
```

### Hero Section
Located at the top of the page with the main headline:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8 bg-gradient-to-r from-purple-600 to-blue-500 bg-clip-text text-transparent">
    Best AI Automation Agency  <!-- Update this headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Transform your business with cutting-edge AI automation  <!-- Update this subheading -->
</p>
```

### Features Section
To modify feature cards:

1. Locate the `features` section
2. Each feature is contained in a `div` with these classes:
```html
<div class="p-8 rounded-2xl bg-white shadow-lg hover:shadow-xl transition-shadow duration-300">
    <h3 class="text-xl font-semibold mb-4">Free Builds</h3>  <!-- Feature title -->
    <p class="text-gray-600">Custom AI solutions built specifically for your business needs.</p>  <!-- Feature description -->
</div>
```

### Understanding Tailwind Classes
Common classes used in this template:

- Layout Classes:
  - `container`: Centers content
  - `mx-auto`: Horizontal auto margins
  - `px-6`: Horizontal padding
  - `py-4`: Vertical padding

- Responsive Classes:
  - `md:text-4xl`: Applies on medium screens and up
  - `lg:text-6xl`: Applies on large screens and up

## Managing Links

### Navigation Menu Links
Update the navigation menu links in the header:

```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Features</a>
    <a href="#benefits" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Benefits</a>
    <!-- Add or modify links here -->
</div>
```

### Call-to-Action Links
Replace the placeholder links:

```html
<!-- Change 'https://test.com' to your actual URL -->
<a href="https://test.com" class="inline-block px-8 py-4 bg-gradient-to-r from-purple-600 to-blue-500 text-white font-bold rounded-full">
    Start Your AI Journey
</a>
```

### Contact Information
Update email addresses:

```html
<!-- In the contact section -->
<p class="text-xl mb-12">Contact us at test@test.com</p>  <!-- Change email address -->

<!-- In the footer -->
<p class="text-gray-400">test@test.com</p>  <!-- Change email address -->
```

## Adding Privacy and Terms Pages

### Step 1: Create New Pages
Create two new files in your project directory:
- `privacy.html`
- `terms.html`

### Step 2: Update Footer Links
Replace the placeholder links in the footer:

```html
<div>
    <h4 class="text-lg font-semibold mb-4">Legal</h4>
    <ul class="space-y-2 text-gray-400">
        <li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

### Step 3: Maintain Consistent Styling
When creating privacy.html and terms.html, copy these essential elements from index.html:
- The `<head>` section with CSS links
- Header and footer sections
- Basic page structure

## Troubleshooting

### Common Issues and Solutions

1. **Broken Links**
   - Check that all `href` attributes start with either:
     - `#` for page sections
     - `https://` for external links
     - Filenames (e.g., `privacy.html`) for internal pages

2. **Responsive Design Issues**
   - Ensure you keep the responsive classes:
     - `md:` prefix for medium screens
     - `lg:` prefix for large screens
   - Don't remove `container` or `mx-auto` classes

3. **Gradient Text Not Showing**
   - Keep these classes together for gradient text:
     ```html
     bg-gradient-to-r from-purple-600 to-blue-500 bg-clip-text text-transparent
     ```

### Need Help?
- Double-check your changes against the original code
- Use browser developer tools (F12) to inspect elements
- Ensure all HTML tags are properly closed
- Maintain the existing class structure when making changes

Remember to test your changes across different screen sizes using browser developer tools before publishing updates.