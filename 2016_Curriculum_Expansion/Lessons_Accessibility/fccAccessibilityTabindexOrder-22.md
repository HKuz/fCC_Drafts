# Use tabindex to specify the order of keyboard focus for several elements

## Challenge Description

The next function that the `tabindex` attribute offers is to specify the exact tab order of elements. This is achieved when the value of the attribute is set to a positive number of 1 or higher. Setting a `tabindex="1"` will bring keyboard focus to that element first, then cycle through the sequence of specified `tabindex` values (2, 3, etc.), before moving to default and `tabindex="0"` items. It's important to note that when the tab order is set this way, it overrides the default order (which uses the HTML source), and may confuse users who are expecting to start navigation from the top of the page. This technique may be necessary in some circumstances, but in terms of accessibility, take care before applying it.

Here's an example:
```html
<div tabindex="1">I get keyboard focus, and I get it first!</div>
<div tabindex="2">I get keyboard focus, and I get it second!</div>
```

## Instructions

CamperCat has a search field on his Inspirational Quotes page that he plans to position in the upper right corner with CSS. He wants the search `input` and submit `input` form controls to be the first two items in the tab order. Add a `tabindex` attribute set to "1" to the search `input`, and a `tabindex` attribute set to "2" to the submit `input`.

## Challenge Seed

```html
<body>
  <header>
    <h1>Even Deeper Thoughts with Master CamperCat</h1>
    <nav>
      <ul>
        <li><a href="">Home</a></li>
        <li><a href="">Blog</a></li>
        <li><a href="">Training</a></li>
      </ul>
    </nav>
  </header>
  <form>
    <label for="search">Search:</label>
    <input type="search" name="search" id="search">
    <input type="submit" name="submit" value="Submit" id="submit">
  </form>
  <h2>Inspirational Quotes</h2>
  <blockquote>
    <p>&ldquo;There's no Theory of Evolution, just a list of creatures I've allowed to live.&rdquo;<br>
    - Chuck Norris</p>
  </blockquote>
  <blockquote>
    <p>&ldquo;Wise men say forgiveness is divine, but never pay full price for late pizza.&rdquo;<br>
    - TMNT</p>
  </blockquote>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```

## Challenge Tests

```
assert($('#search').attr('tabindex')), 'message: Make sure to add a <code>tabindex</code> attribute to the search <code>input</code> tag.');

assert($('#submit').attr('tabindex')), 'message: Make sure to add a <code>tabindex</code> attribute to the submit <code>input</code> tag.');

assert($('search').attr('tabindex') === '1'), 'message: Make sure to set the <code>tabindex</code> attribute on the search <code>input</code> tag to "1".');

assert($('submit').attr('tabindex') === '2'), 'message: Make sure to set the <code>tabindex</code> attribute on the submit <code>input</code> tag to "2".');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Even Deeper Thoughts with Master CamperCat</h1>
    <nav>
      <ul>
        <li><a href="">Home</a></li>
        <li><a href="">Blog</a></li>
        <li><a href="">Training</a></li>
      </ul>
    </nav>
  </header>
  <form>
    <label for="search">Search:</label>
    <input type="search" name="search" id="search" tabindex="1">
    <input type="submit" name="submit" value="Submit" id="submit" tabindex="2">
  </form>
  <h2>Inspirational Quotes</h2>
  <blockquote>
    <p>&ldquo;There's no Theory of Evolution, just a list of creatures I've allowed to live.&rdquo;<br>
    - Chuck Norris</p>
  </blockquote>
  <blockquote>
    <p>&ldquo;Wise men say forgiveness is divine, but never pay full price for late pizza.&rdquo;<br>
    - TMNT</p>
  </blockquote>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```
