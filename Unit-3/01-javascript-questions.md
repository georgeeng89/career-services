# JavaScript Interview Questions

This document has 3 kinds of interview questions:

- Short answer questions that check for understanding, mostly of concepts
- Code analysis / evaluation, mostly checking for your debugging / language skills
- Whiteboard problems, require you to write code

To get the most out of this guide, "golf" some of these questions.  That is, figure out how to answer them correctly in the least number of steps.

## Resources

Before reading this doc, definitely check out these great resources!

- http://lucybain.com/blog/tags/interview-questions/
- http://www.toptal.com/javascript/interview-questions
- http://www.careerride.com/Object-oriented-programming-Interview-Questions.aspx
- https://medium.com/javascript-scene/10-interview-questions-every-javascript-developer-should-know-6fa6bdf5ad95
- http://blog.alinelerner.com/lessons-from-a-years-worth-of-hiring-data/
- https://sites.google.com/site/steveyegge2/five-essential-phone-screen-questions

## Short Answer (phone interview)

Classical Inheritance & OOP
>

NaN
>

Async and Callback Hell
>

Describe event bubbling.
>

Difference between document load event and document ready event?
>

Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?
>

Why would you use something like the load event? Does this event have disadvantages? Do you know any alternatives, and
>
 What is the extent of your experience with Promises and/or their polyfills?
 >

What are the pros and cons of using Promises instead of callbacks?
>

What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?
>

What tools and techniques do you use debugging JavaScript code?
>

What language constructions do you use for iterating over object properties and array items?
>

Explain the difference between mutable and immutable objects.
>

What is an example of an immutable object in JavaScript?
>

What are the pros and cons of immutability?
>

How can you achieve immutability in your own code?
>

Explain the difference between synchronous and asynchronous functions.
>

What is event loop?
>

What is the difference between call stack and task queue?
>


What are the data types in JavaScript?
>
* Boolean
* String
* Undefined
* Number
* Null
* Symbol
* Object

> Functions and Arrays are kinds of Objects.

What's the difference between `null` and `undefined`?
> Something with a value of `null` is empty, while something with the value of `undefined` hasn't been initialized.

What does the `this` keyword refer to in JavaScript?
    1. The first value passed to `call()` or `apply()`
    2. The value that was `bind()`ed to the function
    3. The calling object
    4. The global scope

How are errors usually handled in JavaScript?
> Try/Catch/Finally blocks for synchronous code.  `catch` methods for promises.

How does inheritance work in JavaScript?
> JavaScript has prototypal inheritance. Rather than a blueprint, objects are linked to other object instances via prototypes.

Name two programming paradigms.
> Common answers include procedural, functional, and object-oriented. May also say imperative/delcarative.

What's the difference between imperative programming and declarative programming?
> Imperative programming tells the computer what to do. Declarative programming tells the computer what you want, ignorant of the steps required to produce it.

What are some tenets of functional programming?
* Functional purity (no side-effects, output derived only from input)
* Simple functions
* First-class functions (functions as variables)
* Higher-order functions (functions that return functions)

What is immutability?
> When a stored value can't be changed. Functional programs/languages replace values with new values, rather than changing (or "mutating") the existing ones.

What is async in JavaScript?
> When a function does not immediately return a value. The rest of the program continues executing, requiring special handling and "callback functions" for when function calls complete.

What is the DOM?
> Document Object Model. It's the API for web pages, and what HTML gets parsed into.

Explain how the factory pattern works.
> A factory is when you need an object with a particular interface, but you let a constructor decide which specific object you get back.
```js
myEmployee = Employee.byType("fullTime");
// myEmployee is actually an instance of FullTimeEmployee
```

Name as many kinds of loops as you can.
> For, While, Do While, For-In, For-Each, Map, Reduce

Name as many different kinds of conditionals as you can.
> if/then/elseIf/else, switch, ternary.

What creates scope in Javascript?
> There's global scope and function scope in ES5.  In ES2015 there's also Block scope.

How can variables be assigned in Javascript in ES2015?
> `var` for function scope, `let` for block scope, `const` for block scope protected against reassignment.

What is a typical use case for anonymous functions?
>Callbacks, like in the .then of an AJAX call.

Name 2 or more ways to define a global variable in Javascript
>Leave off the `var` or assign it to the `window`

What does AJAX stand for?  Explain how it works in as much detail as possible
>Asynchronous javascript and xml, it just makes a request to a specific url with a verb and data (and callbacks). Then it makes the call with the appropriate headers.

