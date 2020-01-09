# Adjust the Tone of a Color

## Description:

The `hsl()` option in CSS also makes it easy to adjust the tone of a color. Mixing white with a pure hue creates a **tint** of that color, and adding black will make a **shade**. Alternatively, a **tone** is produced by adding gray, while the hue stays the same, or by both tinting and shading. Recall that the 's' and 'l' of `hsl()` stand for saturation and lightness, respectively. The saturation percent changes the amount of gray and the lightness percent determines how much white or black is in the color. This is useful when you have a base hue you like, but need different variations of it.

## Instructions

The navigation bar on this site currently inherits its `background-color` from the `header` element. Starting with that color as a base, add a `background-color` to the `nav` element so it uses the same teal hue, but has `80%` saturation and `25%` lightness values to change its tone and shade.

## Challenge Seed

```html
<style>
  header {
    background-color: hsl(178, 90%, 35%);
    color: #FFFFFF;
  }
  nav {
    
  }
  h1 {
    text-indent: 10px;
    padding-top: 10px;
  }
  nav ul {
    margin: 0px;
    padding: 5px 0px 5px 30px;
  }
  nav li {
    display: inline;
    margin-right: 20px;
  }
  a {
    text-decoration: none;
    color: inherit;
  }
</style>
<header>
  <h1>Cooking with FCC!</h1>
  <nav>
    <ul>
      <li><a href="">Home</a></li>
      <li><a href="">Classes</a></li>
      <li><a href="">Contact</a></li>
    </ul>
  </nav>
</header>
```

## Challenge Tests

```
assert($('header').css('background-color') === 'rgb(8, 169, 164)', 'message: Don't change the <code>background-color</code> of the <code>header</code> element.');

assert($('nav').css('background-color') === 'rgb(12, 114, 111)', 'message: Give your <code>nav</code> element a <code>background-color</code> of the adjusted teal.');

assert(code.match(/nav\s*?{\s*?background-color:\s*?hsl/gi), 'message: Use <code>hsl()</code> to state the <code>nav background-color</code>.');
```

## Challenge Solution

```html
<style>
  header {
    background-color: hsl(178, 90%, 35%);
    color: #FFFFFF;
  }
  nav {
    background-color: hsl(178, 80%, 25%);
  }
  h1 {
    text-indent: 10px;
    padding-top: 10px;
  }
  nav ul {
    margin: 0px;
    padding: 5px 0px 5px 30px;
  }
  nav li {
    display: inline;
    margin-right: 20px;
  }
  a {
    text-decoration: none;
    color: inherit;
  }
</style>
<header>
  <h1>Cooking with FCC!</h1>
  <nav>
    <ul>
      <li><a href="">Home</a></li>
      <li><a href="">Classes</a></li>
      <li><a href="">Contact</a></li>
    </ul>
  </nav>
</header>
```