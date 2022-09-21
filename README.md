# Frontend Mentor - FAQ accordion card solution

This is a solution to the [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

No JS :)

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked


### Links

- Solution URL: [Frontend Mentor](https://www.frontendmentor.io/solutions/no-js-challenge-evcrZ1wrDG)
- Live Site URL: [live site URL](https://rynex-zv.github.io/faq-accordion-card-main/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- npm


### What I learned

- `<details>` was new to me!

- How to target outer element with CSS 
[stackoverflow](https://stackoverflow.com/questions/49022545/hover-on-div-affects-outside-element)
```css
.parent{
    pointer-events: none;
}
.childe{
    cursor: pointer;
    }
 .parent:hover ~ .element-after-parent {
            transform: translate(-7.7em, 8em) translate(-3em);
            filter: drop-shadow(-0.5em 1.5em 0.9em $VeryDarkGrayishBlue);
        }
```

- Drop shadow for PNG or SVG image in CSS
[stackoverflow](https://stackoverflow.com/questions/3186688/drop-shadow-for-png-image-in-css)
```css
.SVG{
 -webkit-filter: drop-shadow(5px 5px 5px #222);
  filter: drop-shadow(5px 5px 5px #222);
}
```

- How to use shrink in grid
[stackoverflow](https://stackoverflow.com/questions/19848697/css-grid-where-one-column-shrinks-to-fit-content-the-other-fills-the-remaning-s)
```css
.grid {
  display: grid;
  ...
  grid-template-columns: auto minmax(0, 1fr);
  grid-template-areas: "sidebar content";
}
.sidebar {
  grid-area: sidebar;
}
.content {
  grid-area: content;
}
```

- How do I remove or disable old property to keep clean
[stackoverflow](https://stackoverflow.com/questions/46009494/how-do-i-remove-or-disable-min-height-for-my-mobile-page)
```css
.proud-of-this-css {
min-height:initial;
}
//then remove it and place the property in @media 
```


### Useful resources

See above!

## Author

  - LinkedIn - [Rynex Akil](https://www.your-site.com)
  - Frontend Mentor - [@rynex-zv](https://www.frontendmentor.io/profile/rynex-zv)