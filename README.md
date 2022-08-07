# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![Desktop screenshot of the component](./images/desktop-screenshot.png?raw=true)
![Mobile screenshot of the component](./images/mobile-screenshot.png?raw=true)

### Links
- Live Site URL: [Live Site](https://wellington-damasio.github.io/product-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- Flexbox
- Mobile-first workflow
- BEM CSS Naming Conventinon
- CSS Custom Properties


### What I learned

I learned how to use the `<picture>` tag along with the `<souce>` tag to create a responsive image. It makes the image change based on the size of the screen
```html
<picture class="card__img">
  <source 
  srcset="/images/image-product-desktop.jpg"
  media="(min-width: 40em)"
  />
  <img 
    src="./images/image-product-mobile.jpg"
    alt="Perfume laid in a table with some leafs"
  />  
</picture>
```

I learned how to use the `::after` CSS property to style the price without discount.
```css
.card__price {
  display: inline-block;
  position: relative;
  color: var(--dark-cyan);
  font-size: 2rem;
  line-height: 2rem;
  font-family: 'Fraunces', serif;
  margin-bottom: 1rem;
}

.card__price::after {
  content: '$169.99';
  position: absolute;
  font-size: .8rem;
  font-family: 'Montserrat', sans-serif;
  color: var(--dark-grayishBlue);
  text-decoration: line-through;
  right: -4rem;
}
```


### Continued development
- Get better at using the BEM naming convention for classes;
- Build more component challenges to get the fundamentals of HTML, CSS and how to build interesting pieces of an application.

## Author

- Frontend Mentor - [@wellington-damasio](https://www.frontendmentor.io/profile/wellington-damasio)
- LinkedIn - [@wellington-damasio](www.linkedin.com/in/wellington-damásio-992682224)
