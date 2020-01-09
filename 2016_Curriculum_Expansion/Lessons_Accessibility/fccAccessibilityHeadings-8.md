# Use Headings to Show Hierarchical Relationships of Content (Don't skip from H1 to H3 or leave out H1)

## Challenge Description

Headings (`h1` through `h6` elements) are workhorse tags that help provide structure and labeling to your content. Given these characteristics, screen readers can be set to read only the headings on a page so the user gets a summary. This means it is important for the heading tags in your markup to have semantic meaning and relate to each other, not be picked merely for their size values. If you were writing a paper with an introduction, a body, and a conclusion, you wouldn't put the conclusion as a subsection of the body in your outline, right? Similarly, the heading tags in a webpage need to go in order and indicate the hierarchical relationships of your content - ones with equal (or higher) rank start new implied sections, headings with lower rank start subsections of the previous one.

As an example, a page with an `h2` element followed by several subsections labeled with `h4` tags would confuse a screen reader user. With six choices, it's tempting to use a tag because it looks right in a browser, but you can use CSS to edit the relative sizing.

One final point, your page should always have one `h1` element, which is the main subject of your content.

## Instructions

CamperCat wants a page dedicated to becoming a ninja and has some ideas in place. Help him fix the headings so his markup gives semantic meaning to the content, and shows the proper parent-child relationships of his sections. Change all the `h5` tags to the proper heading level to indicate they are subsections of the `h2` ones.

## Challenge Seed

```html
<header>
  <h1>How to Become a Ninja</h1>
</header>
<main>
  <h2>Learn the Art of Moving Stealthily</h2>
  <h5>How to Hide in Plain Sight</h5>
  <h5>How to Climb a Wall</h5>
  
  <h2>Learn the Art of Battle</h2>
  <h5>How to Strengthen your Body</h5>
  <h5>How to Fight like a Ninja</h5>
  
  <h2>Learn the Art of Living with Honor</h2>
  <h5>How to Breathe Properly</h5>
  <h5>How to Simplify your Life</h5> 
</main>
<footer></footer>
```

## Challenge Tests

```
assert($('h3').length === 6, 'message: Make sure to replace the <code>h5</code> tags with <code>h3</code> tags');

assert($('h5').length === 0, 'message: Make sure to replace all the <code>h5</code> tags on the page.')
```

## Challenge Solution

```html
<header>
  <h1>How to Become a Ninja</h1>
</header>
<main>
  <h2>Learn the Art of Moving Stealthily</h2>
  <h3>How to Hide in Plain Sight</h3>
  <h3>How to Climb a Wall</h3>
  
  <h2>Learn the Art of Battle</h2>
  <h3>How to Strengthen your Body</h3>
  <h3>How to Fight like a Ninja</h3>
  
  <h2>Learn the Art of Living with Honor</h2>
  <h3>How to Breathe Properly</h3>
  <h3>How to Simplify your Life</h3>  
</main>
<footer></footer>

```
