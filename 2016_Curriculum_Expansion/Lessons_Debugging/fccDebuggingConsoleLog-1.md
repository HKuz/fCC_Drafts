# Use console.log to Check the Value of a Variable

## Challenge Description

Both Chrome and Firefox have excellent JavaScript consoles, also known as DevTools, for debugging your JavaScript.

You can find Developer tools in your Chrome's menu or Web Console in FireFox's menu. If you're using a different browser, or a mobile phone, we strongly recommend switching to desktop Firefox or Chrome.

--NEW TEXT, INSTRUCTIONS, AND TEST BELOW HERE

The console.log() method, which "prints" the output of what's within its parentheses to the console, will likely be your most helpful debugging tool. Placing it at strategic points in your code can show you the intermediate values of variables. It's good practice to have an idea of what the output should be before looking at what it is. Having check points to see the status of your calculations throughout your code will help narrow down where the problem is.

Here's an example to print 'Hello world!' to the console:

```js
console.log('Hello world!')
```

## Instructions (NEW)

Use the `console.log()` method to print the value of the variable `a` where noted in the code.

## Challenge Seed

```js
"use strict"

let a = 5;
let b = 1;
a++;
// Use console.log() below this line to check the value of a, it should output 6


let sumAB = a + b;
console.log(sumAB);
```

## Challenge Tests

```
assert(code.test(/console\.log\(a\)/gi)), 'message: Use <code>console.log()</code> to check the value of the variable <code>a</code>.');
```

## Challenge Solution

```js
"use strict"

let a = 5;
let b = 1;
a++;
// Use console.log() to check the value of a, it should output 6
console.log(a);

let sumAB = a + b;
console.log(sumAB);
```
