# Standardize Times with the DateTime HTML5 Property

## Challenge Description

Continuing with the date theme, HTML5 also introduced the `time` element along with a `datetime` attribute to standardize times. This is an inline element that can wrap a date or time on a page, then a valid format of that date is held by the `datetime` attribute, which is the value accessed by assistive devices. It helps avoid confusion by stating a standardized version of a time, even if it's written in an informal or colloquial manner.

Here's an example:

```html
<p>Master CamperCat officiated the cage match between Goro and Scorpion <time datetime="2013-02-13">last Wednesday</time>,
 which ended in a draw.</p>
```

## Instructions

CamperCat's mortal combat survey results are in! Wrap a `time` tag around the text "Thursday, September 15<sup>th<sup>" and add a `datetime` attribute to it set to "2016-09-15".

## Challenge Seed

```html
<body>
  <header>
    <h1>Tournaments</h1>
  </header>
  <article>
    <h2>Mortal Combat Tournament Survey Results</h2>
    <p>Thank you to everyone for responding to Master CamperCat's survey. The best day to host the vaunted Mortal Combat tournament is Thursday, September 15<sup>th</sup>. May the best ninja win!</p>
    <section>
      <h3>Comments:</h3>
      <article>
        <p>Posted by: Sub-Zero on <time datetime="2016-08-13T20:01Z">August 13<sup>th</sup></time></p>
        <p>Johnny Cage better be there, I'll finish him!</p>
      </article>
      <article>
        <p>Posted by: Doge on <time datetime="2016-08-15T08:12Z">August 15<sup>th</sup></time></p>
        <p>Wow, much combat, so mortal.</p>
      </article>
      <article>
        <p>Posted by: The Grim Reaper on <time datetime="2016-08-16T00:00Z">August 16<sup>th</sup></time></p>
        <p>Looks like I'll be busy that day.</p>
      </article>
    </section>
  </article>
  <br>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```

## Challenge Tests

```
assert(code.test(/<time \s*?datetime=("|')2016-09-15("|')\s*?>\s*?Thursday, September 15<sup>th<\/sup>\s*?\.?\s*?<\/time>/gi), 'message: Make sure to place an opening and closing <code>time</code> tag around "Thursday, September 15<sup>th</sup>" and include a <code>datetime</code> attribute set to "2016-09-15".');

assert($('time').attr('datetime'), 'message: Make sure to add a <code>datetime</code> attribute on your <code>time</code> element.');

assert($('time').attr('datetime') === "2016-09-15", 'message: Make sure the <code>datetime</code> attribute is set to "2016-09-15".');
```

## Challenge Solution

```html
<body>
  <header>
    <h1>Tournaments</h1>
  </header>
  <article>
    <h2>Mortal Combat Tournament Survey Results</h2>
    <p>Thank you to everyone for responding to Master CamperCat's survey. The best day to host the vaunted Mortal Combat tournament is <time datetime="2016-09-15">Thursday, September 15<sup>th</sup></time>. May the best ninja win!</p>
    <section>
      <h3>Comments:</h3>
      <article>
        <p>Posted by: Sub-Zero on <time datetime="2016-08-13T20:01Z">August 13<sup>th</sup></time></p>
        <p>Johnny Cage better be there, I'll finish him!</p>
      </article>
      <article>
        <p>Posted by: Doge on <time datetime="2016-08-15T08:12Z">August 15<sup>th</sup></time></p>
        <p>Wow, much combat, so mortal.</p>
      </article>
      <article>
        <p>Posted by: The Grim Reaper on <time datetime="2016-08-16T00:00Z">August 16<sup>th</sup></time></p>
        <p>Looks like I'll be busy that day.</p>
      </article>
    </section>
  </article>
  <br>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```
