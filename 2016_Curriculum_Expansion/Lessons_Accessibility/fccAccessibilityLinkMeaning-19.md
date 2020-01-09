# Give Links Meaning by using Descriptive Link Text (and not just things like "click here")

## Challenge Description

As we've seen in prior challenges, screen reader users have different options for what type of content their device reads, including skipping to or over landmark elements, jumping to the main content, or getting a page summary from the headings. Another option is to only hear the links available on a page. Screen readers do this by reading the link text, or what's between the anchor (`a`) tags. Having a list of "click here" or "read more" links isn't helpful, instead, use brief but descriptive text within the `a` tags to provide more meaning for these users.

## Instructions

The link text that CamperCat is using is not very descriptive without the surrounding context. Move the anchor (`a`) tags so they wrap around the text "information about batteries" instead of "Click here".

## Challenge Seed

```html
<body>
  <header>
    <h1>Deep Thoughts with Master CamperCat</h1>
  </header>
  <article>
    <h2>Defeating your Foe: the Red Dot is Ours!</h2>
    <p>Felines the world over have been waging war on the most persistent of foes. This red nemesis combines both cunning stealth and lightening speed. But chin up, fellow fighters, our time for victory may soon be near. <a href="">Click here</a> for information about batteries</p>
  </article>
</body>
```

## Challenge Tests

```
assert(code.test(/<a href="">\s*?information about batteries\s*?<\/a>/gi), 'message: Move the anchor <code>a</code> tags from around the words "Click here" to wrap the words "information about batteries". Don\'t remove the <code>href=""</code> attribute');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Deep Thoughts with Master CamperCat</h1>
  </header>
  <article>
    <h2>Defeating your Foe: the Red Dot is Ours!</h2>
    <p>Felines the world over have been waging war on the most persistent of foes. This red nemesis combines both cunning stealth and lightening speed. But chin up, fellow fighters, our time for victory may soon be near. Click here for <a href="">information about batteries</a></p>
  </article>
</body>
```
