# Push Elements Left or Right with the Float Property

## Challenge Description

The last positioning tool does not actually use `position`, but sets the `float` property of an element. Floating elements are removed from the normal flow of a document and pushed to either the `left` or `right` of their containing parent element. It's commonly used with the `width` property to specify how much horizontal space the floated element requires.

Note:
Positioning gives you a lot of flexibility and power over the visual layout of a page. It's good to remember that no matter the position of elements, the underlying HTML markup should be organized and still make sense when read from top to bottom. This is how users with visual impairments (who rely on assistive devices like screen readers) access your content.

## Instructions

The given markup would work well as a two-column layout, with the `section` and `aside` elements next to each other. Give the `#left` item a `float` of `left` and the `#right` item a float of `right`.

## Challenge Seed

```html
<head>
  <style>
  #left {
    
    width: 60%;
  }
  #right {
    
    width: 30%;
  }
  aside, section {
    padding: 5px;
    background-color: #ccc;
  }
  </style>
</head>
<body>
  <header>
    <h1>Welcome!</h1>
  </header>
  <section id="left">
    <h2>Content</h2>
    <p>Prepare to be wowed!</p>
  </section>
  <aside id="right">
    <h2>Sidebar</h2>
    <p>Relevant links</p>
  </aside>
</body>
```

## Challenge Tests

```
assert($('#left').css('float') === 'left', 'message: Give the <code>#left</code> element a <code>float</code> value of <code>left</code>.');

assert($('#right').css('float') === 'right', 'message: Give the <code>#right</code> element a <code>float</code> value of <code>right</code>.');
```

## Challenge Solution

```html
<head>
  <style>
  #left {
    float: left;
    width: 60%;
  }
  #right {
    float: right;
    width: 30%;
  }
  aside, section {
    padding: 5px;
    background-color: #ccc;
  }
  </style>
</head>
<body>
  <header>
    <h1>Welcome!</h1>
  </header>
  <section id="left">
    <h2>Content</h2>
    <p>Prepare to be wowed!</p>
  </section>
  <aside id="right">
    <h2>Sidebar</h2>
    <p>Relevant links</p>
  </aside>
</body>
```
