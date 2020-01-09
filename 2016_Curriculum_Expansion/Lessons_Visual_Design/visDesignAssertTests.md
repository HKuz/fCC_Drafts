# Visual Design Assert Tests using Regex

- Create Visual Balance Using the Text-align Property
  "assert(code.match(/h4\\s*?{\\s*?text-align:\\s*?center;\\s*?}/gi), 'message: Use the text-align property on the <code>h4</code> tag and set it to center.');",
  "assert(code.match(/p\\s*?{\\s*?text-align:\\s*?justify;\\s*?}/gi), 'message: Use the text-align property on the <code>p</code> tag and set it to justify.');",
  "assert(code.match(/a\\s*?{\\s*?text-align:\\s*?left;\\s*?}/gi), 'message: Use the text-align property on the <code>a</code> tag and set it to left.');"
- Adjust the Width of an Element Using the Width Property
  "assert(code.match(/\\.card-img-top\\s*?{\\s*?width:\\s*?75px;\\s*?}/gi), 'message: Change the width value of the logo to 75 pixels by using the <code>card-img-top</code> class selector.');"
- Adjust the Height of an Element Using the Height Property
  "assert(code.match(/h4\\s*?{\\s*?text-align:\\s*?center;\\s*?height:\\s*?40px;/gi), 'message: Change the <code>h4</code> height value to 40 pixels.');"
- Create a Visual Balance with the Height of an Element
  "assert(code.match(/h4\\s*?{\\s*?text-align:\\s*?center;\\s*?height:\\s*?25px;/gi), 'message: Change the <code>h4</code> height value to 25 pixels.');"
- Create Visual Emphasis by Using bold text
  
- Create Visual Emphasis by Underlining Text
- Create Visual Emphasis by Wrapping the Em Tag Around Text
- Create Visual Emphasis by using Strikethrough on Text
- Create a Line Using the HR Element
- Create Visual Emphasis by Adjusting the Background-color Property of Text
  "assert(code.match(/h4\\s*?{\\s*?.*?\\s*?.*?\\s*?.*?\\s*?background-color:\\s*?rgba\\(45,\\s*?45,\\s*?45,\\s*?0?\\.1\\);/gi), 'message: Add a background-color property to the <code>h4</code> element set to the gray color with 0.1 opacity.');",
  "assert(code.match(/h4\\s*?{\\s*?.*?\\s*?.*?\\s*?padding:\\s*?10px;/gi), 'message: Add a padding property to the <code>h4</code> element and set it to 10 pixels.');",
  "assert(!code.match(/h4\\s*?{\\s*?.*?\\s*?height:\\s*?25px;/gi), 'message: Make sure to remove the height property on the <code>h4</code> element.');"
- Create Visual Emphasis by Adjusting the Size of a Header Versus a Paragraph Tag
  "assert(code.match(/font-size:\\s*?1.3em/gi), 'message: Add a font-size property to the <code>h4</code> element set to 1.3em.');"
- Create Visual Emphasis by Adding a Box-Shadow to a Card-like Element
  "assert(code.match(/#thumbnail:hover\\s*?{\\s*?box-shadow:\\s*?0 10px 20px rgba\\(0,\\s*?0,\\s*?0,\\s*?0?\\.19\\),\\s*?0 6px 6px rgba\\(0,\\s*?0,\\s*?0,\\s*?0?\\.23\\);/gi), 'message: Add a <code>box-shadow</code> property to the <code>thumbnail</code> id using the given CSS.');"
- Decrease the Opacity of an Element
  "assert(code.match(/\\.card-img-top\\s*?{\\s*?width:\\s*?75px;\\s*?opacity:\\s*?0?\\.9;\\s*?}/gi), 'message: Use the opacity property set to 0.9 on the logo image tag with the class of <code>.card-img-top</code>.');"

- Learn the Importance of Ratios in Type - NO CHALLENGE
- Learn About Modular Type - NO CHALLENGE
- Apply Different Ratios to Type Using the font-size Property - NO CHALLENGE
- Create a Typographic Style Guide - NO CHALLENGE
- Set the Font Size Values of Heading Elements
- Set the value of Paragraph text to 16px
- Adjust the color of an Anchor Tag
- Adjust the Hover State of an Anchor Tag
- Adjust the Font-Weight of Header Tags
- Adjust the Line-Height of Paragraphs
- Use the Text-Transform Property to Make Text Uppercase
- Use a Google Font


