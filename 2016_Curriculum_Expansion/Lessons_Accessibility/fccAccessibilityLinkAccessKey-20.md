# Make Links Navigatable with HTML Access Keys

## Challenge Description

HTML offers the `accesskey` attribute to specify a shortcut key to activate or bring focus to an element. This can make navigation more efficient for keyboard-only users. HTML5 allows this attribute to be used on any element, but it's of particular use when paired with interactive ones, such as links, buttons, and form controls.

Here's an example:
`<button accesskey="b">Important Button</button>`

## Instructions

CamperCat wants the links around the two blog article titles to have keyboard shortcuts so his site's users can quickly navigate to the full story. Add an `accesskey` attribute to both links and set the first one to "g" (for Garfield) and the second one to "c" (for Chuck Norris).

## Challenge Seed

```html
<body>
  <header>
    <h1>Deep Thoughts with Master CamperCat</h1>
  </header>
  <article>
    <h2><a id="first" href="">The Garfield Files: Lasagna as Training Fuel?</a></h2>
    <p>The internet is littered with varying opinions on nutritional paradigms, from catnip paleo to hairball cleanses. But let's turn our attention to an often overlooked fitness fuel, and examine the protein-carb-yummy trifecta that is lasagna...</p>
  </article>
  <article>
    <h2><a id="second" href="">Is Chuck Norris a Cat Person?</a></h2>
    <p>Chuck Norris is widely regarded as the premier martial artist on the planet, and it's a complete coincidence anyone who disagrees with this fact mysteriously disappears soon after. But the real question is, is he a cat person?...</p>
  </article>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```

## Challenge Tests

```
assert($('#first').attr('accesskey')), 'message: Make sure to add an <code>accesskey</code> attribute to the <code>a</code> tag with the <code>id</code> of "first".');

assert($('#second').attr('accesskey')), 'message: Make sure to add an <code>accesskey</code> attribute to the <code>a</code> tag with the <code>id</code> of "second".');

assert($('#first').attr('accesskey') === 'g'), 'message: Make sure to set the <code>accesskey</code> attribute on the <code>a</code> tag with the <code>id</code> of "first" to "g". Note that case matters.');

assert($('#second').attr('accesskey') === 'c'), 'message: Make sure to set the <code>accesskey</code> attribute on the <code>a</code> tag with the <code>id</code> of "second" to "c". Note that case matters.');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Deep Thoughts with Master CamperCat</h1>
  </header>
  <article>
    <h2><a accesskey="g" id="first" href="">The Garfield Files: Lasagna as Training Fuel?</a></h2>
    <p>The internet is littered with varying opinions on nutritional paradigms, from catnip paleo to hairball cleanses. But let's turn our attention to an often overlooked fitness fuel, and examine the protein-carb-yummy trifecta that is lasagna...</p>
  </article>
  <article>
    <h2><a accesskey="c" id="second" href="">Is Chuck Norris a Cat Person?</a></h2>
    <p>Chuck Norris is widely regarded as the premier martial artist on the planet, and it's a complete coincidence anyone who disagrees with this fact mysteriously disappears soon after. But the real question is, is he a cat person?...</p>
  </article>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```
