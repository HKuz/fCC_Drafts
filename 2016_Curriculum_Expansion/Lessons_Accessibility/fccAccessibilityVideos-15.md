# Add Subtitles to a Video to Improve Accessibility

## Challenge Description

At least one subtitle format is supported (WebVTT or TTML)
Controls are keyboard accessible (controls must be focusable)

Here's an example:

```html
<video id="video1" controls width="300" height="300">
	<source src="../video/ElephantsDream.mp4" type="video/mp4">
	<source src="../video/ElephantsDream.webm" type="video/webm">
	<track kind="captions" srclang="en" src="../video/subtitles-en.vtt" label="English">
</video>
```

## Instructions

CamperCat wants information about the ninja level of his users when they sign up for his email list. He's added a set of radio buttons, and learned from our last lesson to use `label` tags with `for` attributes for each choice. Go CamperCat! However, his code still needs some help. Change the `div` tag surrounding the radio buttons to a `fieldset` tag, and change the `p` tag inside it to a `legend`.

## Challenge Seed

```html
<body>
  <header>
    <h1>Deep Thoughts with Master CamperCat</h1>
  </header>
  <section>
    <form>
      <p>Sign up to receive CamperCat's blog posts by email here!</p>
      <label for="email">Email:</label>
      <input type="text" id="email" name="email">
      <!-- Only make changes below this line -->
      <div>
        <p>What level ninja are you?</p>
        <input id="newbie" type="radio" name="levels" value="newbie">
        <label for="newbie">Newbie Kitten</label><br>
        <input id="intermediate" type="radio" name="levels" value="intermediate">
        <label for="intermediate">Developing Student</label><br>
        <input id="master" type="radio" name="levels" value="master">
        <label for="master">Master</label>
      </div>
      <!-- Only make changes above this line -->
      <input type="submit" name="submit" value="Submit">
    </form>
  </section>
  <article>
    <h2>The Garfield Files: Lasagna as Training Fuel?</h2>
    <p>The internet is littered with varying opinions on nutritional paradigms, from catnip paleo to hairball cleanses. But let's turn our attention to an often overlooked fitness fuel, and examine the protein-carb-yummy trifecta that is lasagna...</p>
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
  <footer>&copy; 2016 CamperCat</footer>
</body>
```

## Challenge Tests

```
assert($('fieldset').length == 1, 'message: Make sure to use a <code>fieldset</code> tag instead of a <code>div</code> around the radio button set.');

assert($('legend').length == 1, 'message: Make sure to use a <code>legend</code> tag instead of the <code>p</code> tag around the text asking what level ninja a user is.');

assert($('div').length == 0, 'message: Change the <code>div</code> tag to a <code>fieldset</code> tag.');

assert($('p').length == 4, 'message: Change the <code>p</code> tag to a <code>legend</code> tag.');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Deep Thoughts with Master CamperCat</h1>
  </header>
  <section>
    <form>
      <p>Sign up to receive CamperCat's blog posts by email here!</p>
      <label for="email">Email:</label>
      <input type="text" id="email" name="email">
      <!-- Only make changes below this line -->
      <fieldset>
        <legend>What level ninja are you?</legend>
        <input id="newbie" type="radio" name="levels" value="newbie">
        <label for="newbie">Newbie Kitten</label><br>
        <input id="intermediate" type="radio" name="levels" value="intermediate">
        <label for="intermediate">Developing Student</label><br>
        <input id="master" type="radio" name="levels" value="master">
        <label for="master">Master</label>
      </fieldset>
      <!-- Only make changes above this line -->
      <input type="submit" name="submit" value="Submit">
    </form>
  </section>
  <article>
    <h2>The Garfield Files: Lasagna as Training Fuel?</h2>
    <p>The internet is littered with varying opinions on nutritional paradigms, from catnip paleo to hairball cleanses. But let's turn our attention to an often overlooked fitness fuel, and examine the protein-carb-yummy trifecta that is lasagna...</p>
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
  <footer>&copy; 2016 CamperCat</footer>
</body>
```
