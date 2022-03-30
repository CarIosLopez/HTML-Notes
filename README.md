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

### Link to External Pages with Anchor Elements

You can use **`a`** (anchor) elements to link to content outside of your web page. 

Notes:

* `a` elements need a destination web address called an `href` attribute. They also need anchor text.

  Here's an example:

  ```html
  <a href="https://www.freecodecamp.org">this links to freecodecamp.org</a>
  ```

  Then your browser will display the text `this links to freecodecamp.org` as a link you can click. And that link will take you to the web address `https://www.freecodecamp.org`..


### Link to Internal Sections of a Page with Anchor Elements

`a` (anchor) elements can also be used to create internal links to jump to different sections within a webpage.

Notes: 

* To create an internal link, you assign a link's `href` attribute to a hash symbol `#` plus the value of the `id` attribute for the element that you want to internally link to, usually further down the page.
* You then need to add the same `id` attribute to the element you are linking to.
* An `id` **is an attribute that uniquely describes an element.**

  Below is an example of an internal anchor link and its target element:

  ```html
  <a href="#contacts-header">Contacts</a>
  ...
  <h2 id="contacts-header">Contacts</h2>
  ```

When users click the `Contacts` link, they'll be taken to the section of the webpage with the **Contacts** heading element.


### Link in a New Page

`target="_blank"` attribute from the anchor tag since this causes the linked document to open in a new window tab.