- Change an Element's Relative Position
  assert(code.match(/position:\\s*?relative/gi), 'message: Add a CSS rule to specify that the <code>h2</code> has a <code>position</code> set to <code>relative</code>.');
  assert(code.match(/top:\\s*?15px/gi), 'message: Use a CSS offset to relatively position the <code>h2</code> 15px away from the <code>top</code> of where it normally sits.');
- Move a Relatively Positioned Element with CSS Offsets
  assert(code.match(/bottom:\\s*?10px/gi), 'message: Use a CSS offset to relatively position the <code>h2</code> 10px upwards, in other words, 10px away from the <code>bottom</code> of where it normally sits.');
  assert(code.match(/left:\\s*?15px/gi), 'message: Use a CSS offset to relatively position the <code>h2</code> 15px towards the right, in other words, 15px away from the <code>left</code> of where it normally sits.');
- Lock an Element to its Parent with Absolute Positioning
  assert(code.match(/position:\\s*?absolute/gi), 'message: Change the <code>position</code> of the <code>#searchbar</code> element to <code>absolute</code>.');
  assert(code.match(/top:\\s*?0px/gi), 'message: Use the <code>top</code> CSS offset of 0 pixels on the <code>#searchbar</code> element.');
  assert(code.match(/right:\\s*?0px/gi), 'message: Use the <code>right</code> CSS offset of 0 pixels on the <code>#searchbar</code> element.');
- Lock an Element to the Browser Window with Fixed Positioning
  assert(code.match(/position:\\s*?fixed/gi), 'message: Change the <code>position</code> of the <code>#navbar</code> element to <code>fixed</code>.');
  assert(code.match(/top:\\s*?0px/gi), 'message: Use the <code>top</code> CSS offset of 0 pixels on the <code>#navbar</code> element.');
  assert(code.match(/left:\\s*?0px/gi), 'message: Use the <code>left</code> CSS offset of 0 pixels on the <code>#navbar</code> element.');
