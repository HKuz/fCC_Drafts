# Make Screen Reader Navigation easier with the Header Landmark

## Challenge Description

The next HTML5 element that adds semantic meaning and improves accessibility is the `header` tag. It's used to wrap introductory information or navigation links for its parent tag, and works well around content that's repeated at the top on multiple pages.

`Header` shares the embedded landmark feature we saw with `main`, allowing assistive technologies to quickly navigate to that content. Where the `header` is used on your page makes a difference. It's perfectly fine to have `headers` in other sectioned parts of the your page, within `article` or `section` tags. However, it's important to note if a `header` is placed in one of those tags, it loses the landmark navigation capabilities.

Note:
`Header` is meant for use in the `body` tag of your HTML document. This is different than the `head` element, which contains the page's `title`, `meta` information, etc.

## Instructions

CamperCat is writing some great articles about ninja training, and wants to add a page for them to his site. Help him fix the top `div` that currently contains the `h1` to a `header` tag instead.

## Challenge Seed

```html
<body>
  <div>
    <h1>Training with CamperCat</h1>
  </div>
  <section id="stealth">
    <h2>Stealth &amp; Agility Training</h2>
    <article><h3>Quickly climb foliage using a minimum spanning tree approach</h3></article>
    <article><h3>No training is NP-complete without parkour</h3></article>
  </section>
  <section id="combat">
    <h2>Combat Training</h2>
    <article><h3>Dispatch multiple enemies with multithreaded tactics</h3></article>
    <article><h3>Goodbye world: 5 proven ways to knock out an opponent</h3></article>
  </section>
  <section id="weapons">
    <h2>Weapons Training</h2>
    <article><h3>Swords: the best tool to literally divide and conquer</h3></article>
    <article><h3>Breadth-first or depth-first in multi-weapon training?</h3></article>
  </section>
</body>
```

## Challenge Tests

```
assert($('header').length == 1, 'message: Make sure to use a <code>header</code> tag instead of the <code>div</code> tag around the <code>h1</code>.');

assert($('div').length == 0, 'message: Change the <code>div</code> tag to a <code>header</code> tag.');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Training with CamperCat</h1>
  </header>
  <section id="stealth">
    <h2>Stealth &amp; Agility Training</h2>
    <article><h3>Quickly climb foliage using a minimum spanning tree approach</h3></article>
    <article><h3>No training is NP-complete without parkour</h3></article>
  </section>
  <section id="combat">
    <h2>Combat Training</h2>
    <article><h3>Dispatch multiple enemies with multithreaded tactics</h3></article>
    <article><h3>Goodbye world: 5 proven ways to knock out an opponent</h3></article>
  </section>
  <section id="weapons">
    <h2>Weapons Training</h2>
    <article><h3>Swords: the best tool to literally divide and conquer</h3></article>
    <article><h3>Breadth-first or depth-first in multi-weapon training?</h3></article>
  </section>
</body>
```
