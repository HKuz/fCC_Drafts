# Catch Misspelled Variable and Function Names

## Challenge Description

Now that we've covered the two primary ways to check intermediate values and types of program output, let's get into the common forms that bugs take. One syntax-level issue that folks with fast typing skills can commiserate with is the humble spelling error. Transposed, missing, or mis-capitalized characters in a variable or function name will have the browser looking for an object that doesn't exist - and complain in the form of a reference error. As you know, JavaScript variable and function names are case-sensitive.

## Instructions

Fix the two spelling errors in the code so the `netWorkingCapital` calculation works.

## Challenge Seed

```js
"use strict"

let receivables = 10;
let payables = 8;
let netWorkingCapital = recievables - payable;
console.log(`Net working capital is: ${netWorkingCapital}`);
```

## Challenge Tests

```
assert(netWorkingCapital === 2, 'message: Check the spelling of the two variables used in the <code>netWorkingCapital</code> calculation, the console output should show that "Net working capital is: 2".');

assert(!code.test(/recievables/g), 'message: Make sure the <code>receivables</code> variable is spelled correctly.');

assert(!code.test(/payable\s*?;/g), 'message: Make sure the <code>payables</code> variable is spelled correctly.');
```

## Challenge Solution

```js
"use strict"

let receivables = 10;
let payables = 8;
let netWorkingCapital = receivables - payables;
console.log(`Net working capital is: ${netWorkingCapital}`);
```
