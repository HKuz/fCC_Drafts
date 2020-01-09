# Catch Unclosed Parentheses,  Brackets, Braces and Quotes

## Challenge Description

Another syntax error to watch out for is that all opening parentheses, brackets, curly braces, and quotes have a closing pair. This tends to happen when you are editing existing code and inserting items with one of the pair types. Also, take care when you're nesting code blocks into others, such as adding a callback function as an argument to a method.

One way to avoid this mistake is as soon as you type the opening character, immediately type the closing match, then move your cursor back between them and continue coding. Fortunately, most modern code editors generate the second half of the pair automatically.

## Instructions

Fix the two unclosed pair errors so the code runs without issues.

## Challenge Seed

```js
"use strict"

let myArray = [1, 2, 3;
let addSeven = myArray.map((val => val + 7);
console.log(`addSeven array is: ${addSeven}`);
```

## Challenge Tests

```
assert(addSeven[0] === 8 && addSeven[1] === 9 && addSeven[2] === 10, 'message: Check the array and the <code>.map()</code> method for matching pairs. The console output should show that <code>addSeven</code> is <code>[8, 9, 10]</code>.');

assert(code.test(/3\s*?\]\s*?;/gi), 'message: The array should be enclosed with a matching set of brackets.');

assert(code.test(/val\s*?\)\s*?=>/gi), 'message: The <code>.map()</code> method's parameter should be enclosed with a matching set of parentheses.');
```

## Challenge Solution

```js
"use strict"

let myArray = [1, 2, 3];
let addSeven = myArray.map((val) => val + 7);
console.log(`addSeven array is: ${addSeven}`);
```