- Push Elements Left or Right with the Float Property
  assert(code.match(/#left\\s*?{\\s*?float:\\s*?left/gi), 'message: Give the <code>#left</code> element a <code>float</code> value of <code>left</code>.');
  assert(code.match(/#right\\s*?{\\s*?float:\\s*?right/gi), 'message: Give the <code>#right</code> element a <code>float</code> value of <code>right</code>.');
- Change the Position of Overlapping Elements with the Z-index Property

- Learn about Complementary Colors - NO CODE EDITOR
  assert(code.match(/\\.blue\\s*?{\\s*?background-color:\\s*?#0000FF/gi), 'message: Give the <code>div</code> element with class <code>blue</code> the <code>background-color</code> blue.');  assert(code.match(/\\.yellow\\s*?{\\s*?background-color:\\s*?#FFFF00/gi), 'message: Give the <code>div</code> element with class <code>yellow</code> the <code>background-color</code> yellow.');
- Learn about Tertiary Colors - NO CODE EDITOR
  assert(code.match(/\\.orange\\s*?{\\s*?background-color:\\s*?#FF7D00/gi), 'message: Give the <code>div</code> element with class <code>orange</code> the <code>background-color</code> orange.');
  assert(code.match(/\\.cyan\\s*?{\\s*?background-color:\\s*?#00FFFF/gi), 'message: Give the <code>div</code> element with class <code>cyan</code> the <code>background-color</code> cyan.');
  assert(code.match(/\\.raspberry\\s*?{\\s*?background-color:\\s*?#FF007D/gi), 'message: Give the <code>div</code> element with class <code>raspberry</code> the <code>background-color</code> raspberry.');
- Adjusting the Color of Various Elements to Complementary Colors
  assert(code.match(/header\\s*?{\\s*?background-color:\\s*?#09A7A1/gi), 'message: Give your <code>header</code> element the <code>background-color</code> #09A7A1.');
  assert(code.match(/footer\\s*?{\\s*?background-color:\\s*?#09A7A1/gi), 'message: Give your <code>footer</code> element the <code>background-color</code> #09A7A1.');
  assert(code.match(/h2\\s*?{\\s*?color:\\s*?#09A7A1/gi), 'message: Give your <code>h2</code> element the <code>color</code> #09A7A1.');",
  assert(code.match(/button\\s*?{\\s*?background\\-color:\\s*?#FF790E/gi), 'message: Give your <code>button</code> element the <code>background-color</code> #FF790E.');
- Adjust the Hue of a Color
  assert(code.match(/\\.green\\s*?{\\s*?background-color:\\s*?hsl/gi), 'message: Use the <code>hsl()</code> property to declare the color green.');
  assert(code.match(/\\.cyan\\s*?{\\s*?background-color:\\s*?hsl/gi), 'message: Use the <code>hsl()</code> property to declare the color cyan.');
  assert(code.match(/\\.blue\\s*?{\\s*?background-color:\\s*?hsl/gi), 'message: Use the <code>hsl()</code> property to declare the color blue.');
- Adjust the Tone of a Color
  assert(code.match(/nav\\s*?{\\s*?background-color:\\s*?hsl\\(178,\\s*?80%,\\s*?25%\\)/gi), 'message: Give your <code>nav</code> element a <code>background-color</code> of the adjusted teal and make sure to use <code>hsl()</code>.');
- Create a gradual CSS Linear Gradient
- Use a CSS linear gradient to Create a Striped Element
- Create Texture by Adding a Subtle Pattern as a Background Image
- Create a Pattern by Reusing a Block of Elements - NO CHALLENGE

- Use the CSS Transform Scale Property to Change the Size of an Element
- Use the CSS Transform Property to Scale an Element on Hover
- Use the CSS Transform Property SkewX
- Use the CSS Transform Property SkewY
- Create a Graphic Using CSS
- Create a more Complex Shape using CSS and HTML

- Learn How CSS Keyframes and Animation Properties Work
  "assert(code.match(/#rect\\s*?{\\s*?animation-name:\\s*?rainbow;\\s*?animation-duration:\\s*?4s;\\s*?}/gi), 'message: Set the value of the <code>animation-name</code> and <code>animation-duration</code> to rainbow and 4s, respectively, for the <code>#rect</code> element.');"
- Use CSS Animation to Change the Hover State of a Button
- Create Movement Using CSS Animation
- Animate Elements Continually using the Infinity Property
- Make a CSS Heartbeat Using the Infinity Property
  "Note: The code example is using a heart icon via a web framework, which will be covered in a future section. For now, let's focus on the animation aspects of the challenge."
- Animate Elements at Variable Rates
  "Note: The code example is using star icons via a web framework, which will be covered in a future section. For now, let's focus on the animation aspects of the challenge."
- Animate Multiple Elements at Variable Rates
  "Note: The code example is using star icons via a web framework, which will be covered in a future section. For now, let's focus on the animation aspects of the challenge."
- Create Visual Direction by Fading an Element from Left to Right (uses infinite property)
- Use the box-shadow z-axis and Opacity together to Animate an Element - NO CHALLENGE
- Learn how Bezier Curves work
- Use a Bezier Curve to Move a Graphic
  "assert(code.match(/#red\\s*?{\\s*?background:\\s*?red;\\s*?left:\\s*?27%;\\s*?animation-timing-function:\\s*?cubic-bezier\\(0,\\s*?0,\\s*?0?\\.58,\\s*?1\\);/gi), 'message: Set the value of the <code>animation-timing-function</code> property of the element with the id <code>red</code> to a <code>cubic-bezier</code> with  x1, y1, x2, y2 values set respectively to 0, 0, .58, 1 .');"
  "assert(code.match(/#blue\\s*?{\\s*?background:\\s*?blue;\\s*?left:\\s*?56%;\\s*?animation-timing-function:\\s*?ease-out;/gi), 'message: The value of the <code>animation-timing-function</code> property for the <code>blue</code> id should remain as <code>ease-out</code>.');"
- Make Motion more Natural using a Bezier Curve
  "assert(code.match(/#green\\s*?{\\s*?background:\\s*?green;\\s*?left:\\s*?75%;\\s*?animation-timing-function:\\s*?cubic-bezier\\(0?\\.311,\\s*?0?\\.441,\\s*?0?\\.444,\\s*?1\\.649\\);/gi), 'message: Set the value of the <code>animation-timing-function</code> property of the element with the id <code>green</code> to a <code>cubic-bezier</code> with  x1, y1, x2, y2 values set respectively to 0.311, 0.441, 0.444, 1.649.');"
