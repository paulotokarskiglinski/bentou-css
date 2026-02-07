# Bentou CSS Usage Guide

## Quick Start

1. Include the CSS file in your HTML:
```html
<link rel="stylesheet" href="dist/bentou.css">
```

2. Start using the components and utilities!

## Components

### Buttons

```html
<!-- Basic button -->
<button class="btn">Click me</button>

<!-- Primary button -->
<button class="btn btn-primary">Primary</button>

<!-- Accent button -->
<button class="btn btn-accent">Accent</button>

<!-- Button sizes -->
<button class="btn btn-sm">Small</button>
<button class="btn">Medium</button>
<button class="btn btn-lg">Large</button>
```

### Cards

```html
<!-- Basic card -->
<div class="card">
  <div class="card-title">Card Title</div>
  <div class="card-text">Card content goes here.</div>
</div>

<!-- Card with hover effect -->
<div class="card card-hover">
  <div class="card-title">Interactive Card</div>
  <div class="card-text">Hover over this card to see the effect.</div>
</div>

<!-- Card with footer -->
<div class="card card-hover">
  <div class="card-title">Title</div>
  <div class="card-text">Content</div>
  <div class="card-footer">
    <button class="btn">Action</button>
  </div>
</div>
```

### Badges

```html
<!-- Basic badges -->
<span class="badge">Default</span>
<span class="badge badge-primary">Primary</span>
<span class="badge badge-accent">Accent</span>
<span class="badge badge-success">Success</span>
<span class="badge badge-error">Error</span>
<span class="badge badge-warning">Warning</span>
<span class="badge badge-outline">Outline</span>

<!-- Pill badges (rounded) -->
<span class="badge badge-accent badge-pill">New</span>
<span class="badge badge-success badge-pill">Active</span>

<!-- Large badge -->
<span class="badge badge-accent badge-lg">Featured</span>

<!-- In buttons -->
<button class="btn btn-primary">
  Messages <span class="badge">5</span>
</button>

<!-- In headings -->
<h3>Features <span class="badge badge-accent badge-pill">Beta</span></h3>

<!-- Inline with text -->
<p>Status: <span class="badge badge-success">Online</span></p>
```

**Note:** Badges scale to match the size of the immediate parent element by using relative font sizing and em units.

### Forms

```html
<!-- Text inputs -->
<div class="form-group">
  <label for="email">Email</label>
  <input type="email" id="email" placeholder="your@email.com">
</div>

<div class="form-group">
  <label for="message">Message</label>
  <textarea id="message" placeholder="Your message"></textarea>
</div>

<!-- Checkboxes -->
<div class="form-group">
  <div class="form-check">
    <input type="checkbox" id="subscribe" checked />
    <label for="subscribe">Subscribe to newsletter</label>
  </div>
  <div class="form-check">
    <input type="checkbox" id="terms" />
    <label for="terms">I accept the terms</label>
  </div>
</div>

<!-- Radio buttons -->
<div class="form-group">
  <div class="form-check">
    <input type="radio" id="option1" name="options" checked />
    <label for="option1">Option 1</label>
  </div>
  <div class="form-check">
    <input type="radio" id="option2" name="options" />
    <label for="option2">Option 2</label>
  </div>
</div>

<button class="btn btn-primary">Submit</button>
```

### List Groups

