# Use Caution when Reinitializing Variables inside a Loop

## Challenge Description

Sometimes it's necessary to save information, increment counters, or re-set variables within a loop. A potential issue is when variables either should be reinitialized, and aren't, or vice versa. This is particularly dangerous if you accidentally reset the variable being used for the terminal condition, causing an infinite loop.

Printing variable values with each cycle of your loop by using  `console.log()` can uncover buggy behavior related to resetting, or failing to reset a variable.

## Instructions

The following function is supposed to create a two-dimensional array with `m` rows and `n` columns of zeroes. Unfortunately, it's not producing the expected output because the `row` variable isn't being reinitialized in the outer loop. Fix the code so it returns a correct 3x2 array of zeroes ([[0, 0], [0, 0], [0, 0]]).

## Challenge Seed

```js
"use strict"

function zeroArray(m, n) {
    // Creates a 2-D array with m rows and n columns of zeroes
    let newArray = [];
    let row = [];
    for (let i = 0; i < m; i++) {
        // Adds m rows into newArray
        
        for (let j = 0; j < n; j++) {
            // Adds n zeroes into the current row
            row.push(0);
        }
        newArray.push(row);
    }
    return newArray;
}

let test = zeroArray(3, 2);
console.log(test);
```

## Challenge Tests

```
assert(JSON.stringify(test) === "[[0,0],[0,0],[0,0]]", 'message: <code>test</code> should be an array holding 3 rows of 2 columns of zeroes each.');

assert(test.length === 3, 'message: <code>test</code> should have 3 rows.');

assert(test[0].length === 2 && test[1].length === 2 && test[2].length === 2, 'message: <code>test</code> should have 2 columns in each row.');
```

## Challenge Solution

```js
"use strict"

function zeroArray(m, n) {
    // Creates a 2-D array with m rows and n columns of zeroes
    let newArray = [];    
    for (let i = 0; i < m; i++) {
        // Adds m rows into newArray
        let row = [];
        for (let j = 0; j < n; j++) {
            // Adds n zeroes into the current row
            row.push(0);
        }
        newArray.push(row);
    }
    return newArray;
}

let test = zeroArray(3, 2);
console.log(test);
```
