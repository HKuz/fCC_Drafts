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
      <fieldset>
        <legend>What level ninja are you?</legend>
        <input id="newbie" type="radio" name="levels" value="newbie">
        <label for="newbie">Newbie Kitten</label><br>
        <input id="intermediate" type="radio" name="levels" value="intermediate">
        <label for="intermediate">Developing Student</label><br>
        <input id="master" type="radio" name="levels" value="master">
        <label for="master">Master</label>
      </fieldset>
      <input type="submit" name="submit" value="Submit">
    </form>
  </section>
  <article>
    <h2>A Word on the Recent Catnip Doping Scandal</h2>
    <p>The influence that catnip has on feline behavior is well-documented, and its use as an herbal supplement in competitive ninja circles remains controversial. Once again, the debate to ban the substance is brought to the public's attention after the high-profile win of Kittytron, a long-time proponent and user of the green stuff, at the Claw of Fury tournament. As I've stated in the past, I firmly believe a true ninja's skills must come from within, with no external influences. My own catnip use shall continue as purely recreational.</p>
  </article>
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

## Survey - tabindex zero

```html
<body>
  <header>
    <h1>Ninja Survey</h1>
  </header>
  <section>
    <form>
      <p tabindex="0">Instructions: Fill in form below with your information then click <b>Submit</b></p>
      <label for="username">Username:</label>
      <input type="text" id="username" name="username"><br>
      <fieldset>
        <legend>What level ninja are you?</legend>
        <input id="newbie" type="radio" name="levels" value="newbie">
        <label for="newbie">Newbie Kitten</label><br>
        <input id="intermediate" type="radio" name="levels" value="intermediate">
        <label for="intermediate">Developing Student</label><br>
        <input id="master" type="radio" name="levels" value="master">
        <label for="master">9th Life Master</label>
      </fieldset>
      <br>
      <fieldset>
      <legend>Select your favorite weapons:</legend>
      <input id="stars" type="checkbox" name="weapons" value="stars">
      <label for="stars">Throwing Stars</label><br>
      <input id="nunchucks" type="checkbox" name="weapons" value="nunchucks">
      <label for="nunchucks">Nunchucks</label><br>
      <input id="sai" type="checkbox" name="weapons" value="sai">
      <label for="sai">Sai Set</label><br>
      <input id="sword" type="checkbox" name="weapons" value="sword">
      <label for="sword">Sword</label>
      </fieldset>
      <br>
      <input type="submit" name="submit" value="Submit">
    </form><br>
  </section>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```

## Inspirational Quotes - tabindex 1

```html
<body>
  <header>
    <h1>Even Deeper Thoughts with Master CamperCat</h1>
    <nav>
      <ul>
        <li><a href="">Home</a></li>
        <li><a href="">Blog</a></li>
        <li><a href="">Training</a></li>
      </ul>
    </nav>
  </header>
  <form>
    <label for="search">Search:</label>
    <input type="search" name="search" id="search">
    <input type="submit" name="submit" value="Submit">
  </form>
  <h2>Inspirational Quotes</h2>
  <blockquote>
    <p>&ldquo;There's no Theory of Evolution, just a list of creatures I've allowed to live.&rdquo;<br>
    - Chuck Norris</p>
  </blockquote>
  <blockquote>
    <p>&ldquo;Wise men say forgiveness is divine, but never pay full price for late pizza.&rdquo;<br>
    - TMNT</p>
  </blockquote>
  <footer>&copy; 2016 CamperCat</footer>
</body>
```

## Table Comparison - tabindex order?

```html
<head>
  <style>
  .sr-only {
    position: absolute;
    left: -10000px;
    top: auto;
    width: 1px;
    height: 1px;
    overflow: hidden;
  }
  </style>
</head>
<body>
  <form>
    <table summary="This table allows you to compare any two fighters">
      <caption><b>Ninja Comparison</b></caption>
      <tr>
        <th scope="col">Info</th>
        <th scope="col">Ninja 1</th>
        <th scope="col">Ninja 2</th>
      </tr>
      <tr>
        <th>Weight</th>
        <td>
          <label for="N1Weight" class="sr-only">Ninja 1 Weight</label>
          <input type="text" size="15" value="" name="n1Weight" id="N1Weight" tabindex="10">
        </td>
        <td>
          <label for="N2Weight" class="sr-only">Ninja 2 Weight</label>
          <input type="text" size="15" value="" name="n2Weight" id="N2Weight" tabindex="20">
        </td>
      </tr>
      <tr>
        <th>Speed</th>
        <td>
          <label for="N1Speed" class="sr-only">Ninja 1 Speed</label>
          <input type="text" size="15" value="" name="N1Speed" id="N1Speed" tabindex="30">
        </td>
        <td>
          <label for="N2Speed" class="sr-only">Ninja 2 Speed</label>
          <input type="text" size="15" value="" name="N2Speed" id="N2Speed" tabindex="40">
        </td>
      </tr>
    </table>
    <input type="submit">
  </form>
</body>
```

## Audio Kiai

```html
<body>
  <header>
    <h1>The Only Sound of a Ninja</h1>
  </header>
  <h2>Master CamperCat's Kiai</h2>
  <audio controls></audio>
  <p>A clip of Master CamperCat's terrifying meow</p>
</body>
```