```html
<!-- Basic list -->
<ul class="list-group">
  <li class="list-group-item">First item</li>
  <li class="list-group-item">Second item</li>
  <li class="list-group-item">Third item</li>
</ul>

<!-- Active and disabled states -->
<ul class="list-group">
  <li class="list-group-item active">Active item</li>
  <li class="list-group-item">Regular item</li>
  <li class="list-group-item disabled">Disabled item</li>
</ul>

<!-- Link items -->
<div class="list-group">
  <a href="#" class="list-group-item">Link item</a>
  <a href="#" class="list-group-item active">Active link</a>
  <a href="#" class="list-group-item">Another link</a>
</div>

<!-- Button items -->
<div class="list-group">
  <button type="button" class="list-group-item">Button item</button>
  <button type="button" class="list-group-item">Another button</button>
</div>

<!-- With badges -->
<ul class="list-group">
  <li class="list-group-item flex justify-between items-center">
    Notifications
    <span class="badge badge-primary badge-pill">14</span>
  </li>
  <li class="list-group-item flex justify-between items-center">
    Messages
    <span class="badge badge-accent badge-pill">2</span>
  </li>
</ul>

<!-- Contextual variants -->
<ul class="list-group">
  <li class="list-group-item list-group-item-primary">Primary</li>
  <li class="list-group-item list-group-item-accent">Accent</li>
  <li class="list-group-item list-group-item-success">Success</li>
  <li class="list-group-item list-group-item-error">Error</li>
  <li class="list-group-item list-group-item-warning">Warning</li>
</ul>

<!-- Flush variant (no borders) -->
<ul class="list-group list-group-flush">
  <li class="list-group-item">Item</li>
  <li class="list-group-item">Item</li>
</ul>

<!-- Horizontal -->
<ul class="list-group list-group-horizontal">
  <li class="list-group-item">Item 1</li>
  <li class="list-group-item">Item 2</li>
  <li class="list-group-item">Item 3</li>
</ul>
```

### Navigation

```html
<nav>
  <div class="nav-brand">Brand</div>
  <ul class="nav-links">
    <li><a href="#home">Home</a></li>
    <li><a href="#about">About</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>
```

## Layout

### Container

```html
<!-- Standard container (max-width: 1200px) -->
<div class="container">
  Content here
</div>

<!-- Small container (max-width: 800px) -->
<div class="container container-sm">
  Content here
</div>

<!-- Large container (max-width: 1400px) -->
<div class="container container-lg">
  Content here
</div>
```

### Grid System

```html
<!-- 3-column grid (responsive) -->
<div class="grid grid-cols-3">
  <div>Column 1</div>
  <div>Column 2</div>
  <div>Column 3</div>
</div>

<!-- Available columns: grid-cols-1, grid-cols-2, grid-cols-3, grid-cols-4 -->
```

### Flexbox

```html
<!-- Display utilities -->
<div class="d-flex">Display flex</div>
<div class="d-inline-flex">Display inline-flex</div>
<div class="d-block">Display block</div>
<div class="d-none">Display none</div>

<!-- Basic flex container -->
<div class="d-flex justify-content-between align-items-center">
  <div>Left</div>
  <div>Right</div>
</div>

<!-- Flex direction -->
<div class="d-flex flex-row">Row (default)</div>
<div class="d-flex flex-row-reverse">Row reversed</div>
<div class="d-flex flex-column">Column</div>
<div class="d-flex flex-column-reverse">Column reversed</div>

<!-- Flex wrap -->
<div class="d-flex flex-wrap">Wrapping flex items</div>
<div class="d-flex flex-nowrap">No wrap</div>

<!-- Justify content -->
<div class="d-flex justify-content-start">Start</div>
<div class="d-flex justify-content-end">End</div>
<div class="d-flex justify-content-center">Center</div>
<div class="d-flex justify-content-between">Space between</div>
<div class="d-flex justify-content-around">Space around</div>
<div class="d-flex justify-content-evenly">Space evenly</div>

<!-- Align items -->
<div class="d-flex align-items-start">Flex start</div>
<div class="d-flex align-items-end">Flex end</div>
<div class="d-flex align-items-center">Center</div>
<div class="d-flex align-items-baseline">Baseline</div>
<div class="d-flex align-items-stretch">Stretch</div>

<!-- Align self (on individual items) -->
<div class="d-flex">
  <div class="align-self-start">Align self start</div>
  <div class="align-self-center">Align self center</div>
</div>

<!-- Flex grow and shrink -->
<div class="d-flex">
  <div class="flex-grow-1">Grows to fill space</div>
  <div class="flex-grow-0">Won't grow</div>
</div>

<div class="d-flex">
  <div class="flex-shrink-1">Can shrink</div>
  <div class="flex-shrink-0">Won't shrink</div>
</div>

<!-- Flex fill -->
<div class="d-flex">
  <div class="flex-fill">Fills available space</div>
  <div class="flex-fill">Fills available space</div>
</div>
```

**Legacy classes:** The library also includes shorthand classes like `.flex`, `.flex-col`, `.items-center`, `.justify-between` for compatibility.

### Display

