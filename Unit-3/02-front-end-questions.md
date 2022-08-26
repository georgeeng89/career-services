# Frontend Questions

Everything related to CSS, build systems, HTML etc...

## Resources / sources

- http://www.toptal.com/html5/interview-questions
- http://www.skilledup.com/articles/html-html5-interview-questions-answers
- http://www.codeproject.com/Articles/702051/important-HTML-Interview-questions-with-answe
- http://www.sitepoint.com/10-typical-html-interview-exercises/
- http://career.guru99.com/top-50-html-interview-questions/
- http://www.geekinterview.com/Interview-Questions/Web/Html
- http://techpreparation.com/html-interview-questions-answers1.htm#.VlmapN8rLXE
- http://www.careerride.com/Interview-Questions-HTML.aspx

## Example Questions

Explain and contrast the usage of `event.preventDefault()` and `event.stopPropagation()`. Provide an example.
>_

What are data-attributes and why are they useful?
>They let you place information on a dom object so that you can easily recall it later in your code, or with some other dom interaction.

>Data attributes are part of HTML5. They let you store snippets of data in the DOM, for example if you want to store an ID with something but don't want it to appear visible on the page. Before HTML5, you had to store data in class or rel attributes, which sometimes caused problems.

What is minification?
>_

What is isomorphic JavaScript?
> JavaScript can that be run on both the client (in the browser) and in Node (on the server)

What's the difference between one-way and two-way binding?
> Two-way binding is when a UI input is bound to a model, and they are allowed to update each other directly. One-way binding, the model tells the input what to display (single source of truth) and is updated via events.

What does CSS Stand for and what does its name mean?
>Cascading Style Sheets. Refers to the inheritance of style rules from parent elements.

How is CSS Specificity calculated?
>Common answer: A running point total is tallied by from CSS selectors for a given rule. Different selectors are worth different amounts of points. Inline styles are 1000, IDs are 100, classes/attributes are 10, elements and pseudoselectors are 1

>True answer: It's implemented differently in different browsers. You're never supposed to be able to brute-force override a higher specificity, but you can in some browsers.

What is z-index in CSS?
>It's the z axis in a 3 dimensional system. Objects with a greater z index will appear to sit above of those with a lower z index.

Name 3 color systems in CSS
>RGBa, HSLa, HEX, HTML5

>RGBA, Hexadecimal, Keyword

Name 4 different media queries in CSS
>Device height, device aspect ratio, device width, orientation
How do you go about testing your JavaScript?

What's the difference between an "attribute" and a "property"?
>_

Explain the same-origin policy with regards to JavaScript.
>_

Explain what a single page app is and how to make one SEO-friendly.
>_

What does a doctype do?
>_

What's the difference between standards mode and quirks mode?
>_

What's the difference between HTML and XHTML?
>_

Are there any problems with serving pages as application/xhtml+xml?
>_

How do you serve a page with content in multiple languages?
>_

What kind of things must you be wary of when design or developing for multilingual sites?
>_

What are data- attributes good for?
>_

Consider HTML5 as an open web platform. What are the building blocks of HTML5?
>_

Describe the difference between a cookie, sessionStorage and localStorage.
>_

Describe the difference between `<script>`, `<script async>` and `<script defer>`.
>_

Why is it generally a good idea to position CSS `<link>`s between `<head></head>` and JS `<script>`s just before `</body>`? Do you know any exceptions?
>_

What is progressive rendering?
>_

Have you used different HTML templating languages before?
>_

What are some of the key new features in HTML5?
>_

What are “web workers”?
>_

How do you indicate the character set being used by an HTML5 document? How does this differ from older HTML standards?
>_

Discuss the differences between an HTML specification and a browser’s implementation thereof.
>_

Briefly describe the correct usage of the following HTML5 semantic elements: `<header>`, `<article>`, `<section>`, `<footer>`.
>_

Can a `<section>` contain `<article>` elements? Can an `<article>` contain `<section>` elements? Provide usage examples.
>_

Can a web page contain multiple `<header>` elements? What about `<footer>` elements?
>_

Describe the relationship between the `<header>` and `<h1>` tags in HTML5.
>_

Give a simple implementation of the `<video>` tag to embed a video stored at `http://www.example.com/amazing_video.mp4`. Give the video a width of 640 pixels by 360 pixels. Provide the user with controls.
>_

Write the code necessary to create a 300 pixel by 300 pixel `<canvas>`. Within it, paint a blue 100 pixel by 100 pixel square with the top-left corner of the square located 50 pixels from both the top and left edges of the canvas.
>_

What is HTML5 Web Storage? Explain localStorage and sessionStorage.
>_

What is HTML?
>_

