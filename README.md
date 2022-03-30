# HTML5 Notebook

HTML5 introduces more descriptive **HTML tags**.

*These include:*

* Main
* Header
* Footer
* Nav
* Video
* Article
* Section and others.

These tags give a descriptive structure to your HTML, make your HTML easier to read, and help with Search Engine Optimization (SEO) and accessibility.

The **main** HTML5 tag helps search engines and other developers find the main content of your page

### Add Images to Your Website

You can add images to your website by using the `img` element, and point to a specific image's URL using the `src` attribute

```html
<img src="https://www.freecatphotoapp.com/your-image.jpg">
```

*Notes:*

* All `img` elements **must** have an `alt` attribute.
* The text inside an `alt` attribute is used for screen readers to improve accessibility and is displayed if the image fails to load.
* If the image is purely decorative, using an empty `alt` attribute is a best practice.
* Ideally the `alt` attribute should not contain special characters unless needed.

*For example:*

```html
<img src="https://www.freecatphotoapp.com/your-image.jpg" alt="A business cat wearing a necktie.">
```
