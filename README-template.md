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
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

![Screenshot](/screenshot.png)

### Links

- Solution URL: [My Solution](https://your-solution-url.com)
- Live Site URL: [GitHub Pages](https://delanohendrix.github.io/Stats-Preview-Card-Component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

Although relatively small and simple, the aspect of changing the color of an image was the part I was stuck on the longest. I wanted to keep the image linked via the img tag and not through css, as well as retaining the ability to change the image in different resolutions.
By adding a class onto the img tag itself I was able to accomplish this.

```html
<picture class="business-image">
  <source media="(min-width:1440px)" srcset="images/image-header-desktop.jpg" />
  <img
    class="overlay"
    src="images/image-header-mobile.jpg"
    alt="Image of business women working in an office" />
</picture>
```

```css
picture {
  display: flex;
  background-color: var(--accent);
}
img {
  width: 100%;
}
img.overlay {
  mix-blend-mode: multiply;
}
```

### Useful resources

- [CSS Reference](https://cssreference.io/) - This site helped me by refreshing me on the usage of various css attributes and properties.
- [StackOverflow](https://stackoverflow.com/questions/43479968/how-can-i-add-an-image-overlaying-an-img-tag) - This StackOverflow post helped me figure out how to add the overlay onto the image.

## Author

- Frontend Mentor - [@delanohendrix](https://www.frontendmentor.io/profile/delanohendrix)
