# SASSFLOW Framework

**SassFlow** is a modern, comprehensive CSS framework built using Sass. It offers a scalable, modular architecture that makes it easy to create customizable UI components and utility classes. Designed to streamline and improve the consistency of web development projects, this framework was developed for educational purposes to practice and demonstrate the workflow of working with Sass.

## Authors

This project was created as an academic collaboration focused on CSS architecture, modular design systems, and Sass-driven development.

- Anna Nikiforova
- Faoziyyah Busari
- Satellite Nongmaithem
- Anuj Singh

---

## Overview

SassFlow uses a theme-first approach, with centralized variables and utility classes for layout, spacing, colors, and typography. Built entirely with Sass, it enables easy customization through maps and variables, while maintaining scalability and clean code organization across projects.

---

## 📁 Project Structure

```
📦 SASSFLOW-FRAMEWORK/
├── 📂 css
│   └── sassflow.css                  # Compiled CSS file
├── 📂 src
│   ├── 📂 base                      # Base styles including components and utilities
│   │   ├── _align.scss
│   │   ├── _buttons.scss
│   │   ├── _flex.scss
│   │   ├── _forms.scss
│   │   ├── _headings.scss
│   │   ├── _images.scss
│   │   ├── _justify.scss               
│   │   ├── _layout.scss
│   │   ├── _links.scss
│   │   ├── _lists.scss
│   │   ├── _tables.scss
│   │   ├── _utilities.scss
│   │   ├── _index.scss            # Imports all base partials
│   ├── 📂 font                      # Fonts
│   │   ├── font-inter.scss
│   │   ├── font-fira-code.scss
│   │   └── index.scss               # Imports all font partials
│   ├── 📂 reset                     # Reset styles
│   │   └── reset.scss
│   ├── 📂 variables                 # Theme variables and Sass maps
│   │   ├── colors.scss
│   │   ├── radius.scss
│   │   ├── sizing.scss
│   │   ├── theme.scss
│   │   └── typography.scss
│   │   ├── index.scss              # Imports all variables partials
│   │  
│   ├── sassflow.scss               # Main Sass entry file importing all src partials
├── index.html                      # Showcase/demo page
└── README.md 
```

---

## Features

- **Sass & Partials Architecture**  
  Modular partials keep styles organized for maintainability and reuse.

- **Custom Theming with Sass Maps**  
  Define semantic color roles (`primary`, `secondary`, `danger`, `info`, etc.) centrally to ensure consistent UI themes.

- **Comprehensive Utility Classes**   
  Utilities cover spacing, backgrounds, borders, typography, layout (flexbox), display, and sizing.

- **Well-Styled Base HTML Elements**  
  Forms, tables, headings, lists, images, and more receive consistent, theme-based styling.

- **Responsive Flexbox & Grid Systems**  
  Robust support for flexible layouts with alignment, justification, and wrapping utilities.

- **Easy to Customize**  
  Modify variables and maps under `/src/variables/` to personalize the theme and spacing.

- **Modern Sass Syntax**  
  Uses `@use` and `@forward` for modular, maintainable stylesheets.

- **Scalable Design System**  
  Combines components and utilities to maintain visually balanced interfaces.

---


## Usage

Use  the framework’s components and utilities within your HTML effortlessly.

### Buttons
- Themed colors and typography variables
- Responsive font sizes and hover transitions
- Classes: `.button-primary`, `.button-secondary`, `.button-warning`

```html
<button class="btn-primary">Primary</button>
<a href="#" class="btn-pink">Link Button</a>
```

### Typography
- Utilizes global variables for font families, weights, and sizes.
- Ensures vertical rhythm and heading hierarchy.
- Quick theme changes via Sass maps.

Example classes: `h1, h2, h3, p`, `.text-primary`, `.font-sz-lg`

```html
<h1 class="text-primary font-sz-3xl">Heading</h1>
<p class="text-dark font-sz-sm">Paragraph text</p>
```

### Spacing Utilities
Display utilities: `.d-block`, `.d-flex`, `.d-grid`  
Flex utilities: `.flex`, `.flex-row`, `.items-center`, `.justify-between`  
Spacing: `.p-4`, `.m-3`, `.gap-3`  
Visibility, text alignment, shadows, backgrounds, borders, and more.

```html
<div class="p-md mb-lg shadow-sm">Box with padding, margin, and shadow</div>
```

### Layout with Flexbox

```html
<div class="flex flex-wrap gap-md justify-center items-center">
  <div class="box-150 bg-primary text-bright-white">Box 1</div>
  <div class="box-150 bg-secondary text-bright-white">Box 2</div>
</div>

```

### Tables

Base table styling with modifiers for borders, stripes, hover states, sizing, alignment, and responsive behavior.

Example modifiers: `.table--bordered`, `.table--striped`, `.table--compact`

<table class="table table--striped table--hover">
  <thead>
    <tr>
      <th>Name</th>
      <th>Role</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>John</td>
      <td>Developer</td>
    </tr>
  </tbody>
</table>

### Forms
Well-designed form elements with visual variants and validation states.

Modifiers include `.is-sm`, `.is-lg`, `.is-outline`, `.is-filled`, `.is-error`, `.form-horizontal`, `.input-group`, `.switch`

```html
<form class="form">
  <div class="form-field">
    <label class="form-label" for="name">Name</label>
    <input type="text" id="name" class="form-control is-filled">
  </div>
  <div class="form-actions">
    <button type="submit" class="button-primary">Submit</button>
  </div>
</form>


```
### Images

Responsive images and shape classes:

- `.img-fluid`, `.img-circle`, `.img-rounded`  
- Object fit and position utilities  
- Aspect ratios with `.aspect-video`  
- Filters and hover effects  


---

## Installation

To install and start using the Framework:

### 1. Clone or Download the repository

```bash
git clone https://github.com/your-username/sassflow-framework.git
```

### 2. Include the compiled CSS file 
Add the compiled CSS file to your HTML:

```html
<link rel="stylesheet" href="./css/sassflow.css">
```

### 3. Compile Sass (for customization)

If you modify any Sass source files, recompile with:

```bash
sass --watch src/main.scss css/sassflow.css
```

---
---

## Customization

Edit Sass variables and theme maps located in `/src/variables/`  to update colors, fonts, spacing, sizing, and component styles:  

- **_colors.scss** – Define color palette
- **_theme.scss** –  Assign semantic color roles (`primary`, `danger`, `info`.),  
- **_sizing.scss** – Manage spacing, sizing, and responsive classes 
- **_typography.scss** – Configure fonts, weights, and size utilities

After updates, recompile Sass:

```bash
sass src/main.scss css/sassflow.css
```

---
## Tips

- Utility classes like `.w-full`, `.h-100`,  `.radius-gentle`, `.text-success` are dynamically from Sass maps.
-Combine utilities such as `.text-lg`, `.radius-lg`, and `.bg-primary`. for consistent styling. 
-Typography, layout, colors, and buttons sync globally via variables for easy theme adjustments.
- The design system is scalable: update one variable, and the entire framework adapts.
- Default HTML elements are styled cohesively without extra CSS.

---
## Live Demo

Open `index.html` in a browser to explore the full showcase of components, utilities, and core features.

---
## Requirements

- Sass installed (`npm install -g sass`) or use the **Live Sass Compiler** in your IDE.
- Modern browser for preview.
- Basic understanding of Sass and HTML.
- Dart Sass recommended for @use and @forward support.

---
## License

This project is open source and free for personal and educational use.
