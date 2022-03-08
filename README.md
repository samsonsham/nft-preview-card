# Frontend Mentor - QR code component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![](https://ik.imagekit.io/c5xc1x6srka/screenshot/screen-nft-preview-card_lu-F8Slu2.png)

### Links

- Solution URL: [https://github.com/samsonsham/nft-preview-card](https://github.com/samsonsham/nft-preview-card)
- Live Site URL: [https://samsonsham.github.io/nft-preview-card/](https://samsonsham.github.io/nft-preview-card/)

## My process

- Set up SCSS file structure. Define all the styles given by style guide, including colours and font into SCSS files.
- Define components and setup corresponding DOM elements in HTML file.
- Build each elements by with colours, alignment, and adjusting size.
- Add interactive effects onto image and hyperlinks.

### Built with

- Semantic HTML5 markup
- SCSS
- Flexbox
- Transition

### What I learned

As the structure of this Card is more complicated than the QR Code one, this is a good practice for [BEM](https://en.bem.info/methodology/quick-start/#block) concepts with building independent block. One major challenge would be the interactive of the main image. Besides getting used to `transition` which give a fancy `hover` effect, I learnt to create a background image with colour overlay by a creative use of `box-shadow` inset. I learnt to make a responsive background image by using a percentage `padding-top`/`padding-bottom` as well.

```css
.card__img {
  background: url("../images/image-equilibrium.jpg");
  background-repeat: no-repeat;
  background-size: 100%;
  background-position: center;
  transition: box-shadow 0.5s ease;
  border-radius: 15px;
  width: 100%;
  height: 0;
  padding-bottom: 100%;
  opacity: 1;
}
.card__img:hover {
  box-shadow: inset 0 0 0 2000px $cyan_overlay;
}
```

## Author

- Website - [Samson Sham](https://samson-sham-portfolio.vercel.app)
- Frontend Mentor - [@samsonsham](https://www.frontendmentor.io/profile/samsonsham)
- Twitter - [@samson_sham](https://www.twitter.com/samson_sham)
