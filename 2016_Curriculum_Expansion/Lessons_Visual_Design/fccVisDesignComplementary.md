# Learn about Complementary Colors

## Description:

Color theory and its impact on design is a deep topic and only the basics will be covered in the following challenges. Color can be used on a website to draw attention to content, evoke emotions, or create visual harmony. Using different combinations of colors can dramatically change the look of a website, and a lot of thought can go into picking a color palette that works with your content.

The color wheel is a useful tool to visualize how colors relate to each other - similar hues are neighbors and different hues are farther apart. When two colors are opposite each other on the wheel, they are called complementary colors. They have the characteristic that if they are combined, they effectively cancel each other out and result in a gray color. However, when placed side-by-side, these colors will make each other appear more vibrant and produce a strong visual contrast.

Some examples of complementary colors with their `hex codes` are:

red (`#FF0000`) and cyan (`#00FFFF`)
green (`#00FF00`) and magenta (`#FF00FF`)
blue (`#0000FF`) and yellow (`#FFFF00`)

There are many color picking tools available online that have an option to find the complement of a color.

Note for all color challenges:
Using color can be a powerful way to add visual interest to a page. However, color alone should not be used as the only way to convey important information because users with visual impairments may not understand that content. This issue will be covered in more detail in the Applied Accessibility challenges.

## Instructions

Change the `background-color` property of the `blue` and `yellow` classes to their respective colors. Notice how the colors look different next to each other than they do compared against the white background.

## Challenge Seed

```html
<style>
  body {
    background-color: #FFFFFF;
  }
  
  .blue {
    background-color: #000000;
  }
  
  .yellow {
    background-color: #000000;
  }
  
  div {
    display: inline-block;
    height: 100px;
    width: 100px;
  }
</style>
<div class="blue"></div>
<div class="yellow"></div>
```

## Challenge Tests

```
assert($('.blue').css('background-color') === 'rgb(0, 0, 255)', 'message: Give the <code>div</code> element with class <code>blue</code> the <code>background-color</code> blue.');

assert($('.yellow').css('background-color') === 'rgb(255, 255, 0)', 'message: Give the <code>div</code> element with class <code>yellow</code> the <code>background-color</code> yellow.');

```

## Challenge Solution

```html
<style>
  body {
    background-color: #FFFFFF;
  }
  
  .blue {
    background-color: #0000FF;
  }
  
  .yellow {
    background-color: #FFFF00;
  }
  
  div {
    display: inline-block;
    height: 100px;
    width: 100px;
  }
</style>
<div class="blue"></div>
<div class="yellow"></div>
```
