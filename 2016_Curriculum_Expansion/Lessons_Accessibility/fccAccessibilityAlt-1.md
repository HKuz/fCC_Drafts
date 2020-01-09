# Add Alt Text to Images for Visually Impaired Accessibility

## Challenge Description

It's likely you've seen an `alt` attribute on an `img` tag in other challenges. `Alt` text describes the content of the image and provides a text-alternative in case the image fails to load or can't be seen by a user. It's also used by search engines to understand what an image contains to include it in search results. Here's an example:

`<img src="importantLogo.jpeg" alt="Company logo">`

People with visual impairments rely on screen readers to convert web content to an audio interface, and won't get information if it's only presented visually. For images, screen readers can access the `alt` attribute and read its contents to deliver key information.

Good `alt` text is concise but descriptive, and meant to briefly convey the relevant meaning of the image. When should you include an `alt` attribute on your image? Always! Per HTML5 specification, this is now considered mandatory.

## Instructions

CamperCat happens to be both a coding ninja and an actual ninja, and is building a website to share his knowledge. The profile picture he wants to use showcases his skills, and should be appreciated by all site visitors. Add an `alt` attribute in the `img` tag, that explains CamperCat is doing karate in the image.

## Challenge Seed

```
<img src="doingKarateWow.jpeg">
```

## Challenge Tests

```
assert($('img').attr('alt'), 'message: Give the <code>img</code> tag an <code>alt</code> attribute, and make sure it is not empty.');
```

## Challenge Solution

```
<img src="doingKarateWow.jpeg" alt="CamperCat doing karate">
```
