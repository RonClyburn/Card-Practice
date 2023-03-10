# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

LIVE SITE: https://cardpracticesite.netlify.app/

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

## My process

I found that starting with the HTML elements and then working on styling next was an effecient way to complete this task. I used an ```<article>```html tag to create the card, and used ```<div>```'s to seperate different collections of the content inside. I approached this with a mobile first view and then set a @media query with a minimum screen width and different display properties to allow the content to be responsive with various screen sizes. I then set a maximum height on the card to ensure it would stay at the size needed per the design preview.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow

### What I learned

-HTML
  
```html 
  <picture class="product__img">
  <source srcset="./img/image-product-desktop.jpg" media="(min-width: 550px)" />
  <img src="./img/image-product-mobile.jpg" alt="Perfume" />
  </picture>
  ```
By adding the
```<source>``` 
tag with a minimum width, I was able to instruct the HTML to switch between the desktop image and mobile image at whenver the user's screen reached a certain width.

-CSS
  
```css
  {
  --dark-cyan: hsl(158, 36%, 37%);
  --darker-cyan: hsl(158, 36%, 22%);
  --cream: hsl(30, 38%, 92%);
  --very-dark-blue: hsl(212, 21%, 14%);
  --dark-gray-blue: hsl(228, 12%, 48%);
  --white: hsl(0, 0%, 100%);
  --fw--regular: 500;
  --fw-bold: 700;
  --ff-accent: "Fraunces", serif;
  --ff-base: "Montserrat", sans-serif;
}
  ```

By using the :root property I was able to easily keep track of items that I knew I would be frequently using throughout the project. This streamlined the process and made sure that all components were identical throughout.
