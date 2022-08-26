# JavaScript

- See [here](https://github.com/mi-lee/js-interview-questions) for some JS interview questions and resources
- Questions below from https://github.com/nishant8BITS/101-JavaScript-Interview-Question
- Difference between undefined and not defined in JavaScript
- What will be the output of below code?

  ```js
  var y = 1;
  if (function f(){}) {
    y += typeof f;
  }
  console.log(y);
  ```

- What is drawback of creating true private in JavaScript?
- Write a mul function which will work properly when invoked as below syntax:

  ```js
  console.log(mul(2)(3)(4)); // output : 24
  console.log(mul(4)(3)(4)); // output : 48
  ```

- How to empty an array in JavaScript?
- How to check if an object is an array or not?
- What will be the output of below code?

  ```js
  var output = (function(x){
    delete x;
    return x;
  })(0);

  console.log(output);
  ```

- What will be the output of below code?

  ```js
  var x = 1;
  var output = (function(){
    delete x;
    return x;
  })();

  console.log(output);
  ```

- What will be the output of below code?

  ```js
  var x = { foo : 1};
  var output = (function(){
    delete x.foo;
    return x.foo;
  })();

  console.log(output);
  ```

- What will be the output of the below code?

  ```js
  var Employee = {
    company: 'xyz'
  }
  var emp1 = Object.create(Employee);
  delete emp1.company
  console.log(emp1.company);
  ```

- What is undefined x 1 in JavaScript?
- What will be the output of below code?

  ```js
  var trees = ["xyz", "xxxx", "test", "ryan", "apple"];
  delete trees[3];
  console.log(trees.length);
  ```

- What will be the output of below code?

  ```js
  var bar = true;
  console.log(bar + 0);
  console.log(bar + "xyz");
  console.log(bar + true);
  console.log(bar + false);
  ```

- What will be the output of below code?

  ```js
  var z = 1, y = z = typeof y;
  console.log(y);
  ```

- What will be the output of below code?

  ```js
  // NFE (Named Function Expression
  var foo = function bar() { return 12; };
  typeof bar();
  ```

- What is the difference between declaring a function in below format?

  ```js
  var foo = function() {
    // Some code
  };

  function bar() {
    // Some code
  };
  ```

- What will be the output of below code?

  ```js
  var salary = "1000$";

  (function () {
    console.log("Original salary was " + salary);

    var salary = "5000$";

    console.log("My New Salary " + salary);
  })();
  ```

- What is the instanceof operator in JavaScript?
- What would be the output of below code?

  ```js
  function foo() {
    return foo;
  }
  new foo() instanceof foo;
  ```

- How do we calculate the length of the associative array below?

  ```js
  var counterArray = {
    A : 3,
    B : 4
  };
  counterArray["C"] = 1;
  ```

- What is the difference between Function, Method and Constructor calls in JavaScript?
- Write a function that prints a 4x4 multiplication table. E.g.:

  ```
  1 2  3  4
  2 4  6  8
  3 6  9 12
  4 8 12 16
  ```

  - Adjust this function so it takes a parameter for dimension.

- Write a function that determines if a player has won a game of tic-tac-toe.

  - Inputs: Game State, Player sign (X or O)
  - Output: True if player has won, False otherwise

  ```js
  console.log(ticTacToe([
    [1,1,1],
    [0,1,0],
    [0,1,0],
  ], 1), 'should be true');

  console.log(ticTacToe([
    [0,1,1],
    [0,1,0],
    [0,1,0],
  ], 1), 'should be true');

  console.log(ticTacToe([
    [1,0,0],
    [0,1,0],
    [0,1,1],
  ], 1), 'should be true');

  console.log(ticTacToe([
    [1,0,1],
    [0,1,0],
    [1,1,0],
  ], 1), 'should be true');

  console.log(ticTacToe([
    [1,0,1],
    [0,1,0],
    [0,1,0],
  ], 1), 'should be false');
  ```

- You work for a games company that is planning to release a series of different card games (e.g. poker, blackjack, spades, hearts, rummy, etc).

  - You've been tasked with writing a reusable card game library that provides basic classes and functionality common to all (or most) card games.

  - Describe the classes, attributes, and methods that you would build into this library.
