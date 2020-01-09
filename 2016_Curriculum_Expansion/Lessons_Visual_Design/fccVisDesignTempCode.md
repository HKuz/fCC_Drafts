# Code Examples

## Titles

Change an Element's Relative Position
Move a Relatively Positioned Element with CSS Offsets
Lock an Element to its Parent with Absolute Positioning
Lock an Element to the Browser Window with Fixed Positioning
Push Elements Left or Right with the Float Property

## Relative Positioning

```html
<head>
  <style>
  h2 {
    position: relative;
    top: 15px;
  }
  </style>
</head>
<body>
  <h1>On Being Well-Positioned</h1>
  <h2>Move me!</h2>
  <p>I still think the h2 is where it normally sits.</p>
</body>
```

## Relative Positioning Offset Practice

```html
<head>
  <style>
  h2 {
    position: relative;
    bottom: 10px;
    left: 15px;
  }
  </style>
</head>
<body>
  <h1>On Being Well-Positioned</h1>
  <h2>Move me!</h2>
  <p>I still think the h2 is where it normally sits.</p>
</body>
```

## Absolute Positioning

```html
<style>
  #searchbar {
    position: absolute;
    top: 10px;
    right: 0px;
  }
  section {
    position: relative;
  }
</style>
<body>
  <h1>Welcome!</h1>
  <section>
    <form id="searchbar">
      <label for="search">Search:</label>
      <input type="search" id="search" name="search">
      <input type="submit" name="submit" value="Go!">
    </form>
  </section>
</body>
```

## Fixed Positioning

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

## Float Positioning

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

## Complementary Colors

```html
<style>
  body {
    background-color: #FFFFFF;
  }
  
  .blue {
    background-color: #0000FF;
  }
  
  .yellow {
    background-color: #FFFF00;
  }
  
  div {
    display: inline-block;
    height: 100px;
    width: 100px;
  }
</style>
<div class="blue"></div>
<div class="yellow"></div>
```

## Tertiary Colors

```html
<style>
  body {
    background-color: #FFFFFF;
  }
  .orange {
    background-color: #FF7D00;
  }
  .cyan {
    background-color: #00FFFF;
  }
  .raspberry {
    background-color: #FF007D;
  }  
  div {
    display: inline-block;
    height: 100px;
    width: 100px;
  }
</style>
<div class="orange"></div>
<div class="cyan"></div>
<div class="raspberry"></div>
```

## Adjusting Several Element's to Complementary Colors

```html
<style>
  header {
    background-color: #09A7A1;
    color: #FFFFFF;
    padding: 0.25em;
  }
  h2 {
    color: #09A7A1;
  }  
  button {
    background-color: #FF790E;
  }
  footer {
    background-color: #09A7A1;
    color: #FFFFFF;
    padding: 0.5em;
  }
</style>
<header>
  <h1>Cooking with FCC!</h1>
</header>
<main>
  <article>
    <h2 id="h2-one">Machine Learning in the Kitchen</h2>
    <p>Join this two day workshop that walks through how to implement cutting-edge snack-getting algorithms. Coding usually involves writing exact instructions, but sometimes you need your computer to execute flexible commands, like <code>fetch Pringles</code>.</p>
      <button id="b1">Sign Up</button>
  </article>
  <article>
    <h2 id="h2-two">Bisection Vegetable Chopping</h2>
    <p>This week-long retreat will level-up your coding ninja skills to actual ninja skills. No longer is the humble bisection search limited to sorted arrays or coding interview questions, applying its concepts in the kitchen will have you chopping carrots in O(log n) time before you know it.</p>
    <button id="b2">Sign Up</button>
  </article>
</main>
<br />
<footer>&copy;2016 FCC Kitchen</footer>
```

## Adjust Hue

```html
<style>
  body {
    background-color: #FFFFFF;
  }
  .green {
    background-color: hsl(120, 100%, 50%);
  }
  .cyan {
    background-color: hsl(180, 100%, 50%);
  }
  .blue {
    background-color: hsl(240, 100%, 50%);
  }
  
  div {
    display: inline-block;
    height: 100px;
    width: 100px;
  }
</style>
<div class="green"></div>
<div class="cyan"></div>
<div class="blue"></div>
```


## Adjust Tone

```html
<style>
  header {
    background-color: hsl(178, 90%, 35%);
    color: #FFFFFF;
  }
  nav {
    background-color: hsl(178, 80%, 25%);
  }
  h1 {
    text-indent: 10px;
    padding-top: 10px;
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
    color: inherit;
  }
</style>
<header>
  <h1>Cooking with FCC!</h1>
  <nav>
    <ul>
      <li><a href="">Home</a></li>
      <li><a href="">Classes</a></li>
      <li><a href="">Contact</a></li>
    </ul>
  </nav>
</header>
```