```html
<!-- Display types -->
<div class="d-none">Hidden</div>
<div class="d-block">Block level</div>
<div class="d-inline">Inline</div>
<div class="d-inline-block">Inline block</div>
<div class="d-flex">Flex container</div>
<div class="d-inline-flex">Inline flex</div>
<div class="d-grid">Grid container</div>
```

## Utilities

### Spacing

```html
<!-- Margin -->
<div class="mt-md">Margin top</div>
<div class="mb-lg">Margin bottom</div>

<!-- Padding -->
<div class="p-md">Padding all sides</div>
<div class="p-lg">Large padding</div>

<!-- Sizes: xs, sm, md, lg, xl, 2xl -->
```

### Gap

```html
<div class="flex gap-sm">Small gap</div>
<div class="flex gap-md">Medium gap</div>
<div class="flex gap-lg">Large gap</div>
```

### Text Utilities

```html
<p class="text-center">Centered text</p>
<p class="text-primary">Primary color</p>
<p class="text-secondary">Secondary color</p>
<p class="text-accent">Accent color</p>
<p class="text-sm">Small text</p>
<p class="text-lg">Large text</p>
```

### Background & Borders

```html
<div class="bg-secondary">Secondary background</div>
<div class="bg-tertiary">Tertiary background</div>

<div class="rounded-sm">Small radius</div>
<div class="rounded-md">Medium radius</div>
<div class="rounded-lg">Large radius</div>
```

### Shadows

```html
<div class="shadow-sm">Small shadow</div>
<div class="shadow-md">Medium shadow</div>
<div class="shadow-lg">Large shadow</div>
```

### Width & Height

```html
<div class="w-full">Full width</div>
<div class="h-full">Full height</div>
```

## Dark Mode

Dark mode is **automatically** enabled based on system preferences. No configuration needed!

The library uses the `prefers-color-scheme` media query to detect the user's system theme and applies the appropriate color scheme.

### Custom Dark Mode Behavior

If you want to add custom dark mode styles:

```css
@media (prefers-color-scheme: dark) {
  .my-element {
    /* Your dark mode styles */
  }
}
```

## CSS Variables

You can customize the design by overriding CSS variables:

```css
:root {
  --accent-primary: #your-color;
  --border-radius: 12px;
  /* See bentou.css for all available variables */
}
```

## Responsive Design

The library is **mobile-first** and fully responsive:

- Grid columns automatically stack on mobile
- Navigation adapts to smaller screens
- All components are touch-friendly

### Breakpoints

- Mobile: < 768px
- Tablet: 769px - 1024px
- Desktop: > 1024px

### Responsive Utilities

```html
<div class="hide-mobile">Hidden on mobile</div>
<div class="hide-desktop">Hidden on desktop</div>
```

## Typography

### Headings

```html
<h1>Heading 1</h1> <!-- 2.5rem -->
<h2>Heading 2</h2> <!-- 2rem -->
<h3>Heading 3</h3> <!-- 1.5rem -->
<h4>Heading 4</h4> <!-- 1.25rem -->
<h5>Heading 5</h5> <!-- 1.125rem -->
<h6>Heading 6</h6> <!-- 1rem -->
```

### Text Elements

```html
<p>Paragraph text</p>
<a href="#">Link</a>
<small>Small text</small>
<code>Inline code</code>
<pre><code>Code block</code></pre>
<blockquote>Quote</blockquote>
```

## Best Practices

1. **Always use the container class** for proper content width and padding
2. **Combine utility classes** for custom layouts
3. **Use semantic HTML** - the library enhances native elements
4. **Test in both light and dark modes**
5. **Keep it simple** - the library is designed to be minimal

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Examples

Check out the `examples/` folder for complete usage examples:

- `quickstart.html` - Minimal starter template
- `dist/index.html` - Full demo with all components

## Tips

1. **Combine classes**: `<button class="btn btn-primary btn-lg">Large Primary</button>`
2. **Use flexbox for layouts**: `<div class="flex justify-between items-center">`
3. **Grid is responsive**: Automatically stacks on mobile
4. **Customize with CSS variables**: Override defaults in your own CSS
5. **Add hover to cards**: Use `card-hover` class for interactive cards: `<div class="card card-hover">`

---

Need more examples? Check out the [full demo page](dist/index.html)!
