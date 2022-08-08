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

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- Mobile-first workflow
- Flexbox
- SASS


### What I learned

I practiced making a layout with flexbox, and learned how much easier it can make some projects while
minimizing the use of divs.

For example, instead of relying on overusing divs for every element and styling and spacing each one by hand.

```html
<div class='card'>
  <div class='img-container'>
    <img class='image' src='#' alt=''>
  </div>
  <div class='title-box'>
    <h1 class='primary-title'>Title here</h1>
    </div>
    <div class='secondary-title'>
      <h2 class='secondary-title'>Secondary title here</h2>
    </div>
  <div class='text-box'>
    <p class='some-text'>lorem ipsum</p>
    </div>
      <div class='text-box'>
    <p class='some-text'>lorem ipsum</p>
    </div>
</div>
```



You make it cleaner by removing a lot of the dependancies on divs
and using Flexbox to turn the elements into flex-items to help with layouts, and add spacing
to the container's children.

```html
<div class="card">
        <img class='display-img'src="assets/images/image-product-mobile.jpg" alt="A bottle of Gabrielle Essence Eau De Parfum">
        <div class="card-content"> 
            <h2 class="ff-accent fs-accent fw-regular category-heading">PERFUME</h2>
            <h1 class="ff-heading fs-primary-heading fw-bold text-neutral-800">Gabrielle Essence Eau De Parfum</h1>
            <p> A floral, solar and voluptuous interpretation composed by Olivier Polge, 
              Perfumer-Creator for the House of CHANEL.</p>

            <div class="price-container">
              <span class="ff-heading fs-primary-heading fw-bold text-primary-400 current-price">
                $149.99
              </span>
              <span class="previous-price">
                $169.99
              </span>
            </div>
            <button class="fs-accent fw-bold bg-accent-400 button"><img src="assets/images/icon-cart.svg" alt="cart svg">Add to Cart</button>
        </div>
    </div>
  ```

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


I also learned about more recent SASS features like @use and @forward.

For example instead of something like this

```css
@import 'abstract/variables';

```

It's better to use the following to prevent name-spacing conflicts.

```css
 @use '../abstract' as a;

```



## Author

- Website - [Add your name here](https://evanlittlejohn.com/)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/CodeSofty)

