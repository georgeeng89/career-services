# Algorithms

## Suggested Process

1. Ask question and set up problem
1. Clarify any questions the interviewee has
1. Interviewee writes an answer in code or psuedocode
1. Give interviewee a chance to clarify anything you notice wrong or odd

## Questions and Answers

### Reverse a String

#### Question

Given a string,
  return the string reversed
  without using a builtin reverse function.

#### Tips

* `'hello'` -> `'olleh'`
* `String.split` and `Array.join`.

#### Answer

```js
function reverse (input) {
  var output = '';
  for (var i=input.length-1; i>=0; i--) {
    output += input[i];
  }
  return output;
}
```

```js
function reverse (input) {
  return input.split('').reduce(function (r, v) {
    return r.unshift(v);
  }, []).join();
}
```

### Anagrams

#### Question

Given 2 strings,
  return `true` if the 2 strings are
  anagrams of each other and `false` otherwise
  while ignoring spaces, punctuation, and case.

#### Tips

* An anagram is a word or phrase that is comprised of the same letters of another word or phrase.
* `'Debit Card'`, `'Bad Credit'` => `true`
* `'Dormitory'`, `'Dirty Room'` => `true`

#### Answers

```js
function anagram (input1, input2) {
  var sanitized1 = input1.replace(/\W/gi, '').toLowerCase();
	var sanitized2 = input2.replace(/\W/gi, '').toLowerCase();
	sanitized1 = sanitized1.split('').sort().join('');
	sanitized2 = sanitized2.split('').sort().join('');
	return sanitized1 === sanitized2;
}
```

### Palindrome

#### Question

Given a string
  return `true` if it is a palindrome and `false` otherwise
  while ignoring spaces, punctuation, and case.

#### Tips

* A palindrome is a word or phrase that has the same order of letters forwards and backwards.
* `'Never odd or even'` => `true`
* `'racecar'` => `true`
* `'Was it a car or a cat I saw?'` => `true`

#### Answer

```js
function palindrome (input) {
  var sanitized = input.replace(/\W/gi, '').toLowerCase();
	for (var i=0; i<sanitized.length; i++) {
		if (sanitized[i] !== sanitized[sanitized.length-i-1]) {
			return false;
		}
	}
	return true;
}
```

```js
function palindrome (input) {
  var sanitized = input.replace(/\W/gi, '').toLowerCase();
	var reversed = sanitized.split('').reverse().join('');
	return sanitized == reversed;
}
```

### Largest Number in an Array

#### Question

Given an Array of numbers,
  return the largest value of the Array.

#### Tips

* `Math.max`
* `Function.apply`

#### Answers

```js
function maxNumber (array) {
  return Math.max.apply(null, array);
}
```

```js
function maxNumber (array) {
  var max = Number.NEGATIVE_INFINITY;
  for (var i=0; i<array.length; i++) {
    if (max < array[i]) {
      max = array[i];
    }
  }
  return max;
}
```

### Linked List: Deletion

#### Question

Given a singly linked list,
  delete a node at a given index from the linked list.

#### Tips

* Keep a reference to the node's parent.

#### Answer

*Whiteboard Acceptable*

1. Iterate over the linked list keeping track of `currentNode` and `previousNode`
1. When you find the node, do `previousNode.next = currentNode.next`

<!--
### Linked List: Cycle

#### Question

Given a Linked List,
  determine if it contains a cycle.

#### Tips

* A cycle is anytime a `Node.next` points to a previous `Node` in the list.

#### Answer

*Whiteboard Acceptable*

1. Iterate over the linked list.
1. Everytime
-->

### Queue of Two Stacks

#### Question

Create a Queue using 2 Stacks.

#### Tips

* A Queue has 2 functions: `queue` and `dequeue`.
* A Queue is FIFO.
* A Stack has 2 functions: `push` and `pop`.
* A Stack is LIFO.

#### Answer

*Whiteboarding Acceptable*

1. Create a Queue class with 2 Stacks in it.
1. `queue` pushes items onto Stack1.
1. When you want to `dequeue`:
  1. `pop` all items from Stack1 onto Stack2
  1. `pop` and return 1 item from Stack2
  1. `pop` all items from Stack2 back onto Stack1

### Binary Tree Max Depth

#### Question

Given a Binary Tree
  return the greatest length from root to a leaf.

#### Tips

* A Tree traversal algorithm such as depth-first-search.

#### Answer

*Whiteboarding Accepteable*

```js
function greatestDepth (root) {
  var maxDepth = 0;
  function dfs (node, depth) {
    if (!node) {
      return;
    }
    if (depth > maxDepth) {
      maxDepth = depth;
    }
    dfs(node.left, depth + 1);
    dfs(node.right, depth + 1);
  }
  dfs(root, 0);
  return maxDepth;
}
```

### Determine if a Number is Prime

#### Question

Given a Number
  return `true` if it is prime and `false` otherwise.

#### Tips

* A prime is any whole number only divisible by itself and 1.

#### Answer

```js
function isPrime (input) {
  for (var i=2; i<input; i++) {
    if (input % i === 0) {
      return false;
    }
  }
  return true;
}
```

### Print all Possible Arrangements of Parenthesis

#### Question

Given a whole number `n`,
  return an array of all permutations of `n` sets of parenthesis.

#### Tips

* The parenthesis have to be properly opened and closed.
* `3` => `['((()))', '(()())', '(())()', '()(())', '()()()']`
* A tree data type can be used

#### Answer

*Whiteboarding Accepted*
```js
//INCOMPLETE
function permutateParens (n) {
  var combinations = [];
  function dfs (combination, opened, closed) {
    while (opened < n) {
      dfs(combination + '(', opened + 1, closed);
    }
    if (closed < opened) {
      dfs(combination + ')', opened, closed + 1);
    }
  }
  dfs('', 0);
  return combinations;
}
```
