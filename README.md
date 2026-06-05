# Frontend Mentor - Blog Preview Card Solution

This is my solution to the [Blog preview card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/blog-preview-card-ckPaj01IcS).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

---

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Screenshot

![Blog Preview Card Desktop Screenshot](./Screenshot%202026-06-05%20021639.png)
![Blog Preview Card Mobile Screenshot](./Screenshot%202026-06-05%20021704.png)

### Links

- Solution URL: [GitHub Repository](https://github.com/solotechrics/blog-preview-card)
- Live Site URL: [Live link](https://solotechrics.github.io/blog-preview-card/)

---

## My process

### Built with

- Semantic HTML5
- CSS custom properties
- Flexbox
- Google Fonts (Figtree)
- Mobile-first workflow

### What I learned

This challenge helped me practice using `min()` in CSS to handle responsive width without media queries — the card stays fixed at `384px` on desktop but scales down gracefully on mobile:

```css
.card {
    width: min(384px, 90%);
}
```

I also learned how to use `align-self: flex-start` inside a flex column to stop an element from stretching full width — useful for the tag badge:

```css
.tag {
    align-self: flex-start;
}
```

And I implemented a hover state on the card title by wrapping the `h1` in an anchor tag:

```css
.card a:hover h1 {
    color: var(--tag-color);
}
```

### Continued development

- Practice more hover and focus states for accessibility
- Explore CSS transitions to make hover effects smoother
- Move on to more complex multi-section layout challenges

---

## Author

- GitHub - [@solotechrics](https://github.com/solotechrics)
- Frontend Mentor - [@solotechrics](https://www.frontendmentor.io/profile/solotechrics)