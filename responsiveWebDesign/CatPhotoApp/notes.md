# Responsive Web Design

# Section 1:

HTML: Content

CSS: Design

## Elements:

It’s a document component which has starting tag, ending tag and attributes. It is used to add content to the HTML. e.g. `<h1>`, `<h2>`, `<h3>`, `<p>`

`<h1>` to `<h6>`  These are used for headlines, h1 is the largest(most important) and h6 is the smalles(least important) in the text.

`<p>`  These are used for paragraph

`<main>`  These are used to specify the **********main********** section

`<img>`  These are used to include images, it is a self-closing tag

```
💡 Self-Closing: These are not needed to be closed by a closing tag. So, there is no use for </tag>
```

### Attributes:

These are to add aditional functionality to the HTML elements. e.g `src`, `alt` 

`src`  this attribute is for the source of an image

`alt`  this attribute is for an alternative text for the image

`<a>`  these are used for anchor link

`href` this attribute is for to add the link

`target` this attribute for where to open the URL linked in the anchor link

`<section>` these are used to divide the content of a web page in multiple section (adding a new lower rank `h` makes it seem like a new sub-section)

`<ul>` these are used for unordered lists

`<li>` these are for listing items

`<figure>` for marking a photo section

`<figcaption>` for adding caption for a figure

`<em>` for emphasizing a text

`<ol>` for ordered list [usually numbered]

`<strong>` for text to make it stronger or more important

`<form>` for collecting infromation from user

`action` to specify where form data should be sent

`<input>` for collecting data from user [self-closing]

`type` to set the different type for input element

`name` to set the name of the input

`placeholder` to set text for it to appear when it has no value in it

`required` to prevent from user submitting a blank answer

`<button>` to create a clickable button

Adding `type="submit"` in `<button>` makes it clear that it is a submit button

`<label>` these are used to assoicate a text with an input element

`id` for identifying specific elements, the value for this attribute must be unique

```
💡 alternative way to associate a text with an input element is to add `<label>` nested inside the `<input>` adding a new attribute `for` with same value of `id`
```

adding the same name attribute inside `<input>` makes the choice for radio button as unique

`<fieldset>` it is used for setting related inputs and labels into a block

`<legend>` it is used to add caption into a fieldset

## Handwritten Notes:

![notes_1.jpeg](/responsiveWebDesign/Section1/notes_img/notes_1.jpeg)

![notes_2.jpeg](/responsiveWebDesign/Section1/notes_img/notes_2.jpeg)

![notes_3.jpeg](/responsiveWebDesign/Section1/notes_img/notes_3.jpeg)

![notes_4.jpeg](/responsiveWebDesign/Section1/notes_img/notes_4.jpeg)

(*Yes, I’m aware of my bad hand-writting. In the process to improve it, thank you*)

CatPhotoApp.html

```html
<!DOCTYPE html>

<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>CatPhotoApp</title>
  </head>
  <body>
    <main>
      <h1>CatPhotoApp</h1>
      <section>
        <h2>Cat Photos</h2>
        <!-- TODO: Add link to cat photos -->
        <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
      </section>
      <section>
        <h2>Cat Lists</h2>
        <h3>Things cats love:</h3>
        <ul>
          <li>cat nip</li>
          <li>laser pointers</li>
          <li>lasagna</li>
        </ul>
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
          <figcaption>Cats <em>love</em> lasagna.</figcaption>  
        </figure>
        <h3>Top 3 things cats hate:</h3>
        <ol>
          <li>flea treatment</li>
          <li>thunder</li>
          <li>other cats</li>
        </ol>
        <figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Five cats looking around a field.">
          <figcaption>Cats <strong>hate</strong> other cats.</figcaption>  
        </figure>
      </section>
      <section>
        <h2>Cat Form</h2>
        <form action="https://freecatphotoapp.com/submit-cat-photo">
          <fieldset>
            <legend>Is your cat an indoor or outdoor cat?</legend>
            <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>
            <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
          </fieldset>
          <fieldset>
            <legend>What's your cat's personality?</legend>
            <input id="loving" type="checkbox" name="personality" value="loving" checked> <label for="loving">Loving</label>
            <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
            <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic">Energetic</label>
          </fieldset>
          <input type="text" name="catphotourl" placeholder="cat photo URL" required>
          <button type="submit">Submit</button>
        </form>
      </section>
    </main>
    <footer>
      <p>
        No Copyright - <a href="https://www.freecodecamp.org">freeCodeCamp.org</a>
      </p>
    </footer>
  </body>
</html>
```
