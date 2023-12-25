# Frontend Mentor - FAQ accordion solution

This is a solution to the [FAQ accordion challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-wyfFdeBwBz). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- 



## Overview

### The challenge

Users should be able to:

- Hide/Show the answer to a question when the question is clicked
- Navigate the questions and hide/show answers using keyboard navigation alone
- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot


![Frontend Mentor - FAQ accordion](./screenshot.jpg)
![Frontend Mentor - FAQ accordion mobileview](./screenshot.jpg)


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Visit the Live Site](https://debbie-dot5.github.io/FAQ-accordion/)



### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Javascript
- Laptop-first workflow



### What I learned

In Html I learnt how to render a markup on the webpage

```html
  <div class="content-container">
            <div class="question"> What is Frontend Mentor, and how will it help me?</div>
            <div class="answer">Frontend Mentor offers realistic coding challenges to help developers improve their
                frontend coding skills with projects in HTML, CSS, and JavaScript. It's suitable for
                all levels and ideal for portfolio building.</div>
        </div>

```
I learnt how to add a toggle class(active) in css 
```css
.accordion .content-container .answer{
  color: #a097a1;
 padding-top: 10px;
 font-size: 16px;
 width: 100%;
 height: 0;
 overflow: hidden;
 transition: .5s;
}



.accordion .content-container.active .answer{
    height: 100px;
}

.accordion .content-container.active .question::after{
    content: url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" width="30" height="31" fill="none" viewBox="0 0 30 31"><path fill="%23301534" d="M15 3.313A12.187 12.187 0 1 0 27.188 15.5 12.2 12.2 0 0 0 15 3.312Zm4.688 13.124h-9.375a.938.938 0 0 1 0-1.875h9.374a.938.938 0 0 1 0 1.876Z"/></svg>');
}
```
I learnt for loop and ES6 features in javascript
```js
for(i = 0; i < accordion.length; i++){
 

    accordion[i].addEventListener('click', function() {
        this.classList.toggle('active');
    })

};
```



### Continued development

- The DOM
- ES6 features



### Useful resources

- [Free code camp](https://www.youtube.com/watch?v=5fb2aPlgoys) - This helped me learn how to manipulate the Document Object Model in javascript. I really liked this pattern and will use it going forward.



## Author

- Website - [UmohDebbie](https://github.com/Debbie-dot5/FAQ-accordion)
- Frontend Mentor - [@Debbie-dot5](https://www.frontendmentor.io/profile/Debbie-dot5)
- Twitter - [@Debbie35d](https://twitter.com/Debbie35d)

