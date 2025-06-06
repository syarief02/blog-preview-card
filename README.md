# Frontend Mentor – Blog Preview Card Solution

This is a front‐end solution built for the [Blog Preview Card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS). It demonstrates a responsive card component displaying a blog article preview with hover states and mobile‐first styling.

---

## Table of Contents

- [Overview](#overview)

  - [The Challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)

- [My Process](#my-process)

  - [Built With](#built-with)
  - [What I Learned](#what-i-learned)
  - [Continued Development](#continued-development)
  - [Useful Resources](#useful-resources)

- [Author](#author)
- [Acknowledgments](#acknowledgments)

---

## Overview

### The Challenge

The goal of this challenge is to build out a responsive blog preview card component using semantic HTML and modern CSS (custom properties, Flexbox, mobile‐first layout). Users should be able to:

- View the card on mobile (375px) with the illustration on top and content stacked below.
- View the same card on desktop, centered on a yellow background (no separate two‐column layout).
- See a hover state: when hovering anywhere on the card, the title turns gold and the card lifts slightly.
- Use semantic markup and follow the provided style guide for colors, typography, and spacing.

### Screenshot

Preview of the final design:

<p align="center">
  <img src="./preview.jpg" alt="Blog preview card screenshot" width="600">
</p>

> **Note:** For a closer look at mobile vs. desktop, resize your browser window or view on an actual device.

### Links

- **Solution Repository:** [github.com/syarief02/blog-preview-card](https://github.com/syarief02/blog-preview-card)
- **Live Site URL:**

[syarief02.github.io/blog-preview-card](https://syarief02.github.io/blog-preview-card)

---

## My Process

### Built With

- **HTML5** for semantic markup
- **CSS3** (Custom Properties, Flexbox)
- **Mobile‐First Workflow** (design and layout start at 375px width)
- **Google Fonts – Figtree** (Weights: 500, 800)
- **[Frontend Mentor Style Guide](./style-guide.md)** for color and typography reference

### What I Learned

- **Mobile‐First Design**

  - The card had to remain a single column at all breakpoints. Instead of switching to a two‐column layout on desktop, the container stays fixed at 375px wide, and extra yellow “canvas” shows on either side.

- **Hover States & Transitions**

  - Applying a subtle `transform: translateY(-5px)` on `.card:hover` creates a lifted effect.
  - Transitioning the heading color on hover (`.card:hover .card__title`) makes the title text turn gold.

- **Using CSS Custom Properties**

  - Defined root variables for color palette, font sizes, border radius, and shadow.
  - This makes it easy to tweak colors (e.g., the “Learning” pill background and hover title color) in one place.

- **Semantic HTML Structure**

  - Used `<article>` for the card, `<div class="card__image">` for the illustration wrapper, and `<div class="card__content">` for textual content.
  - The author section is grouped inside a `<div class="card__author">` with an `<img>` for the avatar and a `<span>` for the name.

- **CSS Flexbox for Vertical Alignment**

  - Inside `.card__content`, `display: flex; flex-direction: column; gap: 1rem;` allows the author row to auto‐align at the bottom with `margin-top: auto;`.

### Continued Development

- **Accessibility Improvements**

  - Add `alt` text improvements (e.g., more descriptive text for the illustration).
  - Make the card focusable via keyboard and ensure the hover/focus state applies to keyboard users as well.

- **Refinement of Responsive Images**

  - Consider using `srcset` for the illustration to serve an SVG fallback or different image formats (e.g., WebP) based on browser support.

- **Component Reusability**

  - Refactor the card into a reusable component (e.g., React/Vue) to accept dynamic props (category, date, title, description, author) and easily generate multiple cards.

### Useful Resources

- [Frontend Mentor Blog Preview Card Challenge](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS) – Official challenge description, design files, and requirements.
- [Google Fonts – Figtree](https://fonts.google.com/specimen/Figtree) – The font family used for headings and body text.
- [CSS Tricks – Using CSS Custom Properties](https://css-tricks.com/using-css-variables/) – A helpful guide to organizing and leveraging custom properties.
- [MDN – Flexbox Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout) – Reference for flex alignment patterns used to position elements inside the content area.

---

## Author

**Syarief Azman**

- GitHub: [@syarief02](https://github.com/syarief02)
- Frontend Mentor: [@syarief02](https://www.frontendmentor.io/profile/syarief02)

---

## Acknowledgments

- Thanks to **Frontend Mentor** for providing detailed design specs and a real‐world project scenario.
- Inspiration from the official [style-guide.md](./style-guide.md) included in the starter code.
- Special thanks to the Figtree font designers and the CSS-Tricks community for in-depth Flexbox and custom property resources.

---

_Feel free to fork this repository, clone it, or submit pull requests if you have suggestions or improvements!_
