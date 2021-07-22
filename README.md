# Frontend Mentor - FAQ accordion card solution

This is a solution to the [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#Learning)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked


## My process
  The accordion menu is pretty straight foward. With target selector we can do nice tricks and for this challenge it was enough, dismissing the necessity of JS.
  The most challenging part was to position the images out of the layout flow, but once I undestood how each property works everything came together.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### Learning
  The position absolute can be really messy, because the element goes out of the flow, but when it is combine with position relative, in the parent, it gives you more control of where the element child will be, in this case relatively to the parent.
  The z-index was crucial to this project. It enabled the little box image shows over everything, even with some other images that naturally would come over it. 
```css
.card {
  position: relative;
   
    
}

.img-box {
    position: absolute;
    max-width: 25%;
    left: 0%;
    transform: translate(2.3rem,-2rem);
    z-index: 1;
}
```

### Continued development

  Positioning images, espeacilly out of the flow, is really challenging and can be a problem when it comes to responsive designs. With that in mind, I'll keep practicing layout that requires this kind of knowledge to master this ability.


### Useful resources

- [Example resource 1](https://www.youtube.com/watch?v=MXrtXg1kpVs&t=1280s) - This helped me with the target selector to code the accordion. 
- [Example resource 2](https://www.w3schools.com/cssref/sel_target.asp) - This is an amazing article which helped me fully understand target selector. I'd recommend it to anyone still learning this concept.

