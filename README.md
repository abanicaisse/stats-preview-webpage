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

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Screenshot

1. Desktop Design
   ![Stats Preview Card Desktop Design](https://user-images.githubusercontent.com/84383548/132560712-8bbf7eec-6fe9-42db-83df-87d288fe5873.png)

1. Mobile Design <br>
   ![Stats Preview Card Mobile Design](https://user-images.githubusercontent.com/84383548/132560820-a25a1d3e-13dc-4719-b31f-1975377a4d52.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My Process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

- CSS flexbox
- CSS grid
- CSS absolute and relative positioning
- CSS before and after Pseudo elements
- HTML5 Markup

Some HTML code from the project

```html
<main id="main">
    <div class="main__img">
      <img src="/images/image-header-desktop.jpg" alt="desktop header image" class="desktop-img">
      <img src="/images/image-header-mobile.jpg" alt="mobile header imgae" class="mobile-img">
    </div>
    <div class="main__stats">
      <h1>
        Get <span>insights</span> that help your business grow.
      </h1>
      <p>
        Discover the benefits of data analytics and make better decisions regarding revenue, customer
        experience, and overall efficiency.
      </p>
      <div class="stats__details">
        <p>10k+ <br> <span>companies</span></p>
        <p> 314 <br> <span>templates</span></p>
        <p> 12M+ <br> <span>queries</span></p>
      </div>
  </main>
```

Some CSS code from the project

```css
@media screen and (min-width: 1200px) {
  #main {
    grid-template-areas: "stats image";
    place-items: center;
    grid-template-columns: 1fr 1fr;
  }

  #main .main__img {
    height: 100%;
    grid-area: image;
  }

  #main .main__img::before {
    border-top-left-radius: 0;
    border-bottom-right-radius: 10px;
    border-top-right-radius: 10px;
  }

  #main .main__img img {
    width: 100%;
    height: 100%;
    border-top-left-radius: 0;
    border-bottom-right-radius: 10px;
    border-top-right-radius: 10px;
  }

  #main .main__img .mobile-img {
    position: absolute;
    display: none;
  }

  #main .main__img .desktop-img {
    position: static;
    display: block;
  }

  #main .main__stats {
    text-align: left;
    padding: 5rem 4rem;
    place-items: center;
  }

  #main .main__stats > h1 {
    font-size: 2.5rem;
    line-height: 1.3;
    padding: 0 0 2rem 0;
  }

  #main .main__stats > p {
    font-size: 1.5rem;
    padding-bottom: 4rem;
  }

  #main .main__stats > .stats__details {
    grid-template-columns: repeat(3, 1fr);
  }

  #footer {
    margin-top: 0;
  }
}
```

## Author

- Twitter - [@abanicaisse](https://www.twitter.com/abanicaisse)
- Frontend Mentor - [@abanicaisse](https://www.frontendmentor.io/profile/abanicaisse)
- CodePen - [My codepen](https://www.codepen.io/Nicaisse)
