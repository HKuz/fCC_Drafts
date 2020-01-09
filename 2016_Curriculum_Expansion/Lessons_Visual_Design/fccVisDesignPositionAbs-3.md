# Lock an Element to its Parent with Absolute Positioning

## Challenge Description

The next option for the CSS `position` property is `absolute`, which locks the element in place relative to its parent container. Unlike the `relative` position, this removes the element from the normal flow of the document, so surrounding items ignore it. The CSS offset properties (`top` or `bottom` and `left` or `right`) are used to refine the position.

One nuance with `absolute` positioning is that it will be locked relative to its closest *positioned* ancestor. If you forget to add a position rule to the parent item, (typically `position: relative;`), the browser will keep looking up the chain and ultimately default to the `body` tag.

## Instructions

Lock the `#searchbar` element to the top-right of its `section` parent by declaring its `position` as `absolute`. Give it `top` and `right` offsets of 0 pixels each.

## Challenge Seed

```html
<style>
  #searchbar {
    
    
    
  }
  section {
    position: relative;
  }
</style>
<body>
  <h1>Welcome!</h1>
  <section>
    <p>Exciting content</p>
    <form id="searchbar">
      <label for="search">Search:</label>
      <input type="search" id="search" name="search">
      <input type="submit" name="submit" value="Go!">
    </form>
  </section>
</body>
```

## Challenge Tests

```
assert($('#searchbar').css('position') === 'absolute'), 'message: Change the <code>position</code> of the <code>#searchbar</code> element to <code>absolute</code>.');

assert($('#searchbar').css('top') === '0px'), 'message: Use the <code>top</code> CSS offset of 0 pixels on the <code>#searchbar</code> element.');

assert($('#searchbar').css('right') === '0px'), 'message: Use the <code>right</code> CSS offset of 0 pixels on the <code>#searchbar</code> element.');
```

## Challenge Solution

```html
<style>
  #searchbar {
    position: absolute;
    top: 0px;
    right: 0px;
  }
  section {
    position: relative;
  }
</style>
<body>
  <h1>Welcome!</h1>
  <section>
    <p>Exciting content</p>
    <form id="searchbar">
      <label for="search">Search:</label>
      <input type="search" id="search" name="search">
      <input type="submit" name="submit" value="Go!">
    </form>
  </section>
</body>
```
