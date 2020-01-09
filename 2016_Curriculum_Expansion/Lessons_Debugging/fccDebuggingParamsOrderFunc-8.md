# Catch Arguments that are Passed in the Wrong Order when Calling a Function

## Challenge Description

Continuing our discussion on calling functions, the next bug to watch out for is when a function's arguments are supplied in the incorrect order. If the arguments are different types, such as a function expecting an array and an integer, this will likely throw a runtime error. If the arguments are the same type (all integers, for example), then the logic of the code won't make sense. Make sure to supply all required arguments, in the proper order to avoid these issues.

## Instructions

The following function `positivePowers` raises a base to a positive exponent. Unfortunately, it's not called properly - fix the code so the value of `test` is the expected 8.

## Challenge Seed

```js
"use strict"

function positivePowers(b, e) {
    let result = 1;
    if (e <= 0) return result;
    for (let i = 1; i <= e; i++) {
        result *= b;
    }
    return result;
}

let base = 2;
let exp = 3;
let test = positivePowers(exp, base);
console.log(test);
```

## Challenge Tests

```
assert(test == 8, 'message: Fix the code so the variable <code>text</code> equals 2 raised to the 3rd power, not 3 raised to the 2nd power.');

assert(code.test(/positivePowers\(\s*?base,\s*?exp\s*?\);/gi), 'message: Make sure the arguments for the <code>positivePowers</code> function call are in the right order.');
```

## Challenge Solution

```js
"use strict"

function positivePowers(b, e) {
    let result = 1;
    if (e <= 0) return result;
    for (let i = 1; i <= e; i++) {
        result *= b;
    }
    return result;
}

let base = 2;
let exp = 3;
let test = positivePowers(base, exp);
console.log(test);
```
