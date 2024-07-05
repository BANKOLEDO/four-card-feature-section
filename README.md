# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the site depending on their device's screen size


For this challenge, I built an elegant and functional four-card feature section featuring:
- A visually appealing header
- Four distinct feature cards
- A responsive design that looks great on both desktop and mobile devices

### Screenshot
Desktop View

![](./images/Screenshot%20(144).png)

Mobile View
![](./images/four%20card%20mobile%20view.png)


### Links

- Solution URL: [My Solution](https://github.com/BANKOLEDO/four-card-feature-section)
- Live Site URL: [Page Preview](https://bankoledo.github.io/four-card-feature-section/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow

### What I learned

## Key Learnings

 1. CSS Grid Layout
I used CSS Grid to create a flexible and responsive layout, ensuring the design adapts seamlessly across various screen sizes.
```css
.entire-page {
    min-width: 100vw;
    min-height: 100vh;
    display: grid;
    grid-template-rows: repeat(2, 1fr);
    justify-content: center;
    background-color:  var(--very-light-gray);
    row-gap: 1rem;
}

@media (min-width: 950px) {
    .entire-page {
        grid-template-rows: unset;
        grid-template-areas: 
            ".    head .   "
            "a   b    c   ";
        column-gap: 20px;
    }
}
```

2. Typography and Font Styling
I incorporated Google Fonts for a clean and modern look, applying different font weights and styles to create visual hierarchy and improve readability.
```css
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600;700;800;900&display=swap');

.first-heading {
    font-family: 'Poppins', sans-serif;
    font-size: 1.6rem;
    font-weight: 500;
    color: var(--grayish-blue);
}
```

3. CSS Variables
I defined CSS variables to maintain a consistent color palette, streamlining the process of applying and managing colors across the entire stylesheet.
```css
:root {
    /* Primary Colors */
    --red: hsl(0, 78%, 62%);
    --cyan: hsl(180, 62%, 55%);
    --orange: hsl(34, 97%, 64%);
    --blue: hsl(212, 86%, 64%);
    /* Neutral Colors */
    --very-dark-blue: hsl(234, 12%, 34%);
    --grayish-blue: hsl(229, 6%, 66%);
    --very-light-gray: hsl(0, 0%, 98%);
}
```

4. Responsive Design
I utilized media queries to ensure the page is responsive and visually appealing on all devices.
```css
@media (min-width: 950px) {
    .entire-page {
        grid-template-rows: unset;
        grid-template-areas: 
            ".    head .   "
            "a   b    c   ";
        column-gap: 20px;
    }
}
```

## Author

- GitHub - [Bankole David](https://github.com/BANKOLEDO)
- Frontend Mentor - [@BANKOLEDO](https://www.frontendmentor.io/profile/BANKOLEDO)
- Twitter - [@bankydavid12](https://www.twitter.com/bankydavid12)