What’s the difference between `==` and `===` in JS?
>Type Coercion

> == doesn't care about type (i.e. type coercion), so "2" == 2 will evaluate to true. === does care about type, so "2" === 2 will evaluate to false.

What is "callback hell" and how can it be avoided?
>_

What's the difference between Primitive and Reference types in Javascript?
>A primitive type has a fixed amount of memory that it takes up, where as a reference type does not. Examples of primitive types are boolean values or integers, where as examples of ref types would be arrays. ref types like arrays are made up of references to their values, hence the name

Explain event delegation
>

Explain how `this` works in JavaScript
>

Explain how prototypal inheritance works
>

What's the difference between a variable that is: null, undefined or undeclared?  How would you go about checking for these?
>An undefined value typically comes from a variable that has been declared, but was not assigned a value.
  ```js
  var a;
  ```

  A null value is a value that explicitly represents nothingness or a lack of a value.
  ```js
  var a = null;
  ```

  An undeclared variable will throw an error if used in code. Here, `c` is undeclared and will throw an error.
  ```js
  var a = 1;
  var c = a + b
  ```

What is a closure, and how/why would you use one?
> A closure is a function that maintains a reference to it's outer scope. These are useful in high-order functions.

What's a typical use case for anonymous functions?
> These are most commonly used in callbacks and IIFEs.

What's the difference between host objects and native objects?

What's the difference between .call and .apply?
> They both server the same purpose, but one accepts an array or arguments instead of a comma seperated list.

- Explain Function.prototype.bind.
> Bind works like call and apply, but instead of invoking the function it's applied to, it returns a new function with the bound context and arguments.

Explain AJAX in as much detail as possible.
>_

Explain how JSONP works (and how it's not really AJAX).
>_

Explain "hoisting".
>

Why is extending built-in JavaScript objects not a good idea?
>

What is the difference between == and ===?
>

Why is it called a Ternary expression, what does the word "Ternary" indicate?
>

What is "use strict";? what are the advantages and disadvantages to using it?
>

What is the difference between a host object and a native object?
>_

What tools can be used to assure consistent style?
> jsLint etc...

---------------------------------------------------------------------------------------------------

## Code Analysis

In Javascript, what’s the value of x: `var x = 10 + '20'`
>'1020'

What does the following JS code return:
```js
var a = [1,2,3]
var b = [1,2,3]
return a === b
```
>false

What does the following JS code return:
```js
var a = 1
var b = a
a = 2
return b
```

What is the result of running following JS code:

```js
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

What is the value of foo?
```js
var foo = 10 + '20';
```

How would you make this work?

```js
add(2, 5); // 7
add(2)(5); // 7
```

What value is returned from the following statement?
```js
"i'm a lasagna hog".split("").reverse().join("");
```

What is the value of `window.foo`?
```js
( window.foo || ( window.foo = "bar" ) );
```

What is the outcome of the two alerts below?
```js
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);
```

What is the value of foo.length?
```js
var foo = [];
foo.push(1);
foo.push(2);
```

What is the value of foo.x?
```js
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};
```

What does the following code print?
```js
console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```

Explain why the following doesn't work as an IIFE:
  - What needs to be changed to properly make it an IIFE?
```js
function foo(){ }();
```

Given a function `function Person(){}`, what's the difference between:
```js
var person = Person()
```

and

```js
var person = new Person()
```

1. What does this evaluate to - `2 + 3 + '7'`.

------------------------------------------------------------------------------------------------------------------------

## Whiteboard Problems

Make this work:
```js
duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]
```

Create a for loop that iterates up to 100 while outputting "fizz" at multiples of 3, "buzz" at multiples of 5 and - "fizzbuzz" at multiples of 3 and 5

Write a method to check if 2 given words are anagrams.

```js
anagram_checker("Dictionary", "Indicatory")
#=> true

anagram_checker("Dictionary", "blahblah")
#=> false
```

Write code to convert a numeric string like “543” and convert it to the integer version 543. Assume numbers will be whole integers.

Whiteboard the schema for zappos.com

Write FizzBuzz with as few if statements as possible. It's possible without any conditionals at all.

Implement a function which calculates the n-th item of Fibonacci sequence

Find largest prime palindrome less than 1000

Implement an algorithm to reverse a singly linked list

Count the number of nodes in a binary tree

Write your own getElementById function

Show an example of the following array methods - `push`, `pop`, `shift`, and `unshift`.
