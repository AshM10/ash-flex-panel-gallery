# ash-flex-panel-gallery

This is a solution to the [flex panels image gallery on #JavaScript30](https://javascript30.com). 30 day vanilla JS coding challenge.

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

- See panels side by side.
- See transition when panels are clicked. 

### Screenshot

![Screen Shot 2022-09-20 at 1 35 48 PM](https://user-images.githubusercontent.com/89284873/191337510-f45eab7b-0ffa-463c-8e64-f3460361841c.png)
![Screen Shot 2022-09-20 at 1 35 56 PM](https://user-images.githubusercontent.com/89284873/191337520-2c5a5d0d-2768-464e-8830-257b35758277.png)

### Links

- Solution URL: [GitHub](https://github.com/AshM10/ash-flex-panel-gallery)
- Live Site URL: [Netlify](https://ash-flex-panel.netlify.app)

## My process

### Built with

- Flexbox
- CSS Transitions
- Vanilla JavaScript

### What I learned

- CSS flex: 1. each of them will evenly distribute the space between the panels.
- An element in CSS can be both a flex item as well as a flex container. 
- You can nest a flexbox as much as you want.

To see how you can add code snippets, see below:

```css
  .panel > *:first-child {
        transform: translateY(-100%);
      }
      .panel.open-active > *:first-child {
        transform: translateY(0);
      }
      .panel > *:last-child {
        transform: translateY(100%);
      }
      .panel.open-active > *:last-child {
        transform: translateY(0);
      }
 ```

```js
 panels.forEach((panel) => panel.addEventListener("click", toggleOpen));
      panels.forEach((panel) =>
        panel.addEventListener("transitionend", toggleActive)
      );
```

### Continued development

Continue with Challenge #6.

### Useful resources

- [What the Flexbox?!](https://flexbox.io) - A simple, free 20 video course that will help you master CSS Flexbox!

## Author

- Website - [Ash Moreno](https://www.ashmoreno.dev)
- Twitter - [@sexy_gravy](https://twitter.com/sexy_gravy)
