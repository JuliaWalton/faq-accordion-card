# FAQ accordion card solution - Frontend Mentor

![Design preview for the FAQ accordion card coding challenge](./design/desktop-preview.jpg)

## Welcome! 👋

Thanks for checking out my solution of this challenge!

This is a solution to the [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## The challenge

Your challenge is to build out this FAQ accordion card and get it looking as close to the design as possible.

Your users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked

## Links

Live Site URL: [https://juliawalton.github.io/faq-accordion-card/](https://juliawalton.github.io/faq-accordion-card/)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

## What I learned

This project was a helpful practice in using JS to show and hide information via css classes in response to a click. I utilized a forEach high order array method to look through the question array twice. This allowed me to check if the current item in the collection was the one firing the click event and if not remove it's active state.

```js
questions.forEach((question) => {
  const btn = question.querySelector(".question-btn");
  btn.addEventListener("click", (e) => {
    questions.forEach((item) => {
      if (item !== question) {
        item.classList.remove("show-answer");
      }
    });
    question.classList.toggle("show-answer");
  });
});
```

## Author

- Website - [Julia's Portfolio](https://juliawalton.github.io/portfolio/)
- LinkedIn - [Julia Walton](https://www.linkedin.com/in/juliawalton/)
