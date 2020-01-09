# Make Screen Reader Navigation easier to access with the Nav Landmark

## Challenge Description

The `nav` element is another item in the HTML5 suite with the embedded landmark feature for easy screen reader navigation. This tag is meant to wrap around the main navigation links in your page. If there are repeated site links at the bottom of the page, it isn't necessary to markup those with a `nav` tag as well, using a `footer` (covered in the next challenge) is sufficient.

## Instructions

CamperCat included navigation links at the top of his training page, but wrapped them in a `div`. Change the `div` to a `nav` tag to improve the accessibility on his page.

## Challenge Seed

```html
<body>
  <header>
    <h1>Training with CamperCat</h1>
    <div>
      <ul>
        <li><a href="#stealth">Stealth &amp; Agility</a></li>
        <li><a href="#combat">Combat</a></li>
        <li><a href="#weapons">Weapons</a></li>
      </ul>
    </div>
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

## Challenge Tests

```
assert($('nav').length == 1, 'message: Make sure to use a <code>nav</code> tag instead of the <code>div</code> tag around the navigation links.');

assert($('div').length == 0, 'message: Change the <code>div</code> tag to a <code>nav</code> tag.');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Training with CamperCat</h1>
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
</body>
```
