This challenge is meant for the end of the HTML section.

# Declare the Doctype of an HTML Document

## Challenge Description

The challenges so far have covered specific HTML tags and their uses. However, there are a few elements that give overall structure to your page, and should be included in every HTML document.

At the top of your document, you need to tell the browser which version of HTML your page is using. HTML is an evolving language, and is updated regularly. Most major browsers support the latest specification, which is HTML5. However, older web pages may use previous versions of the language. You tell the browser this information by adding the <code>&lt;!DOCTYPE ...&gt;</code> tag on the first line, where the "..." part is the version of HTML. For HTML5, you use <code>&lt;!DOCTYPE html&gt;</code>.

The <code>!</code> and uppercase <code>DOCTYPE</code> is important, especially for older browsers. The <code>html</code> is not case sensitive.

Next, the rest of your HTML code needs to be wrapped in <code>html</code> tags.  The opening <code>&lt;html&gt;</code> goes directly below the <code>&lt;!DOCTYPE html&gt;</code> line, and the closing <code>&lt;/html&gt;</code> goes at the end of the page.

Here's an example of the page structure:

<blockquote>&lt;!DOCTYPE html&gt;<br>&lt;html&gt;<br>  &lt;!-- Your HTML code goes here --&gt;<br>&lt;/html&gt;</blockquote>

<h4>Instructions</h4>

Add a <code>DOCTYPE</code> tag for HTML5 to the top of the blank HTML document in the code editor. Under it, add opening and closing <code>html</code> tags, which wrap around an <code>h1</code> heading that can include any text.


## Challenge Seed

```html



```

## Challenge Tests

```js
assert(code.match(/<!DOCTYPE\s+?html\s*?>/gi), 'message Your code should include a <code>&lt;!DOCTYPE html&gt;</code> tag.');
assert($('html').length == 1, 'There should be one <code>html</code> element.');
assert($('html').children('h1').length == 1, 'message: The <code>html</code> tags should wrap around one <code>h1</code> element.');
```

## Challenge Solution


```html
<!DOCTYPE html>
<html>
  <h1>My Webpage!</h1>
</html>
```



# Define the Head and Body of an HTML Document

## Challenge Description

You can add another level of organization in your HTML document within the <code>html</code> tags with the <code>head</code> and <code>body</code> elements. Any markup with information about your page would go into the <code>head</code> tag. Then any markup with the content of the page (what displays for a user) would go into the <code>body</code> tag.

Metadata elements, such as <code>link</code>, <code>meta</code>, <code>title</code>, and <code>style</code>, typically go inside the <code>head</code> element.

Here's an example of a page's layout:

<blockquote>&lt;!DOCTYPE html&gt;<br>&lt;html&gt;<br>  &lt;head&gt;<br>    &lt;!-- metadata elements --&gt;<br>  &lt;/head&gt;<br>  &lt;body&gt;<br>    &lt;!-- page contents --&gt;<br>  &lt;/body&gt;<br>&lt;/html&gt;</blockquote>

<h4>Instructions</h4>

Edit the markup so there's a <code>head</code> and a <code>body</code>. The <code>head</code> should only include the <code>title</code>, and the <code>body</code> should only include the <code>h1</code> and <code>p</code>.

## Challenge Seed

```html
<!DOCTYPE html>
<html>

  <title>The best page ever</title>


  <h1>The best page ever</h1>
  <p>Cat ipsum dolor sit amet, jump launch to pounce upon little yarn mouse, bare fangs at toy run hide in litter box until treats are fed. Go into a room to decide you didn't want to be in there anyway. I like big cats and i can not lie kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff. Meow i could pee on this if i had the energy for slap owner's face at 5am until human fills food dish yet scamper. Knock dish off table head butt cant eat out of my own dish scratch the furniture. Make meme, make cute face. Sleep in the bathroom sink chase laser but pee in the shoe. Paw at your fat belly licks your face and eat grass, throw it back up kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>

</html>  
```

## Challenge Tests

```js
assert($('head').length == 1, 'message: There should be only one <code>head</code> element on the page.');
assert($('body').length == 1, 'message: There should be only one <code>body</code> element on the page.');
assert($('html').children('head').length == 1, 'message: The <code>head</code> element should be a child of the <code>html</code> element.');
assert($('html').children('body').length == 1, 'message: The <code>body</code> element should be a child of the <code>html</code> element.');
assert($('head').children('title').length == 1, 'message: The <code>head</code> element should wrap around the <code>title</code> element.');
assert($('body').children('h1').length == 1 && $('body').children('p').length == 1, 'message: The <code>body</code> element should wrap around both the <code>h1</code> and <code>p</code> elements.');
```

## Challenge Solution

```html
<!DOCTYPE html>
<html>
  <head>
    <title>The best page ever</title>
  </head>
  <body>
    <h1>The best page ever</h1>
    <p>Cat ipsum dolor sit amet, jump launch to pounce upon little yarn mouse, bare fangs at toy run hide in litter box until treats are fed. Go into a room to decide you didn't want to be in there anyway. I like big cats and i can not lie kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff. Meow i could pee on this if i had the energy for slap owner's face at 5am until human fills food dish yet scamper. Knock dish off table head butt cant eat out of my own dish scratch the furniture. Make meme, make cute face. Sleep in the bathroom sink chase laser but pee in the shoe. Paw at your fat belly licks your face and eat grass, throw it back up kitty ipsum dolor sit amet, shed everywhere shed everywhere stretching attack your ankles chase the red dot, hairball run catnip eat the grass sniff.</p>
  </body>
</html>  
```
