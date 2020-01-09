# Change an Element's Relative Position

## Challenge Description

CSS treats each HTML element as its own box, which is usually referred to as the "CSS Box Model". Block-level items automatically start on a new line (think headings, paragraphs, and divs) while inline items sit within surrounding content (like images or spans). The default layout of elements in this way is called the "normal flow" of a document, but CSS offers the `position` property to override it.

When the `position` of an element is set to `relative`, it allows you to specify how CSS should move it *relative* to its current position in the normal flow of the page. It pairs with the CSS offset properties of `left` or `right`, and `top` or `bottom`, which say how many pixels, percentages, or ems to move the item away from where it is normally positioned. The following example moves the paragraph 10 pixels away from the bottom:

```css
p {
  position: relative;
  bottom: 10px;
}
```

Changing an element's `position` to `relative` does not remove it from the normal flow - other elements around it still behave as if that item were there.

## Instructions

Change the `position` of the `h2` to `relative`, and use a CSS offset to move it 15 pixels away from the top of where it sits in the normal flow. Notice there is no impact on the positions of the surrounding `h1` and `p` elements.

## Challenge Seed

```html
<head>
  <style>
  h2 {


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
assert($('h2').css('position') === 'relative'), 'message: Add a CSS rule to specify that the <code>h2</code> has a <code>position</code> set to <code>relative</code>.');

assert($('h2').css('top') === '15px'), 'message: Use a CSS offset to relatively position the <code>h2</code> 15px away from the <code>top</code> of where it normally sits.');
```

## Challenge Solution

```html
<head>
  <style>
  h2 {
    position: relative;
    top: 15px;
  }
  </style>
</head>
<body>
  <h1>On Being Well-Positioned</h1>
  <h2>Move me!</h2>
  <p>I still think the h2 is where it normally sits.</p>
</body>
```
