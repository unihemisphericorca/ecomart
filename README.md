EcoMart – Project README
Project Overview
EcoMart is a three-page static website for an eco-friendly online store.
Built using only basic HTML and CSS — no JavaScript frameworks, no libraries.

---
Project Structure
```
ecomart/
├── index.html        ← Page 1: Home Page
├── catalog.html      ← Page 2: Product Catalog
├── contact.html      ← Page 3: Contact Form
└── css/
    └── styles.css    ← ONE shared stylesheet for all three pages
```
---
How to Run
Download and extract the zip file
Open the `ecomart/` folder
Double-click `index.html` to open it in your browser
Use the navigation links (Home | Catalog | Contact) to move between pages
No installation, no server, no terminal needed.

---
Pages
Page 1 — Home (`index.html`)
Header with logo and navigation
Hero section: banner image, heading, description, "Shop Now" button
Three feature cards in a 3-column grid
Footer with 3 columns (About, Help, Legal) and copyright

Page 2 — Catalog (`catalog.html`)
Same header and hero as Home
Product grid with 5 product cards (auto-fit responsive grid)
Each card has an image, name, description, and "Add to Cart" button
Same footer

Page 3 — Contact (`contact.html`)
Same header and hero
Contact form in a 2-column grid layout:
Name and Email side by side
Subject (full width)
Message textarea (full width)
Send Message and Clear buttons
Same footer

---
Stylesheet (`css/styles.css`)
All three pages share one stylesheet. Sections in the file:
Section	Purpose
Reset	Removes browser default margin/padding
Body	Sets font (Arial) and background (#f3f4f6)
.container	Centres content, max-width 1100px
Links	Blue (#0d6efd), underline on hover
Header	Dark bg (#1f2937), white text, flexbox layout
.btn	Blue button, rounded corners, hover darken
.cards-grid	3-column CSS Grid for feature cards
.product-grid	Auto-fit grid for catalog products
.contact-form	2-column grid for form fields
Footer	Dark bg (#111827), 3-column grid, copyright bar
@media 768px	Tablet: 2-column cards, 1-column footer and form
@media 480px	Mobile: 1-column everything, stacked header

---
Color & Style Guide
Element	Value
Body font	Arial, sans-serif
Body background	#f3f4f6
Primary color (buttons, links)	#0d6efd
Header background	#1f2937
Header text	white
Footer background	#111827
Footer text	#9ca3af
Container max-width	1100px
Button style	Rounded corners, white text, bold, hover darken

---
Responsive Breakpoints
Screen Width	Layout
> 768px (Desktop)	3-column cards, 2-column form, 3-column footer
≤ 768px (Tablet)	2-column cards, 1-column form, 1-column footer
≤ 480px (Mobile)	1-column everything, stacked header nav
---
Key HTML & CSS Concepts Used
Flexbox — used in the header to push the logo left and nav right.
CSS Grid — used for feature cards, product grid, contact form, and footer columns.
auto-fit + minmax — the catalog grid automatically adjusts the number of columns based on screen width.
Media queries — `@media (max-width: 768px)` and `@media (max-width: 480px)` handle tablet and mobile layouts.
Shared stylesheet — one `styles.css` file linked by all three pages so any style change applies site-wide.
Semantic HTML — `<header>`, `<main>`, `<section>`, `<footer>`, `<nav>` used instead of generic `<div>` tags where appropriate.
type="reset" button — the Clear button on the contact form resets all fields using a built-in browser feature, no JavaScript required.

---
External Resources
Placeholder images provided by dummyimage.com.
No other external libraries or dependencies used.

---
Author Notes
All pages use the same header and footer (copy-pasted across files — in a real project you would use a templating system or JavaScript to avoid repetition)
The "Add to Cart" and "Send Message" buttons do not have backend functionality — this is a front-end only project
The form uses `action="#"` which prevents any real submission
