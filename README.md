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
- [Author](#author)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./assets/images/desktop-view-screenshot.png)
![](./assets/images/mobile-view-screenshot.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://preview-product-card.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- Mobile-first workflow
- Flexbox
- SASS


### What I learned

I took on this challenge to practice more with flexbox and SASS.

- I got more comfortable with how to work with parent-child flexbox relationships

For example, this makes it much easier to target a parent's children with the parent > * selector
and then apply styles to a flex parent's children.

```css
.card-content {
    display: flex;
    flex-direction: column;
    padding: $card-padding;

    & > * {
        padding: $tb-padding-smll
    }
}
```


- I learned about more recent SASS features like @use and @forward.

For example instead of something like this

```css
@import 'abstract/variables';

```

It's better to use the following to prevent name-spacing conflicts.

```css
 @use '../abstract' as a;

```
or

```css
 @use '../abstract' as *; 
```


## Author

- Website - [Portflio](https://evanlittlejohn.com/)
- Frontend Mentor - [@CodeSofty](https://www.frontendmentor.io/profile/CodeSofty)

