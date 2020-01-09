# Improve Chart Accessibility with the Figure Element

## Challenge Description

HTML5 introduced the `figure` element, along with its buddy `figcaption`. Used together, these items wrap a visual representation (like an image, diagram, chart, etc.) along with its caption. This gives a two-fold accessibility boost by both semantically grouping related content, and providing a text alternative that explains the figure. For data visualizations like charts, the caption can be used to briefly note the trends or conclusions for users with visual impairments, but we'll cover how to move a table version of the chart's data off-screen (using CSS) for screen reader users in another challenge.

Here's an example - note that the `figcaption` goes inside the `figure` tags and can be combined with other elements:

```html
<figure>
  <img src="roundhouseDestruction.jpeg" alt="Photo of CamperCat executing a roundhouse kick">
  <br />
  <figcaption>
    Master CamperCat demonstrates proper form of a roundhouse kick.
  </figcaption>
</figure>
```

## Instructions

CamperCat is hard at work creating a stacked bar chart showing the amount of time per week to spend training in stealth, combat, and weapons. Help him structure his page better by changing the `div` tag he used to a `figure` tag, and the `p` tag that surrounds the caption to a `figcaption` tag.

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
  <section>
    <!-- Only change code below this line -->
    <div>
      <!-- Stacked bar chart will go here -->
      <br />
      <p>Breakdown per week of time to spend training in stealth, combat, and weapons.</p>
    </div>
    <!-- Only change code above this line -->
  </section>
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
assert($('figure').length == 1, 'message: Make sure to use a <code>figure</code> tag instead of the <code>div</code> tag around the chart and caption.');

assert($('figcaption').length == 1, 'message: Make sure to use a <code>figcaption</code> tag instead of the <code>p</code> tag around the caption.');

assert($('div').length == 0, 'message: Change the <code>div</code> tag to a <code>figure</code> tag.');

assert($('p').length == 0, 'message: Change the <code>p</code> tag to a <code>figcaption</code> tag.');

assert($('figure').children('figcaption').length == 1, 'message: Make sure the <code>figcaption</code> is a child of the <code>figure</code> tag.')
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
  <section>
    <!-- Only change code below this line -->
    <figure>
      <!-- Stacked bar chart will go here -->
      <br />
      <figcaption>Breakdown per week of time to spend training in stealth, combat, and weapons.</figcaption>
    </figure>
    <!-- Only change code above this line -->
  </section>
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
