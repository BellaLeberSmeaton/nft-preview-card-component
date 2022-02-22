# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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
- See hover states for interactive elements

### Screenshot

![ntf-preview-card screenshot](./images/screenshot-hover.png)

### Links

- [Repo Url](https://github.com/BellaLeberSmeaton/nft-preview-card-component)
- [Live site URL here](https://laughing-almeida-fce662.netlify.app)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

The use of flex-box mixed with position and z-index to help create the hover state of the top image over the back image.

I'm proud of the hover states:

```css
.--img {
  width: 100%;
  position: relative;
  height: 335px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.__img-bottom {
  z-index: 0;
  position: absolute;
  max-width: 335px;
  border-radius: 10px;
}

.__img-top {
  display: none;
}

.--img:hover .__img-top {
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1;
  height: 100%;
  width: 100%;
  border-radius: 10px;
  background-color: hsl(178, 100%, 50%, 0.3);
  cursor: pointer;
}
```

### Continued development

I definitely want to learn more about media queries to better understand breakpoints and how I can apply them to all the devices.

### Useful resources

- [Tutorial Republic resource 1](https://www.tutorialrepublic.com/faq/how-to-change-image-on-hover-with-css.php#:~:text=Answer%3A%20Use%20the%20CSS%20background,change%20the%20image%20on%20mouseover.) - This helped me with understanding the positioning method, that the relative image sits at the base level, and the top images sit upon as position absolute. This was paired with z-index for ordering.

## Author

- [Bella Leber Smeaton - LinkedIn](https://www.linkedin.com/in/bella-leber-smeaton/)