What is the difference between HTML elements and tags?
>_

What is “Semantic HTML?”
>_

What does DOCTYPE mean?
>_

What’s the difference between standards mode and quirks mode?
>_

What are the limitations when serving XHTML pages?
>_

How many HTML tags are should be used for the most simple of web pages?
>_

How do you make comments without text being picked up by the browser?
>_

What is the difference between linking to an image, a website, and an email address?
>_

My hyperlink or image is not displaying correctly, what is wrong with it?
>_

What is the syntax difference between a bulleted list and numbered list?
>_

What is the difference between `<div>` and `<frame>`?
>_

What is the difference between the application model of HTML and HTML5?
>_

Ok, what’s the real difference between HTML and HTML5?
>_

What is the new DOCTYPE?
>_

What are some new HTML5 markup elements?
>_

What elements have disappeared?
>_

What are the new media-related elements in HTML5?
>_

What are the new image elements in HTML5?
>_

What is the difference between SVG and `<Canvas>`?
>_

What are data- attributes good for?
>_

What is the difference between HTML5 interaction in Sencha and Twitter/Bootstrap?
>_

Describe the difference between cookies, sessionStorage, and localStorage.
>_

What are some of the major new API’s that come standard with HTML5?
>_

What is the difference in caching between HTML5 and the old HTML?
>_

- What are some templating libraries.
- What's LESS?
- What do you think of AMD vs CommonJS?
- What's the difference between feature detection, feature inference, and using the UA string?
- Have you ever used JavaScript templating? If so, what libraries have you used?
- How do you handle internationalization?

### CSS Questions:

- What does FlexBox fix?
- What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
- What is the difference between classes and ID's in CSS?
- Describe Floats and how they work.
- Describe z-index and how stacking context is formed.
- Describe BFC(Block Formatting Context) and how it works.
- What are the various clearing techniques and which is appropriate for what context?
- Explain CSS sprites, and how you would implement them on a page or site.
- What are your favorite image replacement techniques and which do you use when?
- How would you approach fixing browser-specific styling issues?
- How do you serve your pages for feature-constrained browsers?
- What are the different ways to visually hide content (and make it available only for screen readers)?
- Have you ever used a grid system, and if so, what do you prefer?
- Have you used or implemented media queries or mobile specific layouts/CSS?
- Are you familiar with styling SVG?
- How do you optimize your webpages for print?
- What are some of the "gotchas" for writing efficient CSS?
- What are the advantages/disadvantages of using CSS preprocessors?
- Describe what you like and dislike about the CSS preprocessors you have used.
- How would you implement a web design comp that uses non-standard fonts?
- Explain how a browser determines what elements match a CSS selector.
- Describe pseudo-elements and discuss what they are used for.
- Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
- What does * { box-sizing: border-box; } do? What are its advantages?
- List as many values for the display property that you can remember.
- What's the difference between inline and inline-block?
- What's the difference between a relative, fixed, absolute and statically positioned element?
- The 'C' in CSS stands for Cascading. How is priority determined in assigning styles (a few examples)? How can you use this system to your advantage?
- What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
- Have you played around with the new CSS Flexbox or Grid specs?
- How is responsive design different from adaptive design?
- Have you ever worked with retina graphics? If so, when and what techniques did you use?
- Is there any reason you'd want to use translate() instead of absolute positioning, or vice-versa? And why?

Questions from https://github.com/developerquestions/css-questions
- What are the pros and cons of using absolute positioning?
- What is the difference between display: inline; and display: inline-block;?

Questions from https://github.com/bargitta/cssInterview
- What is the box model? Draw it out and explain the different elements.
- Where to define styles?
- List CSS selectors and their priorities
- The difference between block element, inline-block element and inline element
- Talk about position property, and its values
- How to hide an element?
- What is float element?
- What is pseudo element? what is pseudo class?
- How to center align a paragraph?
- How to center align a div inside another div?
- How to make a two column Web page? a three column Web page?
- How to draw a triangle? a circle? a colored square?
- How to make a tab view?

Questions from https://css-tricks.com/interview-questions-css/
- Using CSS properties alone, recreate this button:
  ![CSS Button](./css-button.png)
- Describe what a “reset” CSS file does and how it’s useful. Are you familiar with normalize.css? If so, how do they differ?
- What are the various techniques for clearing floats?
- What are sprites and why would use them? How do you go about creating them? What are possible alternatives to sprites?
- What are some accessibility concerns that come up in CSS?
- What tools do you use for cross-browser testing?
- Say you found a rendering problem on one of your sites in Internet Explorer 8, which you have decided you are supporting. How would you approach fixing it?
- What is responsive design all about?
- Have you ever worked with a grid layout? What are your thoughts on that?
- What are the benefits of SVG?
- Say you were tasked with coding a design that used non-standard web fonts, how would you go about it?

