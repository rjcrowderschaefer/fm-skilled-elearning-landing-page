# Frontend Mentor - Skilled e-learning landing page solution

This is a solution to the [Skilled e-learning landing page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/skilled-elearning-landing-page-S1ObDrZ8q). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout depending on their device's screen size: mobile (min-width 766px), tablet (min-width 767, max-width 1439px) and desktop (min-width 1440px)
- See hover states for interactive elements for tablet and desktop breakpoints

### Screenshot

![Mobile](https://i.imgur.com/7D0ydyA.png)
![Tablet](https://i.imgur.com/EcbLLYz.png)
![Desktop](https://i.imgur.com/AgnhDkd.png)
![Desktop - Header button hover state](https://i.imgur.com/SRHhU1S.png)
![Desktop - Aside button hover state](https://i.imgur.com/3vTN9E9.png)
![Desktop - Footer button hvoer state](https://i.imgur.com/O7hJABq.png)


### Links

- [GitHub Repo](https://github.com/rjcrowderschaefer/fm-skilled-elearning-landing-page)
- [Live Site URL](https://main--cozy-rolypoly-9c8a2d.netlify.app/)

## My process

I used a mobile first approach to develop this process, beginning with the mobile layout and expanding to the tablet and desktop layouts using a CSS media query and adjusting the CSS grid sizing. Where possible I used semantic HTML and was diligent on when and where I used classes versus ids throughout the development process. I made sure to include accessibility components like alt text with images.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

For this project, I focused primarily on how to best implement CSS grid for each breakpoint and ultimately adjusted the grid sizing for the tablet and desktop breakpoints compared to the mobile breakpoint. I also worked with flexbox and how to adjust element placement and sizing in conjunction with using relative and absolute positioning. 

To see how you can add code snippets, see below:

```html
 <div class="category">
          <svg
            class="animation"
            width="56"
            height="56"
            viewBox="0 0 56 56"
            xmlns="http://www.w3.org/2000/svg"
          >
            <defs>
              <linearGradient x1="50%" y1="0%" x2="50%" y2="100%" id="a">
                <stop stop-color="#FF6F48" offset="0%" />
                <stop stop-color="#F02AA6" offset="100%" />
              </linearGradient>
            </defs>
            <g fill="none" fill-rule="evenodd">
              <circle fill="url(#a)" cx="28" cy="28" r="28" />
              <path
                d="M33.97 20.678c.565-.498.893-1.21.906-1.962A2.706 2.706 0 0 0 32.16 16a2.794 2.794 0 0 0-1.66.603 2.825 2.825 0 0 0-.854 1.962 2.69 2.69 0 0 0 4.325 2.113Zm-8.752.453c0 .05-.05.05-.1.1v.05a6.308 6.308 0 0 0-2.919 1.41c-.503.473-.958.995-1.358 1.559-1.006 1.408 1.358 2.766 2.315 1.358 1.257-1.762 2.816-2.264 4.527-1.71a141.96 141.96 0 0 0-2.717 5.181c-1.107 2.163-3.47 3.874-5.786 2.566a1.402 1.402 0 1 0-1.508 2.364 6.826 6.826 0 0 0 8.704-1.66c.05 0 .153.05.2.05 1.5.624 2.907 1.454 4.177 2.466.603.502 1.66 3.065 2.263 4.376a1.392 1.392 0 0 0 2.113.452c.393-.382.476-.982.202-1.456-.705-1.456-1.862-4.427-2.818-5.135a31.566 31.566 0 0 0-2.364-1.762l.1-.1a16.972 16.972 0 0 0-1.006-.605c.856-1.609 1.711-3.168 2.616-4.728 2.11.667 4.415.19 6.087-1.258.517-.46.973-.984 1.358-1.56.956-1.257-.905-2.515-2.012-1.66a.709.709 0 0 0-.153.202 4.36 4.36 0 0 1-2.013 1.66c-.05.05-.1.05-.1.1h-.051a4.146 4.146 0 0 1-3.622-.452l.101-.101h.05a.383.383 0 0 0-.201-.1 9.292 9.292 0 0 0-.956-.554 7.258 7.258 0 0 0-5.134-1.056l.005.003Z"
                fill="#FFF"
                fill-rule="nonzero"
              />
            </g>
          </svg>
          <h4>Animation</h4>
          <p class="desc">
            Learn the latest animation techniques to create stunning motion
            design and captivate your audience.
          </p>
          <span class="get-started">Get Started</span>
        </div>
```
<!-- I set up a `category` class in order to apply styling to all of the category cards instead of styling one at a time -->

```css
    #pageAside {    
        display: flex;
        flex-direction: row;
        margin-bottom: 220px;
        position: relative;
    }
    
    .image-hero-mobile {
        display: none;
    }
    
    .image-hero-tablet {
        display: block;
        width: 641px;
        height: 640px;
        transform: scale(1.1);
        top: -120px;
        right: -270px;
        z-index: 1;
        position: absolute;
    }
    
    .aside-container-left {
        margin: 85px 330px 0 39px;
        height: auto;
        z-index: 2;
        width: 500px;
    }
```
<!-- For the tablet and desktop breakpoints, I adjusted the page aside to `flex-direction: row` and aligned the left div container with the h1, p and button elements with the img element on the right side. -->

## Author

- LinkedIn - [RJ Crowder-Schaefer](https://www.linkedin.com/in/rjcrowderschaefer/)
- Frontend Mentor - [@rjcrowderschaefer](https://www.frontendmentor.io/profile/rjcrowderschaefer)
- GitHub - [@rjcrowderschaefer](https://github.com/rjcrowderschaefer)
