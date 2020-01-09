# Wrap Content in the Article Element

## Challenge Description

We mentioned `article` as one of the new HTML5 elements that adds semantic meaning to your markup in the last challenge. `Article`s are sectioning elements, and are used to wrap independent, self-contained content. The tag works well with blog entries, forum posts, or news articles. Determining whether content can stand alone is usually a judgement call, but there are a couple simple tests you can use. Ask yourself if you removed all surrounding context, would that content still make sense, or similarly for text, would the content hold up if it were in an RSS feed?

Remember that folks using assistive technologies rely on organized, semantically meaningful markup to better appreciate your work.

A note about `section` and `div`:
The `section` element was also added with HTML5, and has a slightly different semantic meaning than `article`. Where `article` is for standalone content, `section` is for grouping thematically related content. They can be used within each other, as needed. For example, if a book is the `article`, then the chapters are the `section`s. When there's no relationship between groups of content, then use a `div`.

`div` - blocks content
`section` - blocks related content
`article` - blocks independent, self-contained content

## Instructions

Astute campers may have noticed that CamperCat used `article` tags to wrap the posts on his blog page, but he forgot to use them around the top one. Change the `div` tag to use an `article` tag instead.

## Challenge Seed

```html
<header>
  <h1>Deep Thoughts with Master CamperCat</h1>
</header>
<div>
  <h2>The Garfield Files: Lasagna as Training Fuel?</h2>
  <p>The internet is littered with varying opinions on nutritional paradigms, from catnip paleo to hairball cleanses. But let's turn our attention to an often overlooked fitness fuel, and examine the protein-carb-NOM trifecta that is lasagna...</p>
</div>

<img src="samuraiSwords.jpeg" alt="">

<article>
  <h2>Defeating your Foe: the Red Dot is Ours!</h2>
  <p>Felines the world over have been waging war on the most persistent of foes. This red nemesis combines both cunning stealth and lightening speed. But chin up, fellow fighters, our time for victory may soon be near...</p>
</article>

<img src="samuraiSwords.jpeg" alt="">

<article>
  <h2>Is Chuck Norris a Cat Person?</h2>
  <p>Chuck Norris is widely regarded as the premier martial artist on the planet, and it's a complete coincidence anyone who disagrees with this fact mysteriously disappears soon after. But the real question is, is he a cat person?...</p>
</article>
<footer></footer>
```

## Challenge Tests

```
assert($('article').length == 3, 'message: There should be three separate <code>article</code> elements in the markup.');

assert($('div').length == 0, 'message: Change the <code>div</code> tag to an <code>article</code> tag.');
```

## Challenge Solution

```html
<header>
  <h1>Deep Thoughts with Master CamperCat</h1>
</header>
<article>
  <h2>The Garfield Files: Lasagna as Training Fuel?</h2>
  <p>The internet is littered with varying opinions on nutritional paradigms, from catnip paleo to hairball cleanses. But let's turn our attention to an often overlooked fitness fuel, and examine the protein-carb-NOM trifecta that is lasagna...</p>
</article>

<img src="samuraiSwords.jpeg" alt="">

<article>
  <h2>Defeating your Foe: the Red Dot is Ours!</h2>
  <p>Felines the world over have been waging war on the most persistent of foes. This red nemesis combines both cunning stealth and lightening speed. But chin up, fellow fighters, our time for victory may soon be near...</p>
</article>

<img src="samuraiSwords.jpeg" alt="">

<article>
  <h2>Is Chuck Norris a Cat Person?</h2>
  <p>Chuck Norris is widely regarded as the premier martial artist on the planet, and it's a complete coincidence anyone who disagrees with this fact mysteriously disappears soon after. But the real question is, is he a cat person?...</p>
</article>
<footer></footer>
```
