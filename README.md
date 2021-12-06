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

![](./screenshot.jpg)




### Links

- Solution URL: https://github.com/akinsanyajoseph/nft-card-componet
- Live Site URL: https://github.com/akinsanyajoseph/nft-card-componet

## My process
In approaching the challenge, I firstly wrote my HTML codes with the appropriate semantic tag to ensure accessibility compliance and functionality even if the CSS file (for any weird reason) doesn't work oe load.

Then I started with the base styles for my project - the body selector, heading, paragraph and color codes. Next was styling the classes and IDs I'd used in my markup, ensuring they looked as close to perfection as the template that was provided in the challenge.

Lastly, I worked on the hover states. 

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

Majortity of this project was pretty easy to accomplish except for the hover state of the image card where I had to display the view icon as well as background color with a degree of opacity. It was a bit challenging cos I wanted to solve the problem in the smartest way possible - with the least amount of CSS codes.

I googled various approaches (like all good developers do 😂) and drew inspiration from the various solutions I found and was able to solve the problem. Here's what my approached looked like for the overlay and hover state:

1. I created the overlay class that handled the color overlay when there's a mouse over the main image.

```css
.overlay {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    width: 100%;
    height: 100%;
    opacity: 0;
    background-color: hsl(178, 100%, 50%);
    border-radius: 20px;
}
```

2. Next I used this class to hide the view-icon in the normal state

```css
.overlay-icon {
    position: absolute;
    top: 40%;
    left: 40%;
    display: none;
}
```

3. Then I wrote this codes to ensure that when the mouse is over the image, the overlay and the view icon becomes visible

```css
.image-card:hover .overlay {
    opacity: 0.7;
}

.image-card:hover .overlay-icon {
    display: block;
}
```


### Continued development

The goal is to keep learning and getting better particularly with being efficient with how I approach solutions.

### Useful resources

- [How to create Overlay Effects](https://www.w3schools.com/howto/howto_css_image_overlay.asp) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.



## Author

- Website - [Akinsanya Joseph](https://akinsanyajoseph.com)
- Frontend Mentor - [@akinsanyajoseph](https://www.frontendmentor.io/profile/akinsanyajoseph)
- Twitter - [@akinsanyajoe](https://www.twitter.com/yakinsanyajoe)
