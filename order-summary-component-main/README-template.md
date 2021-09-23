# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- See hover states for interactive elements

My solution to this was to add a simple hover effect on the CTA button

```css
.btn:hover {
  cursor: pointer;
  background-color: #4635ff;
}
```

### Screenshots

![desktop screenshot](images\desktop-screenshot.png)
![mobile screenshot](images\mobile-screenshot.png)

### Links

- Live Site URL: (https://order-summary-component-responsive.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Desktop-first workflow

### What I learned

````css example 1
@media (max-width: 29em) {
  html {
    font-size: 50%;
  }

  body {
    background-color: #e0e8ff;
    display: flex;
  }
  .hero-img {
    transform: scale(0.8, 0.8);
    height: auto;
    object-fit: contain;
  }

  .hero-img-container {
    height: 24rem;
  }

  .container {
    background-color: #e0e8ff !important;
    background-image: none !important;
  }
}

- this has been the first media query I have written by myself,
allowing the design to be fully reponsive as per the brief,
I noticed the design broke at around 464px so even though
the brief stated for it to be responsive at 375px, I adjusted
this so that even before the design hit the required width
it already looked good and fit well on the mobile Dev Tools.


``` css example 2
.annual-plan-text li:last-child {
  color: #7280a7;
}

- Here I used a descendant selector and psuedo element
to enable me to change the text colour, a simple addition
but I was happy with how I could use the last-child to
change a specific element of the design by targeting it
this way.

``` css example 3
.annual-plan-container {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  background: #f5f7ff;
  padding: 2.4rem 0rem;
  border-radius: 15px;
  margin: 0 2.4rem;
  margin-bottom: 3.2rem;
  transition: all 0.3s;
}

- CSS Grid has helped with this design totally and
definately helps to make designs responsive.

I remembered how to layout the grid using the repeat
function and further in the design I changed the position
of specific elements with the grid-column selector
/* grid-column: span 3; */
allowing me to span the element across making it
easier for the design to be more responsive.


### Continued development

I like how I was able to use css grid/ flexbox during this project,
but to further improve I need to become more comfortable with using
properties such as flex-direction or grid-row/ grid-columns,
but overall I am happy with my progress as of the moment.

In future projects I would like to be more confident with media queries
and responsive web design.

The course that I have been learning from
has been very helpful with this but I need to practice more to
use the correct methods for example using rem instead of px.

### Useful resources

(https://stackoverflow.com/questions/787839/resize-image-proportionally-with-css)
This helped me with the responsive design of the hero image.
I would never have thought to use transform:scale and it was a great solution to the problem I had.

````
