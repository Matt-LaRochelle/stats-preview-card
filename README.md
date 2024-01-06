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
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![](./images/screenshot.png)

### Links

- Solution URL: [GitHub Pages Live Site (Solution)](https://matt-larochelle.github.io/stats-preview-card/)

## My process

### Built with

- I started by writing up the HTML in as basic a manner as possible, but eventually decided I needed an extra div in the main section in order to center things properly.
- CSS custom properties
- Desktop-first workflow
- Google Fonts


### What I learned

The main challenge for me was to get a purple filter overlay on the image. I couldn't make this work on the img element, so I decided to use a div and use the image as a background. This works pretty well, BUT now there is no alt text for the image, which bothers me. If anyone has any ideas for a solution to this, please let me know!

```css
.image {
    background-color: rgba(127, 0, 159, 0.5);
    color: #fff;
    height: 500px;
    width: 100%;
    position: relative;
    margin-bottom: 4rem;
}
.image::before {
    content: '';
    background: url('./images/image-header-desktop.jpg') no-repeat center center/cover;
    height: 100%;
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
}
```

### Continued development

I feel that my code is not organized well, and it is a bit overwhelming to look at for such a simple component. I would like to work on organizing my CSS.

Every time I have to use the ::before or ::after pseudo elements I always struggle with this concept as well. I need to work on this more so that I can write it more fluently.

## Author

- Website - [Matt's Dev Projects](https://mattsdevprojects.com/)
