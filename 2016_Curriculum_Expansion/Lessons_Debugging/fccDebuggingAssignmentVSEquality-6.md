# Catch Use of Assignment operator Instead of Equality Operator (= VS == and ===)

## Challenge Description

Branching programs, aka ones that do different things if certain conditions are met, rely on `if`, `else if`, and `else` statements in JavaScript. The condition sometimes takes the form of testing whether a result is equal to a value. How we speak this logic (in English, at least) is "if x equals y, then ..." which can literally translate into code using the `=`, or assignment operator, and unexpected control flow in your program.

As you know, the assignment operator (`=`) in JavaScript assigns a value to a variable name. And the `==` and `===` operators check for equality (the triple `===` tests for strict equality, meaning both value and type are the same). The code below assigns `x` to be 2, which evaluates as true. Almost every value on its own in JavaScript evaluates to true, except the "falsy" values of false, 0, "" (an empty string), NaN, undefined, and null.

```js
let x = 1;
let y = 2;

if (x = y) {
  // this will run for any value of y (except for a falsy)
} else {
  // this is what should run (but won't) in this example
}
```

## Instructions

Fix the condition so the program runs the right branch, and the appropriate value is assigned to `result`.

## Challenge Seed

```js
"use strict"

let x = 7;
let y = 9;
let result = "to come";

if(x = y) {
    result = "Equal!";
} else {
    result = "Not equal!";
}

console.log(result);
```

## Challenge Tests

```
assert(result == "Not equal!", 'message: Fix the code so it checks for equality, instead of using assignment in the condition.');

assert(code.test(/if\(x\s*?(==|===)\s*?y/gi), 'message: The condition can use either <code>==</code> or <code>===</code> to test for equality.');
```

## Challenge Solution

```js
"use strict"

let x = 7;
let y = 9;
let result = "to come";

if(x == y) {
    result = "Equal!";
} else {
    result = "Not equal!";
}

console.log(result);
```