Questions from http://www.skilledup.com/articles/25-css-interview-questions-answers
- Explain what a class selector is and how it’s used
- What are pseudo classes and what are they used for?
- Explain the three main ways to apply CSS styles to a Web page
- What is grouping and what is it used for?
- What is an ID selector and how is it used?
- What is a Class selector and how does it differ from an ID selector?
- What are child selectors?
- What are the different CSS properties used to change dimensions and what values can they accept?
- How is the float property implemented in CSS?
- How to restore the default property value using CSS?
- What is the purpose of pseudo-elements and how are  they made?
- What is the purpose of the z-index and how is it used?
- What are the advantages and disadvantages of External Style Sheets?
- Explain the difference between visibility:hidden and display:none
- What are some of the new features and properties in CSS3?
- Why shouldn’t I use fixed sized fonts?
- Which font names are available on all platforms?
- What are the advantages/disadvantages of using CSS preprocessors? (SASS, Compass, Stylus, LESS)
- Why and how are shorthand properties used? Give examples.

### jQuery

- What is $(document).ready() function? Why should you use it?
- How do you retrieve attribute of an HTML tag using jQuery e.g. href of links?
- What’s the deal with the $ in jQuery? What is it and what does it mean?
- How can jQuery be used in conjunction with another JavaScript library that also uses $ for naming?
- What is method chaining in jQuery? Provide an example. What advantages does it offer?
- What is the difference between jQuery.get() and jQuery.ajax()?
- What selector would I use to query for all elements with an ID that ends with a particular string? Also, how would I modify the selector to retrieve only `<div>` elements whose IDs end with that same string? Provide an example.
- What is accomplished by returning `false` from (a) a jQuery event handler, (b) a regular JavaScript onclick event handler for an anchor tag, and (c) a regular JavaScript onclick event handler for a non-anchor tag (e.g., a div, button, etc.)?
- What is the proper way in jQuery to remove an element from the DOM before its Promise is resolved?
- Explain the difference between the `.detach()` and `.remove()` methods in jQuery.
- What are some problems with jQuery?

jQuery provides a useful `.clone()` method to create a deep copy of matching elements. Answer the following questions:
1. What is meant by a “deep copy”?
2. What is normally not included in the cloned copy? How can some of this behavior be controlled?
3. What is a potential “gotcha” when using the `.clone()` method? (HINT: What is an element attribute that you would generally not want to clone?)

## Code analysis / quiz

Order the following CSS selectors by specificity
```css
p {}
#special {}
.selected {}
div p {}
.red .green .blah {}
```

Consider the code snippet below. If there are 5 `<div>` elements on the page, what will be the difference between the start and end times displayed?
```js
function getMinsSecs() {
  var dt = new Date();
  return dt.getMinutes()+":"+dt.getSeconds();
}

$( "input" ).on( "click", function() {
  $( "p" ).append( "Start time: " + getMinsSecs() + "<br />" );
  $( "div" ).each(function( i ) {
    $( this ).fadeOut( 1000 * ( i * 2 ) );
  });
  $( "div" ).promise().done(function() {
    $( "p" ).append( "End time: " + getMinsSecs() + "<br />" );
  });
});
```

- Explain what the following code does:
```js
$( "div" ).css( "width", "300px" ).add( "p" ).css( "background-color", "blue" );
```

Which of the two lines of code below is more efficient? Explain your answer.
```js
document.getElementById( "logo" );
```
or
```js
$( "#logo" );
```

## Code Challenges

Write code in jQuery to animate the `#expander` div, expanding it from 100 x 100 pixels to 200 x 200 pixels over the course of three seconds.

Build an HTML page with a circle that is centered both horizontally and vertically, using only CSS.

Following questions taken from http://www.toptal.com/jquery/interview-questions

Explain what the following code will do:
```js
$( "div#first, div.first, ol#items > [name$='first']" )
```

The code below is for an application that requires defining a click handler for all buttons on the page, including those buttons that may be added later dynamically. What is wrong with this code, and how can it be fixed to work properly even with buttons that are added later dynamically?
```js
// define the click handler for all buttons
$( "button" ).bind( "click", function() {
    alert( "Button Clicked!" )
});

/* ... some time later ... */

// dynamically add another button to the page
$( "html" ).append( "<button>Click Alert!</button>" );
```

Explain to me what's going on in this CSS selector:

```css
[role=navigation] > ul a:not([href^=mailto]) {

}
```

Write a function that validates a form entry.

Select an element on the page and change the font size with vanilla JavaScript.
