# Pseudo-Code

References:

* http://www.careercup.com/page?pid=software-engineer-developer-interview-questions&topic=algorithm-interview-questions

## Create options

Write an algorithm to generate all possible combinations of a product code
based on all available product options. Each possible option value has a
code/slug that make up the product code. For example, shoes:

* style: 001, 002, 003, etc...
* color: red, blue, white, etc...
* size: 7,8,9,10,etc...
* gender: m,f

number of options and possible values for each option have to be flexible, though pretty finite.

## Remove Duplicates

Write a function to remove the duplicated characters from a string,
and maintain the order of the characters.

ex. `abracadabra` becomes `abrcd`

## Reverse a string

Write a function to reverse a string.

* pretend there's no built-in reverse method
* you do have `string#length` and you can access substrings

## Starry Numbers

In a programming language or pseudo code of your choosing, solve the following (evolving) problem.

1. Create a method to print the numbers 1-10 to the command line (one per line).
1. Print an asterisk after each even number.
1. Exclude numbers passed in as a single array from the output. (i.e. if a value is in the passed in array, don’t print it)
1. Now make the output look like this (assuming the exclude array contains [4, 6, 7]):

```
1
1 2*
1 2* 3
1 2* 3 5
1 2* 3 5 8*
1 2* 3 5 8* 9
1 2* 3 5 8* 9 10*
```

## Anagram

Given two arrays, write a method that returns true if it's an anagram.

## Reverse words

Given an array of characters which form a sentence of words, give an efficient algorithm to reverse the order of the words (not characters) in it.

## Substring removal

Given two strings S1 and S2 return a string that is S2 with all characters in S1 removed.

## Integers in a file

Write a function that sums up integers from a text file, one int per line.

## Odd numbers

Write function to print the odd numbers from 1 to 99.

Pretend you don't have `odd?` in this language.

## Largest number

Find the largest int value in an int array.
