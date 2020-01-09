# Improve Form Field Accessibility with the Label Element (use the "for" property)

## Challenge Description

Improving accessibility using semantic HTML markup applies to using both appropriate tag names and attributes. We'll cover several important scenarios using attributes in forms in the next few challenges. You may have seen a `label` tag wrapping the text for a specific form control item, which ties meaning to it and makes it more readable. The `for` attribute on a `label` tag explicitly associates that label with the form control and is used by screen readers. The value of the `for` attribute must be the same as the value of the `id` attribute of the form control.

Here's an example:
```html
<form>
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
</form>
```

## Instructions

CamperCat expects a lot of interest in his thought-provoking blog posts, and wants to include an email sign up form. Add a `for` attribute on the email `label` that matches the `id` on its `input` field.

## Challenge Seed

```html
<body>
  <header>
    <h1>Deep Thoughts with Master CamperCat</h1>
  </header>
  <section>    
    <form>
      <p>Sign up to receive CamperCat's blog posts by email here!</p>
      <label>Email:</label>
      <input type="text" id="email" name="email">
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
assert($('label').attr('for'), 'message: Give the <code>label</code> tag a <code>for</code> attribute, and make sure it is not empty.');

assert($('label').attr('for') == 'email', 'message: Make sure the <code>for</code> attribute matches the value of the email <code>input id</code>attribute, which is case sensitive.');
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
