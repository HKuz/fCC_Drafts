# Improve Accessibility of Video Content with the Video Element

## Challenge Description

HTML5 offers the `video` element and its partner-in-crime the `track` tag to semantically wrap videos and add accessibility functionality. Multimedia content, which usually has both visual and auditory components, needs synchronized captions and a transcript so users with visual and/or auditory impairments can access it. The `track` element is a child to the `video` tag and provides information plus the source link to the timed caption text track.

Here's an example:
```html
<video id="video" controls width="300" height="300">
	<source src="../video/ninjaWarriorMoves.mp4" type="video/mp4">
	<source src="../video/ninjaWarriorMoves.webm" type="video/webm">
	<track kind="captions" srclang="en" src="../video/captions-en.vtt" label="English">
</video>
```

Note:
Generally, web developers aren't responsible for creating the caption file, but need to know to include it.

The most common forms of web multimedia - Flash and HTML5 Video - both support captioning.
Embedded multimedia is identified via accessible text. 

Audio content without a text alternative is inaccessible for the deaf and hard of hearing. 
For content that is audio only, a transcript will usually suffice.

## Instructions

TO COME

## Challenge Seed

```html
<body>
  <header>
    <h1>Amazing Ninja Cat Video</h1>
  </header>
  <video>
    <source src="" type="video/mp4">
    <source src="" type="video/webm">
    <track>
  </video>
</body>
```

## Challenge Tests

```
assert($('#first').attr('accesskey')), 'message: Make sure to add an <code>accesskey</code> attribute to the <code>a</code> tag with the <code>id</code> of "first".');

assert($('#second').attr('accesskey')), 'message: Make sure to add an <code>accesskey</code> attribute to the <code>a</code> tag with the <code>id</code> of "second".');

assert($('#first').attr('accesskey') === 'g'), 'message: Make sure to set the <code>accesskey</code> attribute on the <code>a</code> tag with the <code>id</code> of "first" to "g". Note that case matters.');

assert($('#second').attr('accesskey') === 'c'), 'message: Make sure to set the <code>accesskey</code> attribute on the <code>a</code> tag with the <code>id</code> of "second" to "c". Note that case matters.');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Deep Thoughts with Master CamperCat</h1>
  </header>
  <article>
    <h2><a accesskey="g" id="first" href="">The Garfield Files: Lasagna as Training Fuel?</a></h2>
    <p>The internet is littered with varying opinions on nutritional paradigms, from catnip paleo to hairball cleanses. But let's turn our attention to an often overlooked fitness fuel, and examine the protein-carb-yummy trifecta that is lasagna...</p>
  </article>
  <article>
    <h2><a accesskey="c" id="second" href="">Is Chuck Norris a Cat Person?</a></h2>
    <p>Chuck Norris is widely regarded as the premier martial artist on the planet, and it's a complete coincidence anyone who disagrees with this fact mysteriously disappears soon after. But the real question is, is he a cat person?...</p>
  </article>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```
