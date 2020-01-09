# Improve Accessibility of Audio Content with the Audio Element

## Challenge Description

HTML5's `audio` element gives semantic meaning when it wraps sound or audio stream content in your markup. Audio content also needs a text alternative to be accessible to the deaf or hard of hearing. This can be done with nearby text on the page or a link to a transcript.

The `audio` tag supports the `controls` attribute, which shows the browser default play, pause, etc. controls, and supports keyboard functionality. This is a boolean attribute, meaning it doesn't need a value, it's presence on the tag turns the setting on.

Here's an example:

```html
<audio id="meowClip" controls>
	<source src="audio/meow.mp3" type="audio/mpeg" />
	<source src="audio/meow.ogg" type="audio/ogg" />
</audio>
```

Note:
Multimedia content, which usually has both visual and auditory components, needs synchronized captions and a transcript so users with visual and/or auditory impairments can access it. Generally, a web developer is not responsible for creating the captions or transcript, but needs to know to include them.

## Instructions

Let's break from our normally scheduled programming and meet one of our fellow campers, Zersiax (@zersiax), a champion of accessibility and a screen reader user. To hear a clip of his screen reader in action, add an `audio` element (after the `p`) with the `controls` attribute. Then place a `source` tag inside the `audio` tags with the `src` attribute set to "https://s3.amazonaws.com/freecodecamp/screen-reader.mp3" and `type` attribute set to "audio/mpeg".

## Challenge Seed

```html
<body>
  <header>
    <h1>Real Coding Ninjas</h1>
  </header>
  <p>A sound clip of Zersiax's screen reader in action.</p>
  
</body>
```

## Challenge Tests

```
assert($('audio').length === 1, 'message: Make sure to add an <code>audio</code> element after the <code>p</code> tag.');

assert($('audio').attr('controls'), 'message: Make sure the <code>audio</code> tag includes the <code>controls</code> attribute.');

assert($('source').length === 1, 'message: Make sure to add a <code>source</code> element inside the <code>audio</code> tags. Use the example code as a model.');

assert($('audio').children('source').length === 1, 'message: Make sure the <code>source</code> element is a child of the <code>audio</code> element.');

assert($('source').attr('src') === "https://s3.amazonaws.com/freecodecamp/screen-reader.mp3", 'message: Make sure to include the <code>src</code> attribute on the <code>source</code> tag exactly as it is in the instructions.');

assert($('source').attr('type') === "audio/mpeg", 'message: Make sure to include the <code>type</code> attribute on the <code>source</code> tag exactly as it is in the instructions.');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Real Coding Ninjas</h1>
  </header>
  <p>A sound clip of Zersiax's screen reader in action.</p>
  <audio controls>
    <source src="https://s3.amazonaws.com/freecodecamp/screen-reader.mp3" type="audio/mpeg" />
  </audio>
</body>
```
