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
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

#### Mobile Solution
![](./Mobile-Solution.png)


#### Desktop Solution
![](./Desktop-Solution.png)


### Links

- Solution URL: [Solution](https://www.frontendmentor.io/solutions/frontend-mentor-stats-preview-card-component-solution-ey6p47DGf)
- Live Site URL: [Live Site](https://frontend-mentor-stats-preview-card-component-gamma.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

How to create a simple overlay background over an image.

```html
  <section class="card-image-container">
    <img id="card-image" src="images/image-header-mobile.jpg" alt="">
  </section>
```
```css
.card-image-container {
    /* height: 100%; */
    width: 100%;
    background-color: var(--accent);
    border-radius: 10px 10px 0 0;
}

#card-image {
    height: 100%;
    width: 100%;
    opacity: 0.5;
    border-radius: 10px 10px 0 0;

}
```


Update: Thanks to [@brasspetals](https://www.frontendmentor.io/profile/brasspetals) I discovered out a more elegant way to achieve the background color overlay on the background image:

```html
  <div id="card-image"></div>
```
```css
  #card-image {
      flex: 0 0 240px;
      width: 100%;

      border-radius: 10px 10px 0 0;

      background-blend-mode: multiply;
      background-color: var(--accent);
      background-image: url(/images/image-header-mobile.jpg);
      background-size: cover;
  }
```
## Author

- Website - David Shanahan (https://vulnerable.computer)
- Frontend Mentor - [@ds0-sec](https://www.frontendmentor.io/profile/ds0-sec)
- Twitter - [@0ds01](https://twitter.com/0ds01)
