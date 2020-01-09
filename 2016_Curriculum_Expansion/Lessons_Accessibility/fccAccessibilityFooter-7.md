# Make Screen Reader Navigation Easier with the Footer Landmark

## Challenge Description

Similar to `header` and `nav`, the `footer` element has a built-in landmark feature to aid assistive devices with navigation. It's primarily used to contain copyright information or links to related documents for a page. A `footer` can be placed within `articles` or `sections` as part of their content, but as we saw with `header`, this removes the landmark navigation component. Of course, it still retains its semantic meaning within your markup.

## Instructions

CamperCat's training page is making good progress. Change the `div` he used to wrap his copyright information at the bottom of the page to a `footer` element.

## Challenge Seed

```html
<body>
  <header>
    <h1>Training</h1>
    <nav>
      <ul>
        <li><a href="#stealth">Stealth &amp; Agility</a></li>
        <li><a href="#combat">Combat</a></li>
        <li><a href="#weapons">Weapons</a></li>
      </ul>
    </nav>
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
  <div>&copy; 2016 CamperCat</div>
</body>
```

## Challenge Tests

```
assert($('footer').length == 1, 'message: Make sure to use a <code>footer</code> tag instead of the <code>div</code> tag around the copyright information.');

assert($('div').length == 0, 'message: Change the <code>div</code> tag to a <code>footer</code> tag.');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Training</h1>
    <nav>
      <ul>
        <li><a href="#stealth">Stealth &amp; Agility</a></li>
        <li><a href="#combat">Combat</a></li>
        <li><a href="#weapons">Weapons</a></li>
      </ul>
    </nav>
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
  <footer>&copy; 2016 CamperCat</footer>
</body>
```
