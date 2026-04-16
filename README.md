# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

Set up steps: Create styles.css, link it in the head of the html, link the font in the head as well. Move the provided styles to styles.css and delete the style tag. Write the custom variables and the universal reset in styles.css.

Working on the HTML: Create a main element to hold the content, and give it the flex-container class in order to position the card. Create a div element for the card itself, and give it the flex-container class. Create 5 section.flex-container elements: hero section, prep, ingredients, instructions, and nutrition. Fill in the necessary elements and their respective content in each of the sections. Most of the h2 elements were given the subtitle class to use for styling, and the spans within several of the list items were given the task class for styling; most of the other elements were given classes to target them by as well but subtitle and task were more of utility classes.

Styling: Set overall styles for the body, set the broad flex-container rules, and set styles for the card. Then work down the card, styling elements from top to bottom. I had a little trouble figuring out how to organize my CSS with, for example with the subtitle class styles appearing more than once throughout the hierarchy. I ended up putting the subtitle styles before the more element-based styles, and then put the list styles and table styles at the end. I finished by adding margins and adjusting the padding throughout to try to get the spacing right, then did the media query for small screens.

### Built with

HTML and CSS (including flexbox); no CSS frameworks or JS

### What I learned

I learned about some of the unique behaviors of tables and their related elements; I had trouble getting the borders and padding to work on my table rows. After I looked it up I figured out I needed to set border-collapse: collapse; on the table itself in order for the border to work, and for the padding to work, I ended up just targeting the cells themselves as that seemed like the cleanest way to do it.

In addition to learning about tables, I also had to figure out how to make the hero image ignore its parent card's padding for the mobile layout. I ended up using negative margins on the top and sides to make it overlay the existing padding, and set its width using calc(). Even after that it still wasn't working correctly so I also used align-self, which I didn't know about previously, to make the image center aligned instead of flex-start aligned inside the card. I also had to use min-width instead of width.

### Continued development

In the future I would like to focus on building mobile-first instead of desktop-first like I have been doing. I'd also like to get a better understanding of how flexbox can sometimes "ignore" certain properties, such as width.

## Author

- Frontend Mentor - [@leven-carr](https://www.frontendmentor.io/profile/leven-carr)
- GitHub - [@leven-carr](https://github.com/leven-carr)
