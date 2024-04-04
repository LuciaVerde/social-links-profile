# Frontend Mentor - Social links profile solution

This is a solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ). 

## Table of contents
  - [The challenge](#the-challenge)
  - [Screenshots](#screenshots)
      - [Mobile screenshot](#mobile-screenshot)
      - [Desktop screenshot](#desktop-screenshot)
  - [Links](#links)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
  - [Author](#author)

### The challenge

This challenge is to create a social link profile where the user can see a hover status when hovering over the social links in the profile.

### Screenshots

#### Mobile screenshot
![](./screenshots/mobile%20screenshot.png)

#### Desktop screenshot
![](./screenshots/desktop%20screenshot.png)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

### Built with
- HTML 5 
- SASS
- Mobile-first workflow

### What I learned

In this challenge I had the opportunity to learn about the `inherit` keyword.

My task was to ensure that whenever I hovered over each list item, the background would shift to green, the text to black, and the cursor to a particular icon. 

I knew how to implement the changes for the `li` element upon hovering, but I was unsure how to extend these changes to the nested `a` element.

When hovering over a li element, the &:hover rule sets new properties for the background and text color, as well as the cursor.

Because within the `a` selector, both the color and cursor properties are set to inherit, the text color and cursor of the `li` element influence those of the nested `a` element upon hovering. This occurs as the `a` element naturally inherits the color and cursor properties of its parent `li` element.


```scss
li {
  list-style: none;
  background-color: $grey;
  padding-top: 0.8rem;
  padding-bottom: 0.8rem;
  width: 100%;
  text-align: center;
  border-radius: 0.5rem;
  color: $white;

  &:hover {
   background-color: $green;
   color: $off-black;
   cursor: url(/assets/images/handcursor.svg )10 10, auto;
  }

  a{
   text-decoration: none;
   color: inherit;
   cursor: inherit;
  }
}

```

### Useful resources

- [Inherit](https://developer.mozilla.org/en-US/docs/Web/CSS/inherit) - This helped me out understanding the inherit keyword. 

### Author

- GitHub - [Lucía Verde](https://github.com/LuciaVerde)
- Frontend Mentor - [@LuciaVerde](https://www.frontendmentor.io/profile/LuciaVerde)
- LinkedIn - [Lucía Verde](https://www.linkedin.com/in/luc%C3%ADa-verde-6bb9822b1/)
