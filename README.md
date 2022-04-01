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

### Nest an Anchor Element within a Paragraph

You can nest links within other text elements.

```html
<p>
  Here's a <a target="_blank" href="https://www.freecodecamp.org"> link to www.freecodecamp.org</a> for you to follow.
</p>
```

Let's break down the example. Normal text is wrapped in the `p` element:

```html
<p> Here's a ... for you to follow. </p>
```

Next is the *anchor* element `<a>` (which requires a closing tag `</a>`):

```html
<a> ... </a>
```

`target` is an anchor tag attribute that specifies where to open the link. The value `_blank` specifies to open the link in a new tab. The `href` is an anchor tag attribute that contains the URL address of the link:

```html
<a href="https://www.freecodecamp.org" target="_blank"> ... </a>
```

The text, `link to www.freecodecamp.org`, within the `a` element is called anchor text, and will display the link to click:

```html
<a href=" ... " target="...">link to freecodecamp.org</a>
```

The final output of the example will look like this:

**Here's a [link to www.freecodecamp.org](https://www.freecodecamp.org/) for you to follow.**

### Make Dead Links Using the Hash Symbol

Sometimes you want to add `a` elements to your website before you know where they will link.

This is also handy when you're changing the behavior of a link using `JavaScript`, which we'll learn about later.

### Turn an Image into a Link

You can make elements into links by nesting them within an `a` element.

Nest your image within an `a` element. Here's an example:

```html
<a href="#"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="Three kittens running towards the camera."></a>
```

Remember to use `#` as your `a` element's `href` property in order to turn it into a dead link.

### Create a Bulleted Unordered List

HTML has a special element for creating unordered lists, or bullet point style lists.

Unordered lists start with an opening `<ul>` element, followed by any number of `<li>` elements. Finally, unordered lists close with a `</ul>`.

For example:

```html
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```

would create a bullet point style list of `milk` and `cheese`.


### Create an Ordered List

HTML has another special element for creating ordered lists, or numbered lists.

Ordered lists start with an opening `<ol>` element, followed by any number of `<li>` elements. Finally, ordered lists are closed with the `</ol>` tag.

For example:

```html
<ol>
  <li>Garfield</li>
  <li>Sylvester</li>
</ol>
```



### Create a Text Field

Now let's create a web form.

`input` elements are a convenient way to get input from your user.

You can create a text input like this:

```html
<input type="text">
```

Note that `input` elements are self-closing.
