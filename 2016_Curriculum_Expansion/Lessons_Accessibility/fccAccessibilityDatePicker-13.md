# Add a Date Picker

## Challenge Description

Forms often include the `input` field, which can be used to create several different form controls. The `type` attribute on this element indicates what kind of input will be created. You may have noticed the `text` and `submit` `input` types in prior challenges, and HTML5 introduced an option to specify a `date` field. Depending on browser support, a date picker shows up in the input field when it's in focus, which makes filling in a form easier for all users. For older browsers, the `type` will default to `text`, so it helps to show users the expected date format just in case.

Here's an example:

```html
<label for="input1">Enter a date (MM-DD-YYYY):</label>
<input type="date" id="input1" name="input1">
```

## Instructions

CamperCat is setting up a mortal combat tournament and wants to survey his likely competitors to see what date works best. Add an `input` tag under the `label`, which has a `type` attribute of 'date', an `id` attribute of 'pickdate', and a `name` attribute of 'date'.

## Challenge Seed

```html
<body>
  <header>
    <h1>Tournaments</h1>
  </header>
  <section>
    <h2>Mortal Combat Tournament Survey</h2>
    <form>
      <p>Tell us the best date for the competition</p>
      <label for="pickdate">Preferred Date (MM-DD-YYYY):</label>
      <!-- Add your code below this line -->
      
      <!-- Add your code above this line -->
      <input type="submit" name="submit" value="Submit">
    </form>
  </section>
  <br>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```

## Challenge Tests

```
assert($('input').length == 2, 'message: Make sure to add one <code>input</code> tag for the date selector field above the <code>input</code> tag for submit.');

assert($('input').attr('type') == 'date', 'message: Make sure to have a <code>type</code> attribute of \'date\' on your <code>input</code> tag.');

assert($('input').attr('id') == 'pickdate', 'message: Make sure to have an <code>id</code> attribute of \'pickdate\' on your <code>input</code> tag.');

assert($('input').attr('name') == 'date', 'message: Make sure to have a <code>name</code> attribute of \'date\' on your <code>input</code> tag.');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Tournaments</h1>
  </header>
  <section>
    <h2>Mortal Combat Tournament Survey</h2>
    <form>
      <p>Tell us the best date for the competition</p>
      <label for="pickdate">Preferred Date:</label>
      <!-- Add your code below this line -->
      <input type="date" id="pickdate" name="date">
      <!-- Add your code above this line -->
      <input type="submit" name="submit" value="Submit">
    </form>
  </section>
  <br>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```
