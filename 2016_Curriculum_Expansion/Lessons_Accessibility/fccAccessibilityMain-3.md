# Jump Straight to the Content Using the Main Element

## Challenge Description

HTML5 introduced a number of new elements that give developers more options while also incorporating accessibility features. These tags include `main`, `header`, `footer`, `nav`, `article`, and `section`, among others. By default, a browser renders these elements similarly to the humble `div`, but using them where appropriate layers additional meaning in your markup. The tag name alone can indicate the type of information it contains, which adds what is called *semantic* meaning to that content. Assistive technologies can access this information to provide better page summary or navigation options to their users.

The `main` element is used to wrap (you guessed it) the main content, and there should be only one per page. It's meant to surround only the information that's related to the central topic of your page, and not include items that repeat across pages, like navigation links or banners. This tag also has an embedded landmark feature that can be used by assistive technology to quickly navigate to the good stuff. If you've ever seen a "Jump to Main Content" link at the top of a page, using a `main` tag automatically gives assistive devices that functionality now.

## Instructions

CamperCat has some big ideas for his ninja weapons page. Help him set up his markup by adding opening and closing `main` tags between the `header` and `footer` in the code below. Keep the `main` tags empty for now.

## Challenge Seed

```html
<header>
  <h1>Weapons of the Ninja</h1>
</header>

<footer></footer>
```

## Challenge Tests

```
assert($('main').length == 1, 'message: Add one <code>main</code> element to the page.');

assert(code.match(/<\/header>\s*?<main>\s*?<\/main>/gi), 'message: Place the <code>main</code> element between the <code>header</code> and <code>footer</code>.');
```

## Challenge Solution

```html
<header>
  <h1>Weapons of the Ninja</h1>
</header>
<main></main>
<footer></footer>
```
