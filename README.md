# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
- [The challenge](#the-challenge)
- [Links](#links)
- [Built with](#built-with)
- [What I learned](#what-i-learned)
- [Useful resources](#useful-resources)
- [Author](#author)

## Overview

Product preview card component built using HTML and CSS. It changes layout and image depending on the device's screen size.

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

### Built with

- HTML5
- CSS
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

picture element
@media - media queries
mobile first workflow

html:
<picture>

    <source
              srcset="images\image-product-desktop.jpg"
              media="(min-width:40rem)"
              alt="Gabrielle Channel perfume bottle"
            />
    <img
              src="images/image-product-mobile.jpg"
              alt="Gabrielle Channel perfume bottle"
              class="product-image"
            />
    </picture>

css:
@media (min-width: 40rem) {
main {
max-width: 37rem;

          grid-template-columns: repeat(2, 1fr);

          gap: 0;

}
.product-image {
border-top-right-radius: 0;
border-bottom-left-radius: 0.6rem;
width: 100%;
}
.product-info {
gap: 1.5rem;
padding-right: 10%;
}
.product-type {
padding-top: 1.5rem;
}
.prices {
margin-top: 0;
}
}

### Useful resources

-[Learn CSS Grid the easy way](https://www.youtube.com/watch?v=rg7Fvvl3taU) - This video by Kevin Powell helped me better understand CSS grid, how to use media queries for this project, and how to approach mobile-first workflow.

## Author

- Frontend Mentor - [@jrc17](https://www.frontendmentor.io/profile/jrc17)
