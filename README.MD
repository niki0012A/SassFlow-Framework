# SASSFLOW Framework

**Sassflow** is a small framework that includes all the essential basic customizations. This framework was created for educational purposes to help us practice the workflow of working with Sass.

---

## Authors

**Sassflow** was created as part of an academic project focused on CSS architecture, modular design systems, and Sass-based development.

Created by:  
- Anna Nikiforova
- Faoziyyah Busari 
- Satellite Nongmaithem
- Anuj Singh

---

## Overview



---

## 📁 Project Structure





---

## Features

## USAGE


### TABLE
The .table class provides a styled base for any HTML <table>.
<table class="table">
  <thead>
    <tr>
      <th>Month</th>
      <th>Sales</th>
      <th>Growth</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$5,400</td>
      <td>+8%</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$6,200</td>
      <td>+15%</td>
    </tr>
  </tbody>
</table>

Modifier classes:
| Class                                                               | Description                                   |
| ------------------------------------------------------------------- | --------------------------------------------- |
| `.table--bordered`                                                  | Adds a border around all cells                |
| `.table--striped`                                                   | Alternates row background colors              |
| `.table--hover`                                                     | Highlights rows on hover                      |
| `.table--sm`, `.table--lg`, `.table--xl`                            | Adjusts cell padding                          |
| `.table--compact`, `.table--dense`                                  | Reduces vertical spacing                      |
| `.table--align-top`, `.table--align-middle`, `.table--align-bottom` | Controls vertical alignment                   |
| `.table-responsive`                                                 | Enables horizontal scrolling on small screens |




### FORMS

<form class="form">
  <div class="form-field">
    <label class="form-label" for="email">Email</label>
    <input type="email" id="email" class="form-control" placeholder="name@example.com" required />
    <span class="form-help">We’ll never share your email.</span>
  </div>

  <div class="form-field">
    <label class="form-label">Message</label>
    <textarea class="form-control" rows="4"></textarea>
  </div>

  <div class="form-actions">
    <button class="btn btn-primary">Submit</button>
  </div>
</form>

Modifiers
| Modifier                                         | Description                                           |
| ------------------------------------------------ | ----------------------------------------------------- |
| `.is-sm`, `.is-lg`                               | Size variants for inputs                              |
| `.is-outline`, `.is-filled`, `.is-ghost`         | Visual style variants                                 |
| `.is-error`, `.has-error`, `.is-success`         | Validation states                                     |
| `.form-horizontal`                               | Two-column layout with labels and inputs side-by-side |
| `.input-group`, `.addon`                         | Combine inputs and add-ons                            |
| `.input-with-icon`                               | Position icons inside input fields                    |
| `.switch`, `.control-radio`, `.control-checkbox` | Custom controls                                       |
| `.input-file`                                    | Styled file uploader                                  |
| `.form-help`, `.error-text`, `.success-text`     | Helper and feedback text                              |


### UTILITIES

Display
<div class="d-none"></div>
<div class="d-block"></div>
<span class="d-inline"></span>
<span class="d-inline-block"></span>
<div class="d-flex"></div> 
<div class="d-grid"></div>

Gaps (axis-specific; works with flex or grid)
<div class="d-flex gap-x-sm gap-y-xs">…</div>

Position & Layering
<div class="relative">
  <span class="absolute top-0 right-0 z-20">…</span>
</div>

Overflow & Object Fit
<div class="overflow-hidden">…</div>
<img class="object-cover" src="hero.jpg" alt="">

Visibility & Cursor
<button class="pointer">Clickable</button>
<span class="sr-only">Screen reader text</span>

Text helpers
<p class="text-center uppercase no-wrap truncate">…</p>
<p class="fw-semibold leading-relaxed">…</p>

Background & Border colors (theme-mapped)
<div class="bg-primary border-danger">…</div>
<div class="bg-muted border-2 border-dashed">…</div>

Shadows
<div class="shadow-sm"></div>
<div class="shadow-lg"></div>

Containers
<section class="container container-comfortable">…</section>

Aspect Ratios
<div class="aspect-video">
  <iframe …></iframe>
</div>

Opacity
<div class="opacity-50">Faded</div>


### FLEX

Flex Container
<div class="flex flex-row">
  <div>Item 1</div>
  <div>Item 2</div>
</div>

<div class="inline-flex flex-col">
  <span>Child A</span>
  <span>Child B</span>
</div>

Direction & Wrapping
<div class="flex flex-col-reverse flex-wrap">
  <div>Box A</div>
  <div>Box B</div>
</div>

Align Items & Self
<div class="flex items-center">
  <img src="icon.svg" alt="">
  <p class="self-end">Aligned bottom</p>
</div>

Grow, Shrink, and Flex Basis
<div class="flex">
  <div class="grow">Expands to fill</div>
  <div class="grow-0 basis-200">Fixed 200px width</div>
</div>

Order
<div class="flex">
  <div class="order-2">Second</div>
  <div class="order-1">First</div>
</div>


### JUSTIFY

Justify Content (Main Axis)
<div class="flex justify-between">
  <div>Left</div>
  <div>Right</div>
</div>

<div class="flex justify-center">
  <p>Centered horizontally</p>
</div>

Align Content (Cross Axis for Multi-Line Flex)
<div class="flex flex-wrap content-around">
  <div>Box A</div>
  <div>Box B</div>
  <div>Box C</div>
</div>

### IMAGES

Responsive Images
<img src="team.jpg" alt="Team" class="img-fluid">
<img src="banner.jpg" alt="Banner" class="img-full">

Shape Utilities
<img src="avatar.jpg" alt="User" class="img-circle">
<img src="product.jpg" alt="Item" class="img-rounded img-shadow">

Borders & Shadows
<img src="logo.png" alt="Logo" class="img-border-primary img-shadow-lg">

Object Fit & Position
<img src="cover.jpg" alt="Cover" class="object-cover object-center">

Aspect Ratios
<div class="aspect-video">
  <img src="video-thumbnail.jpg" class="object-cover" alt="Video">
</div>

Filters & Effects
<img src="portrait.jpg" class="img-grayscale img-hover-zoom" alt="Stylized Portrait">

Framed Image
<div class="img-frame">
  <img src="photo.jpg" class="img-fluid" alt="Framed">
</div>


