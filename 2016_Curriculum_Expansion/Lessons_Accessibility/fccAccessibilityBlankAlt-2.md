# Know when alt text should be left blank

## Challenge Description

In the last challenge, you learned that including an `alt` attribute on `img` tags is mandatory. However, sometimes images are grouped with a caption already describing them, or are used for decoration only, and `alt` text may seem redundant or unnecessary. In situations when an image is already explained with text content, or does not add meaning to a page, the `img` still needs an `alt` attribute, but it can be set to an empty string. Here's an example:

`<img src="visualDecoration.jpeg" alt="">`

Background images usually fall under the 'decorative' label as well, but they are typically applied with CSS rules, and are therefore not part of the markup that screen readers process.

## Instructions

CamperCat has coded a skeleton page for the blog part of his website below. He's planning to add a visual break between his two articles with a decorative image of a samurai sword. Add an `alt` attribute to the `img` tag in the code below and set it to an empty string.

## Challenge Seed

```html
<header>
  <h1>Deep Thoughts with Master CamperCat</h1>
</header>
<article>
  <h2>Defeating your Foe: the Red Dot is Ours!</h2>
  <p>To Come...</p>
</article>

<img src="samuraiSwords.jpeg">

<article>
  <h2>Is Chuck Norris a Cat Person?</h2>
  <p>To Come...</p>
</article>
<footer></footer>
```

## Challenge Tests

```
assert(!($('img').attr('alt') == undefined), 'message: Make sure to add an <code>alt</code> attribute to the <code>img</code> tag.');

assert($('img').attr('alt') == "", 'message: The <code>alt</code> attribute should be set to an empty string.');
```

## Challenge Solution

```html
<header>
  <h1>Deep Thoughts with Master CamperCat</h1>
</header>
<article>
  <h2>Defeating your Foe: the Red Dot is Ours!</h2>
  <p>To Come...</p>
</article>

<img src="samuraiSwords.jpeg" alt="">

<article>
  <h2>Is Chuck Norris a Cat Person?</h2>
  <p>To Come...</p>
</article>
<footer></footer>
```
