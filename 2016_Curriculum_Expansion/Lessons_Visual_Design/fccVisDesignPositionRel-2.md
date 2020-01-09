# Move a Relatively Positioned Element using CSS Offsets

## Challenge Description

When combined with an element whose `position` is `relative`, the CSS offsets of `top` or `bottom`, and `left` or `right` tell the browser how far to offset that item relative to where it would sit in the normal flow of the document. This can be slightly confusing, because you're offsetting an element away from given spot, which effectively moves it towards the opposite direction. As you saw in the last challenge, using the `top` offset moved the `h2` downwards. Likewise, using a `left` offset effectively moves an item to the right.

## Instructions

Let's do one more problem for practice. Move the `h2` 15 pixels to the right and 10 pixels up.

## Challenge Seed

```html
<head>
  <style>
  h2 {
    position: relative;
    
    
  }
  </style>
</head>
<body>
  <h1>On Being Well-Positioned</h1>
  <h2>Move me!</h2>
  <p>I still think the h2 is where it normally sits.</p>
</body>
```

## Challenge Tests

```
assert($('h2').css('bottom') === '10px'), 'message: Use a CSS offset to relatively position the <code>h2</code> 10px upwards, in other words, 10px away from the <code>bottom</code> of where it normally sits.');

assert($('h2').css('left') === '15px'), 'message: Use a CSS offset to relatively position the <code>h2</code> 15px towards the right, in other words, 15px away from the <code>left</code> of where it normally sits.');
```

## Challenge Solution

```html
<head>
  <style>
  h2 {
    position: relative;
    bottom: 10px;
    left: 15px;
  }
  </style>
</head>
<body>
  <h1>On Being Well-Positioned</h1>
  <h2>Move me!</h2>
  <p>I still think the h2 is where it normally sits.</p>
</body>
```
