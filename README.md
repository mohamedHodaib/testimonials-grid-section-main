# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

- Desktop design
![](./images/desktop-design.jpg)

- Mobile design
![](./images/mobile-design.jpg)

### Links

- Solution URL: [https://github.com/mohamedHodaib/testimonials-grid-section](https://github.com/mohamedHodaib/testimonials-grid-section)
- Live Site URL: [https://mohamedhodaib.github.io/testimonials-grid-section/](https://mohamedhodaib.github.io/testimonials-grid-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Responsive Web Design

### What I learned

This project was a great practice for **CSS Grid**. I learned how to create a complex grid layout by spanning columns and rows to create the specific "bento box" style design.

I am particularly proud of how I handled the 5th card (Kira's card), which spans two rows on desktop to create the vertical sidebar effect:

```css
.container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(2, auto);
    gap: 30px;
}

/* The vertical card on the right */
.box:nth-child(5) {
    grid-row: 1 / 3;
    grid-column: 4;
}
```

### Continued development

In future projects, I want to focus on:

- **Mobile-first workflow:** Currently, I designed the desktop view first and used `max-width` media queries for mobile. In the future, I aim to start with mobile styles and use `min-width` for larger screens.
- **BEM Naming Convention:** I want to improve my class naming structure (e.g., changing `.box` to something like `.testimonial-card`) to make the code more maintainable for larger teams.

## Author

- GitHub - [Mohamed Hodaib](https://github.com/mohamedHodaib)
- Frontend Mentor - [@mohamedHodaib](https://www.frontendmentor.io/profile/mohamedHodaib)
- LinkedIn - [Mohamed Hodaib](https://www.linkedin.com/in/mohamed-hodaib-2670b2344/)
