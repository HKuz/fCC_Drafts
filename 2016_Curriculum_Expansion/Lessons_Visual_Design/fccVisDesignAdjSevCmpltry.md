# Adjusting the Color of Various Elements to Complementary Colors

## Description:

The complementary colors challenge showed that opposite colors on the color wheel can make each other appear more vibrant when placed side-by-side. However, the strong visual contrast can be jarring if it's overused on a website, and can sometimes make text harder to read if it's placed on a complementary-colored background. In practice, one of the colors is usually dominant and the complement is used to bring visual attention to certain content on the page.


## Instructions

This page will use a shade of teal (`#09A7A1`) as the dominant color, and its orange (`#FF790E`) complement to visually highlight the sign-up buttons. Change the `background-color` of both the `header` and `footer` from black to the teal color. Then change the `h2` text `color` to teal as well. Finally, change the `background-color` of the `button` to the orange color.

## Challenge Seed

```html
<style>
  body {
    background-color: white;
  }
  header {
    background-color: black;
    color: white;
    padding: 0.25em;
  }
  h2 {
    color: black;
  }  
  button {
    background-color: white;
  }
  footer {
    background-color: black;
    color: white;
    padding: 0.5em;
  }
</style>
<header>
  <h1>Cooking with FCC!</h1>
</header>
<main>
  <article>
    <h2>Machine Learning in the Kitchen</h2>
    <p>Join this two day workshop that walks through how to implement cutting-edge snack-getting algorithms with a command line interface. Coding usually involves writing exact instructions, but sometimes you need your computer to execute flexible commands, like <code>fetch Pringles</code>.</p>
    <button>Sign Up</button>
  </article>
  <article>
    <h2>Bisection Vegetable Chopping</h2>
    <p>This week-long retreat will level-up your coding ninja skills to actual ninja skills. No longer is the humble bisection search limited to sorted arrays or coding interview questions, applying its concepts in the kitchen will have you chopping carrots in O(log n) time before you know it.</p>
    <button>Sign Up</button>
  </article>
</main>
<br />
<footer>&copy;2016 FCC Kitchen</footer>
```

## Challenge Tests

```
assert($('header').css('background-color') === 'rgb(9, 167, 161)', 'message: Give your <code>header</code> element the <code>background-color</code> #09A7A1.');

assert($('footer').css('background-color') === 'rgb(9, 167, 161)', 'message: Give your <code>footer</code> element the <code>background-color</code> #09A7A1.');

assert($('h2').css('color') === 'rgb(9, 167, 161)', 'message: Give your <code>h2</code> element the <code>color</code> #09A7A1.');

assert($('button').css('background-color') === 'rgb(255, 121, 14)', 'message: Give your <code>button</code> element the <code>background-color</code> #FF790E.');
```

## Challenge Solution

```html
<style>
  header {
    background-color: #09A7A1;
    color: #FFFFFF;
    padding: 0.25em;
  }
  h2 {
    color: #09A7A1;
  }  
  button {
    background-color: #FF790E;
  }
  footer {
    background-color: #09A7A1;
    color: #FFFFFF;
    padding: 0.5em;
  }
</style>
<header>
  <h1>Cooking with FCC!</h1>
</header>
<main>
  <article>
    <h2 id="h2-one">Machine Learning in the Kitchen</h2>
    <p>Join this two day workshop that walks through how to implement cutting-edge snack-getting algorithms. Coding usually involves writing exact instructions, but sometimes you need your computer to execute flexible commands, like <code>fetch Pringles</code>.</p>
      <button id="b1">Sign Up</button>
  </article>
  <article>
    <h2 id="h2-two">Bisection Vegetable Chopping</h2>
    <p>This week-long retreat will level-up your coding ninja skills to actual ninja skills. No longer is the humble bisection search limited to sorted arrays or coding interview questions, applying its concepts in the kitchen will have you chopping carrots in O(log n) time before you know it.</p>
    <button id="b2">Sign Up</button>
  </article>
</main>
<br />
<footer>&copy;2016 FCC Kitchen</footer>
```
