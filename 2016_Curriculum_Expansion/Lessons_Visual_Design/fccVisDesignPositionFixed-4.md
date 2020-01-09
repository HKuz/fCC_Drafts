# Lock an Element to the Browser Window with Fixed Positioning

## Challenge Description

The next layout scheme that CSS offers is the `fixed` position, which is a type of absolute positioning that locks an element relative to the browser window. Similar to `absolute` positioning, it's used with the CSS offset properties and also removes the element from the normal flow of the document. Other items no longer "realize" where it is positioned, which may require some layout adjustments elsewhere.

One key difference from the `absolute` position is that the element won't move when the user scrolls.

## Instructions

The navigation bar in the code is labeled with an `id` of `navbar`. Change its `position` to `fixed`, and offset it 0 pixels from the `top` and 0 pixels from the `left`.

## Challenge Seed

```html
<style>
  #navbar {
    
    
    
    width: 100%;
    background-color: #767676;
  }
  nav ul {
    margin: 0px;
    padding: 5px 0px 5px 30px;
  }
  nav li {
    display: inline;
    margin-right: 20px;
  }
  a {
    text-decoration: none;
  }
</style>
<body>
  <header>
    <h1>Welcome!</h1>
    <nav id="navbar">
      <ul>
        <li><a href="">Home</a></li>
        <li><a href="">Contact</a></li>
      </ul>
    </nav>
  </header>
  <p>I shift up when the #navbar is fixed to the browser window.</p>
</body>
```

## Challenge Tests

```
assert($('#navbar').css('position') === 'fixed', 'message: Change the <code>position</code> of the <code>#navbar</code> element to <code>fixed</code>.');

assert($('#navbar').css('top') === '0px', 'message: Use the <code>top</code> CSS offset of 0 pixels on the <code>#navbar</code> element.');

assert($('#navbar').css('left') === '0px', 'message: Use the <code>left</code> CSS offset of 0 pixels on the <code>#navbar</code> element.');
```

## Challenge Solution

```html
<style>
  #navbar {
    position: fixed;
    top: 0px;
    left: 0px;
    width: 100%;
    background-color: #767676;
  }
  nav ul {
    margin: 0px;
    padding: 5px 0px 5px 30px;
  }
  nav li {
    display: inline;
    margin-right: 20px;
  }
  a {
    text-decoration: none;
  }
</style>
<body>
  <header>
    <h1>Welcome!</h1>
    <nav id="navbar">
      <ul>
        <li><a href="">Home</a></li>
        <li><a href="">Contact</a></li>
      </ul>
    </nav>
  </header>
  <p>I shift up when the #navbar is fixed to the browser window.</p>
</body>
```
