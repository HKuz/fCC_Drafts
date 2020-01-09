# Catch "Off By One" Errors when Using Indexing

## Challenge Description

"Off by one" errors (sometimes called OBOE) crop up when you're trying to target a specific index of a string or array (to slice or access a segment), or when looping over the indices of them. As you know, JavaScript indexing starts at zero, not one, which means the last index is always one less than the length of the item. If you try to access an index equal to the length, the program may throw an "index out of range" reference error or print `undefined`. Also, read the documentation for any string or array methods that take index ranges as arguments, and understand if they are inclusive (the item at the given index is part of what's returned) or not.

Here are some examples of off by one errors:

```js
let alphabet = "abcdefghijklmnopqrstuvwxyz";
let len = alphabet.length;

for (let i = 0; i <= len; i++) {
    // loops one too many times
    console.log(alphabet[i]);
}

for (let j = 1; j < len; j++) {
    // loops one too few times and misses the first character at index 0
    console.log(alphabet[j]);
}

for (let k = 0; k < len; k++) {
    // Goldilocks approves - this is just right
    console.log(alphabet[k]);
}
```

## Instructions

Fix the two indexing errors in the following function so all the numbers 1 through 5 are printed to the console.

## Challenge Seed

```js
"use strict"

function countToFive() {
    let firstFive = "12345";
    let len = firstFive.length;
    for (let i = 1; i <= len; i++) {
        console.log(firstFive[i]);
    }
}

countToFive();
```

## Challenge Tests

```
assert(code.test(/let i\s*?=\s*?0\s*?;\s*?i\s*?<\s*?len\s*?;/g), 'message: Fix both the initial condition for <code>i</code> and the loop's terminal condition so all five numbers are printed to the console.');
```

## Challenge Solution

```js
"use strict"

function countToFive() {
    let firstFive = "12345";
    let len = firstFive.length;
    for (let i = 0; i < len; i++) {
        console.log(firstFive[i]);
    }
}

countToFive();
```
