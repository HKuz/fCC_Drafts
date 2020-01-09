# Learn about Tertiary Colors

## Description:

Computer monitors and device screens create different colors by combining amounts of red, green, and blue light. This is known as the RGB additive color model in modern color theory, where red (R), green (G), and blue (B) are called primary colors. Mixing two primary colors creates the secondary colors cyan (G + B), magenta (R + B), and yellow (R + G). You saw in the Complementary Colors lesson that these secondary colors happen to be the complement to the primary color not used in their creation, and are opposite to them on the color wheel.

Tertiary colors are the result of combining a primary color with one of its secondary color neighbors. For example, red (primary) and yellow (secondary) make orange. This adds six more colors to a simple color wheel for a total of twelve.

[NOTE TO DRAFT: INCLUDING A 12-COLOR RGB COLOR WHEEL DIAGRAM IN THIS LESSON MAY BE HELPFUL]

There are various methods of selecting different colors that result in a harmonious combination in design. One example that can use tertiary colors is called the split-complementary color scheme. It starts with a base color, then pairs it with the two colors that are adjacent to its complement. The three colors provide strong visual contrast in a design, but is more subtle than using two complementary colors.

Here are three colors using the split-complement scheme:

cyan (`#00FFFF`)
orange (`#FF7D00`)
raspberry (`FF007D`)

## Instructions

Change the `background-color` property of the `orange`, `cyan`, and `raspberry` classes to their respective colors. Make sure to use the `hex codes` because the orange and raspberry in the example above are not browser-recognized color names.

## Challenge Seed

```html
<style>
  body {
    background-color: #FFFFFF;
  }
  .orange {
    background-color: #000000;
  }
  .cyan {
    background-color: #000000;
  }
  .raspberry {
    background-color: #000000;
  }  
  div {
    display: inline-block;
    height: 100px;
    width: 100px;
  }
</style>
<div class="orange"></div>
<div class="cyan"></div>
<div class="raspberry"></div>
```

## Challenge Tests

```
assert($('.orange').css('background-color') === 'rgb(255, 125, 0)', 'message: Give the <code>div</code> element with class <code>orange</code> the <code>background-color</code> orange.');

assert($('.cyan').css('background-color') === 'rgb(0, 255, 255)', 'message: Give the <code>div</code> element with class <code>cyan</code> the <code>background-color</code> cyan.');

assert($('.raspberry').css('background-color') === 'rgb(255, 0, 125)', 'message: Give the <code>div</code> element with class <code>raspberry</code> the <code>background-color</code> raspberry.');
```

## Challenge Solution

```html
<style>
  body {
    background-color: #FFFFFF;
  }
  .orange {
    background-color: #FF7D00;
  }
  .cyan {
    background-color: #00FFFF;
  }
  .raspberry {
    background-color: #FF007D;
  }  
  div {
    display: inline-block;
    height: 100px;
    width: 100px;
  }
</style>
<div class="orange"></div>
<div class="cyan"></div>
<div class="raspberry"></div>
```
