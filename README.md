# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./images/screenshot-desktop.png)

### Links

- Solution URL: [GitHub](https://github.com/mbdelarosa/stats-preview-card-component)
- Live Site URL: [Stats Preview Card Component](https://mbdelarosa.github.io/stats-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Grid
- Mobile-first workflow

### What I learned

Through this challenge, I was able to accomplish the following:
- Learn and implement Grid, and use it with Flexbox
- Try out the BEM naming convention
- Use the `<picture>` tag to serve images in different screen sizes
- Use the `mix-blend-mode` and `opacity` properties to create a gradient effect on the picture
- Learn that changing the display property of a list will sometimes remove the list semantics, but can be fixed by adding `role="list"` to the `<ul>` and `role="listitem"` to the `<li>`

Some pain points I encountered while doing this challenge:
- Scrolling and display issue when I used Flexbox on the `<body>` instead of grid for mobile display
  - To fix this, I decided to also use Grid for the mobile display and added a `max-width` for both mobile and desktop view
- Getting the gradient effect on the picture
  - I had to play around with the `.card-component__image` and `img` css blocks for this, realizing that I had to set the background color on the parent `.component__image` and the opacity on the child `img`
- Picture was shrinking inside the container when resized
  - Had to set the `width` and `height` to 100% for both `picture` and `img`

### Continued development

This was my first encounter with Grid, so I'm looking forward to using it again in future challenges. I'm also interested to read up on `clamp()` and when to use it, as I'm wondering if this could be a better tool for resizing text/images

### Useful resources

- ["Learn CSS Grid the easy way" by Kevin Powell (Youtube)](https://youtu.be/rg7Fvvl3taU) - This was a good introduction to Grid and its properties

## Author

- Frontend Mentor - [@mbdelarosa](https://www.frontendmentor.io/profile/mbdelarosa)
