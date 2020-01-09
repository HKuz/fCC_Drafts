# Catch Missing Open and Closing Parenthesis After a Function Call

## Challenge Description

When a function or method doesn't take any arguments, you may forget to include the (empty) opening and closing parentheses when you try to call it. Often times the result of a function call is saved in a variable for other use in your code. This error can be detected when you're logging variable values (or their types) to the console and see one is set to a function reference, instead of the expected value the function returns.

The variables in the following example are different:

```js
function myFunction() {
  return "You rock!";
}

let varOne = myFunction; // set to equal a function
let varTwo = myFunction(); // set to equal the string "You rock!"
```

## Instructions

Fix the code so `result` is set to the value returned from calling `getNine`.

## Challenge Seed

```js
"use strict"

function getNine() {
    let x = 6;
    let y = 3;
    return x + y;
}

let result = getNine;
console.log(result);
```

## Challenge Tests

```
assert(result == 9, 'message: Fix the code so the variable <code>result</code> is the number that the function <code>getNine</code> returns.');

assert(code.test(/getNine\(\);/gi), 'message: Make sure to call the <code>getNine</code> function.');
```

## Challenge Solution

```js
"use strict"

function getNine() {
    let x = 6;
    let y = 3;
    return x + y;
}

let result = getNine();
console.log(result);
```
