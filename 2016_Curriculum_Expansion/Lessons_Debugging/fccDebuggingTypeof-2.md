# Using typeof to Check the Type of a Variable

## Challenge Description

You can use typeof to check the data structure, or type, of a variable. This is useful in debugging when you're working with multiple data types. If you think your code is adding two numbers, but one is actually a string, the results can be unexpected. Type errors can lurk in calculations or function calls. Especially take care when you're accessing and working with external data in the form of a JavaScript object (JSON).

Here are some examples using typeof:

```js
console.log(typeof ""); // outputs "string"
console.log(typeof 0); // outputs "number"
console.log(typeof []); // outputs "object"
console.log(typeof {}); // outputs "object"
```

JavaScript recognizes six primitive (immutable) data types: Boolean, Null, Undefined, Number, String, and Symbol (new with ES6) and one type for mutable items: Object. Note that in JavaScript, arrays are technically a type of object.

## Instructions

Add `console.log()` statements to check the `typeof` each of the two variables `number7` and `string3` in the code.

## Challenge Seed

```js
"use strict"

let number7 = 7;
let string3 = "3";
console.log(number7 + string3);
// Add your code below this line


```


## Challenge Tests

```
assert(code.test(/console.log\(\s*?typeof\s*?\(?number7\)?\s*?\)/g), 'message: Use <code>typeof</code> in a <code>console.log()</code> statement to check the type of the <code>number7</code> variable.');

assert(code.test(/console.log\(\s*?typeof\s*?\(?string3\)?\s*?\)/g), 'message: Use <code>typeof</code> in a <code>console.log()</code> statement to check the type of the <code>string3</code> variable.');
```

## Challenge Solution

```js
"use strict"

let number7 = 7;
let string3 = "3";
console.log(number7 + string3);
// Add your code below this line
console.log(typeof number7);
console.log(typeof string3);
```
