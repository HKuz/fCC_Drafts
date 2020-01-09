# Introduction to the Debugging Challenges

## Challenge Description

Debugging is a valuable and (unfortunately) necessary tool for programmers. It follows the testing phase of checking if your code works as intended, and discovering it does not. Debugging is the process of routing out exactly what isn't working and fixing it.

After spending time creating a brilliant block of code, it can be tough realizing it may have a flaw or two. These issues generally come in three forms - 1) syntax errors that prevent a program from running, 2) runtime errors when code fails to execute or has unexpected behavior, and 3) semantic (or logical) errors when code doesn't do what it's meant to. Modern code editors (and experience) can help identify syntax errors, but semantic and runtime errors can be harder to pin down. They may cause your program to crash, make it run forever, or give incorrect output. Think of debugging as trying to understand why your code is behaving the way it is.

Example of a syntax error - often detected by the code editor:

```js
funtion willNotWork( {
  console.log("Yuck");
}
// "function" keyword is misspelled and there's a missing parenthesis
```

Example of a runtime error - often detected while the program executes:

```js
function loopy() {
  while(true) {
      console.log("Hello, world!");
  }
}

loopy(); // This kicks off an infinite loop, which may crash your browser
```

Example of a semantic error - often detected after testing code output:

```js
function calcAreaOfRect(w, h) {
  return w + h; // This should be w * h
}

let myRectArea = calcAreaOfRect(2, 3);
// Correct syntax and the program executes, but this gives the wrong answer
```

Debugging is potentially frustrating, but it helps to develop (and follow) a systematic approach of checking the intermediate value and/or type of variables against what you think they should be. You can start with a simple process of elimination - if function A works and returned what it's supposed to, then function B may have the issue. Alternatively, you can start checking values in a block of code from the middle to try to cut the search space in half - a problem here indicates a bug in the first half, if not, it's likely in the second, and so on.

This section will cover a couple helpful tools to find bugs, and some of the common forms they take. Fortunately, debugging is a learnable skill that just requires a little patience and practice to master.

## Instructions

N/A

## Challenge Seed

```html
```

## Challenge Tests

```
assert(true, 'message: Carry on')
```

## Challenge Solution

```html
```

## Challenge List
- [x] [Intro text](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243167181)
- [x] [Use console.log to Check the Value of a Variable](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243160968)
- [x] [Using typeof to Check the Type of a Variable](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243161254)
- [x] [Catch Misspelled Variable and Function Names](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243162882)
- [x] [Catch Unclosed Parentheses,  Brackets, Braces and Quotes](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243163631)
- [x] [Catch Mixed Usage of Single and Double Quotes](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243240495)
- [x] [Catch Use of Assignment operator Instead of Equality Operator (= VS == and ===)](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243241537)
- [x] [Catch Missing Open and Closing Parenthesis Afte a Function Call (newFunction() is different than newFunction)](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243243746)
- [x] [Catch Arguments that are Passed in the Wrong Order when Calling a Function](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243277471)
- [x] [Catch "Off By One" Errors when Using Indexing](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243443573)
- [x] [Use Caution when Reinitializing Variables inside a Loop](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243425505)
- [x] [Prevent Infinite Loops with a Valid Terminal Condition](https://github.com/FreeCodeCamp/CurriculumExpansion/issues/47#issuecomment-243507085)

