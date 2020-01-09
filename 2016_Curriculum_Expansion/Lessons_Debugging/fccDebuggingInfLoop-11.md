# Prevent Infinite Loops with a Valid Terminal Condition

## Challenge Description

Our final topic is the dreaded infinite loop. Loops are great tools when you need your program to run a code block a certain number of times or until a condition is met, but they need a terminal condition that ends the looping. Infinite loops are likely to freeze or crash the browser, and cause general program execution mayhem, which no one wants.

We saw an example of an infinite loop in the introduction - there is no terminal condition to break out of this `while` loop:

```js
function loopy() {
  while(true) {
      console.log("Hello, world!");
  }
}
```

It's the programmer's job to ensure that the terminal condition, which tells the program when to break out of the loop code, is eventually reached. Some errors include incrementing or decrementing a counter variable in the wrong direction from the terminal condition, or accidentally resetting a counter or index variable within the loop code, instead of incrementing or decrementing it.

## Instructions

The below function contains an infinite loop because the terminal condition `i != 4` will never be reached - `i` will increment by 2 each pass, and jump right over 4 since it's odd to start. Fix the comparison operator in the terminal condition so the loop only runs for `i` up to 4.

## Challenge Seed

```js
"use strict"

function myFunc() {
    for (let i = 1; i != 4; i += 2) {
        console.log("Still going!");
    }
}
```

## Challenge Tests

```
assert(code.test(/for\s*?\(\s*?let i\s*?=\s*?1;\s*?i\s*?(<=|<)\s*?4\s*?;\s*?i\s*?\+=\s*?2\s*?\)/g), 'message: Only change the comparison operator of <code>!=</code> in the terminal condition so the loop terminates for values bigger than 4. Don't change any other parts of the loop statement.');
```

## Challenge Solution

```js
"use strict"
function myFunc() {
    for (let i = 1; i <= 4; i += 2) {
        console.log("Still going!");
    }
}
```
