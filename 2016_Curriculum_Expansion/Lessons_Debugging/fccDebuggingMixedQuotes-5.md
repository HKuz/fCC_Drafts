# Catch Mixed Usage of Single and Double Quotes

## Challenge Description

JavaScript allows the use of both single ('') and double ("") quotes to declare a string, and deciding which one to use generally comes down to personal preference. Having two choices is great when your string has contractions or another piece of text that's in quotes. Just be careful that you don't close the string too early, which causes a syntax error.

Examples of mixing quotes:

```js
// These work
const grouchoContraction = "I've had a perfectly wonderful evening, but this wasn't it.";
const quoteInString = "Groucho Marx once said 'Quote me as saying I was mis-quoted.'";

// This is wrong
const uhOhGroucho = 'I've had a perfectly wonderful evening, but this wasn't it.';
```

Of course, if you prefer to only use one style of quotes, then you can escape the ones inside the string by using the backslash escape character:

```js
const allSameQuotes = 'I\'ve had a perfectly wonderful evening, but this wasn\'t it.';
```

## Instructions

Fix the string so it either uses different quotes for the `href` value, or escape the existing ones.

## Challenge Seed

```js
"use strict"

let innerHtml = "<p>Click here to <a href="#Home">return home.</a></p>"
console.log(innerHtml);
```

## Challenge Tests

```
assert(code.test(/href=('|\")#Home('|\")/gi), 'message: Fix the quotes around the <code>href</code> value "#Home" by either changing or escaping them.');
```

## Challenge Solution

```js
"use strict"

let innerHtml = "<p>Click here to <a href='#Home'>return home.</a></p>"
console.log(innerHtml);
```
