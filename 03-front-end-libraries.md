
# Bootstrap
# 1. Use Responsive Design with Bootstrap Fluid Containers

## Description
<section id='description'>
In the HTML5 and CSS section of freeCodeCamp we built a Cat Photo App. Now let's go back to it. This time, we'll style it using the popular Bootstrap responsive CSS framework.
Bootstrap will figure out how wide your screen is and respond by resizing your HTML elements - hence the name <code>Responsive Design</code>.
With responsive design, there is no need to design a mobile version of your website. It will look good on devices with screens of any width.
You can add Bootstrap to any app by adding the following code to the top of your HTML:
<code>&#60;link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous"/&#62;</code>
In this case, we've already added it for you to this page behind the scenes. Note that using either <code>></code> or <code>/></code> to close the <code>link</code> tag is acceptable.
To get started, we should nest all of our HTML (except the <code>link</code> tag and the <code>style</code> element) in a <code>div</code> element with the class <code>container-fluid</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<h2 class="red-text">CatPhotoApp</h2>

<p>Click here for <a href="#">cat photos</a>.</p>

<a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

<p>Things cats love:</p>
<ul>
  <li>cat nip</li>
  <li>laser pointers</li>
  <li>lasagna</li>
</ul>
<p>Top 3 things cats hate:</p>
<ol>
  <li>flea treatment</li>
  <li>thunder</li>
  <li>other cats</li>
</ol>
<form action="/submit-cat-photo">
  <label><input type="radio" name="indoor-outdoor"> Indoor</label>
  <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
  <label><input type="checkbox" name="personality"> Loving</label>
  <label><input type="checkbox" name="personality"> Lazy</label>
  <label><input type="checkbox" name="personality"> Crazy</label>
  <input type="text" placeholder="cat photo URL" required>
  <button type="submit">Submit</button>
</form>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 2. Make Images Mobile Responsive

## Description
<section id='description'>
First, add a new image below the existing one. Set its <code>src</code> attribute to <code>https://bit.ly/fcc-running-cats</code>.
It would be great if this image could be exactly the width of our phone's screen.
Fortunately, with Bootstrap, all we need to do is add the <code>img-responsive</code> class to your image. Do this, and the image should perfectly fit the width of your page.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 3. Center Text with Bootstrap

## Description
<section id='description'>
Now that we're using Bootstrap, we can center our heading element to make it look better. All we need to do is add the class <code>text-center</code> to our <code>h2</code> element.
Remember that you can add several classes to the same element by separating each of them with a space, like this:
<code>&#60h2 class="red-text text-center"&#62your text&#60/h2&#62</code>
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```
</section>
<hr>

# 4. Create a Bootstrap Button

## Description
<section id='description'>
Bootstrap has its own styles for <code>button</code> elements, which look much better than the plain HTML ones.
Create a new <code>button</code> element below your large kitten photo. Give it the <code>btn</code> and <code>btn-default</code> classes, as well as the text of "Like".
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">

  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```html
<html>
<head>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>
</head>
<body>
<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">

   <!-- ADD Bootstrap Styled Button -->
  <button class="btn btn-default">Like</button> 

  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
</html>
```

</section>
<hr>

# 5. Create a Block Element Bootstrap Button

## Description
<section id='description'>
Normally, your <code>button</code> elements with the <code>btn</code> and <code>btn-default</code> classes are only as wide as the text that they contain. For example:
<code>&lt;button class="btn btn-default"&gt;Submit&lt;/button&gt;</code>
This button would only be as wide as the word "Submit".
<button class='btn btn-default'>Submit</button>
By making them block elements with the additional class of <code>btn-block</code>, your button will stretch to fill your page's entire horizontal space and any elements following it will flow onto a "new line" below the block.
<code>&lt;button class="btn btn-default btn-block"&gt;Submit&lt;/button&gt;</code>
This button would take up 100% of the available width.
<button class='btn btn-default btn-block'>Submit</button>
Note that these buttons still need the <code>btn</code> class.
Add Bootstrap's <code>btn-block</code> class to your Bootstrap button.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <button class="btn btn-default">Like</button>
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 6. Taste the Bootstrap Button Color Rainbow

## Description
<section id='description'>
The <code>btn-primary</code> class is the main color you'll use in your app. It is useful for highlighting actions you want your user to take.
Replace Bootstrap's <code>btn-default</code> class by <code>btn-primary</code> in your button.
Note that this button will still need the <code>btn</code> and <code>btn-block</code> classes.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <button class="btn btn-default btn-block">Like</button>
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 7. Call out Optional Actions with btn-info

## Description
<section id='description'>
Bootstrap comes with several pre-defined colors for buttons. The <code>btn-info</code> class is used to call attention to optional actions that the user can take.
Create a new block-level Bootstrap button below your "Like" button with the text "Info", and add Bootstrap's <code>btn-info</code> and <code>btn-block</code> classes to it.
Note that these buttons still need the <code>btn</code> and <code>btn-block</code> classes.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <button class="btn btn-block btn-primary">Like</button>
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 8. Warn Your Users of a Dangerous Action with btn-danger

## Description
<section id='description'>
Bootstrap comes with several pre-defined colors for buttons. The <code>btn-danger</code> class is the button color you'll use to notify users that the button performs a destructive action, such as deleting a cat photo.
Create a button with the text "Delete" and give it the class <code>btn-danger</code>.
Note that these buttons still need the <code>btn</code> and <code>btn-block</code> classes.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <button class="btn btn-block btn-primary">Like</button>
  <button class="btn btn-block btn-info">Info</button>
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 9. Use the Bootstrap Grid to Put Elements Side By Side

## Description
<section id='description'>
Bootstrap uses a responsive 12-column grid system, which makes it easy to put elements into rows and specify each element's relative width. Most of Bootstrap's classes can be applied to a <code>div</code> element.
Bootstrap has different column width attributes that it uses depending on how wide the user's screen is. For example, phones have narrow screens, and laptops have wider screens.
Take for example Bootstrap's <code>col-md-*</code> class. Here, <code>md</code> means medium, and <code>*</code> is a number specifying how many columns wide the element should be. In this case, the column width of an element on a medium-sized screen, such as a laptop, is being specified.
In the Cat Photo App that we're building, we'll use <code>col-xs-*</code>, where <code>xs</code> means extra small (like an extra-small mobile phone screen), and <code>*</code> is the number of columns specifying how many columns wide the element should be.
Put the <code>Like</code>, <code>Info</code> and <code>Delete</code> buttons side-by-side by nesting all three of them within one <code>&#60;div class="row"&#62;</code> element, then each of them within a <code>&#60;div class="col-xs-4"&#62;</code> element.
The <code>row</code> class is applied to a <code>div</code>, and the buttons themselves can be nested within it.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <button class="btn btn-block btn-primary">Like</button>
  <button class="btn btn-block btn-info">Info</button>
  <button class="btn btn-block btn-danger">Delete</button>
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary">Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info">Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger">Delete</button>
    </div>
  </div>
  
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```
</section>
<hr>

# 10. Ditch Custom CSS for Bootstrap

## Description
<section id='description'>
We can clean up our code and make our Cat Photo App look more conventional by using Bootstrap's built-in styles instead of the custom styles we created earlier.
Don't worry - there will be plenty of time to customize our CSS later.
Delete the <code>.red-text</code>, <code>p</code>, and <code>.smaller-image</code> CSS declarations from your <code>style</code> element so that the only declarations left in your <code>style</code> element are <code>h2</code> and <code>thick-green-border</code>.
Then delete the <code>p</code> element that contains a dead link. Then remove the <code>red-text</code> class from your <code>h2</code> element and replace it with the <code>text-primary</code> Bootstrap class.
Finally, remove the "smaller-image" class from your first <code>img</code> element and replace it with the <code>img-responsive</code> class.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  .red-text {
    color: red;
  }

  h2 {
    font-family: Lobster, Monospace;
  }

  p {
    font-size: 16px;
    font-family: Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

  .smaller-image {
    width: 100px;
  }
</style>

<div class="container-fluid">
  <h2 class="red-text text-center">CatPhotoApp</h2>

  <p>Click here for <a href="#">cat photos</a>.</p>

  <a href="#"><img class="smaller-image thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary">Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info">Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger">Delete</button>
    </div>
  </div>
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 11. Use a span to Target Inline Elements

## Description
<section id='description'>
You can use spans to create inline elements. Remember when we used the <code>btn-block</code> class to make the button fill the entire row?
<button class='btn' style='background-color: rgb(0, 100, 0);  color: rgb(255, 255, 255);'>normal button</button>
<button class='btn btn-block' style='background-color: rgb(0, 100, 0);  color: rgb(255, 255, 255);'>btn-block button</button>
That illustrates the difference between an "inline" element and a "block" element.
By using the inline <code>span</code> element, you can put several elements on the same line, and even style different parts of the same line differently.
Nest the word "love" in your "Things cats love" element below within a <code>span</code> element. Then give that <code>span</code> the class <code>text-danger</code> to make the text red.
Here's how you would do this with the "Top 3 things cats hate" element:
<code>&#60;p&#62;Top 3 things cats &#60;span class="text-danger"&#62;hate:&#60;/span&#62;&#60;/p&#62;</code>
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>

  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

</style>

<div class="container-fluid">
  <h2 class="text-primary text-center">CatPhotoApp</h2>

  <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary">Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info">Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger">Delete</button>
    </div>
  </div>
  <p>Things cats love:</p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 12. Create a Custom Heading

## Description
<section id='description'>
We will make a simple heading for our Cat Photo App by putting the title and relaxing cat image in the same row.
Remember, Bootstrap uses a responsive grid system, which makes it easy to put elements into rows and specify each element's relative width. Most of Bootstrap's classes can be applied to a <code>div</code> element.
Nest your first image and your <code>h2</code> element within a single <code>&#60;div class="row"&#62;</code> element. Nest your <code>h2</code> element within a <code>&#60;div class="col-xs-8"&#62;</code> and your image in a <code>&#60;div class="col-xs-4"&#62;</code> so that they are on the same line.
Notice how the image is now just the right size to fit along the text?
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">

<style>
  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }
</style>

<div class="container-fluid">
  <h2 class="text-primary text-center">CatPhotoApp</h2>

  <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>

  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary">Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info">Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger">Delete</button>
    </div>
  </div>
  <p>Things cats <span class="text-danger">love:</span></p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 13. Add Font Awesome Icons to our Buttons

## Description
<section id='description'>
Font Awesome is a convenient library of icons. These icons are vector graphics, stored in the <code>.svg</code> file format. These icons are treated just like fonts. You can specify their size using pixels, and they will assume the font size of their parent HTML elements.
You can include Font Awesome in any app by adding the following code to the top of your HTML:
<code>&#60;link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.5.0/css/font-awesome.min.css" integrity="sha384-XdYbMnZ/QjLh6iI4ogqCTaIjrFk87ip+ekIjefZch0Y+PvJ8CDYtEs1ipDmPorQ+" crossorigin="anonymous"&#62;</code>
In this case, we've already added it for you to this page behind the scenes.
The <code>i</code> element was originally used to make other elements italic, but is now commonly used for icons. You can add the Font Awesome classes to the <code>i</code> element to turn it into an icon, for example:
<code>&lt;i class="fa fa-info-circle"&gt;&lt;/i&gt;</code>
Note that the <code>span</code> element is also acceptable for use with icons.
Use Font Awesome to add a <code>thumbs-up</code> icon to your like button by giving it an <code>i</code> element with the classes <code>fa</code> and <code>fa-thumbs-up</code>; make sure to keep the text "Like" next to the icon.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }
</style>

<div class="container-fluid">
  <div class="row">
    <div class="col-xs-8">
      <h2 class="text-primary text-center">CatPhotoApp</h2>
    </div>
    <div class="col-xs-4">
      <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
    </div>
  </div>
  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary">Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info">Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger">Delete</button>
    </div>
  </div>
  <p>Things cats <span class="text-danger">love:</span></p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 14. Add Font Awesome Icons to all of our Buttons

## Description
<section id='description'>
Font Awesome is a convenient library of icons. These icons are vector graphics, stored in the <code>.svg</code> file format. These icons are treated just like fonts. You can specify their size using pixels, and they will assume the font size of their parent HTML elements.
Use Font Awesome to add an <code>info-circle</code> icon to your info button and a <code>trash</code> icon to your delete button.
Note: The <code>span</code> element is an acceptable alternative to the <code>i</code> element for the directions below.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }
</style>

<div class="container-fluid">
  <div class="row">
    <div class="col-xs-8">
      <h2 class="text-primary text-center">CatPhotoApp</h2>
    </div>
    <div class="col-xs-4">
      <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
    </div>
  </div>
  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info">Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger">Delete</button>
    </div>
  </div>
  <p>Things cats <span class="text-danger">love:</span></p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 15. Responsively Style Radio Buttons

## Description
<section id='description'>
You can use Bootstrap's <code>col-xs-*</code> classes on <code>form</code> elements, too! This way, our radio buttons will be evenly spread out across the page, regardless of how wide the screen resolution is.
Nest both your radio buttons within a <code>&#60;div class="row"&#62;</code> element. Then nest each of them within a <code>&#60;div class="col-xs-6"&#62;</code> element.
<strong>Note:</strong> As a reminder, radio buttons are <code>input</code> elements of type <code>radio</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }
</style>

<div class="container-fluid">
  <div class="row">
    <div class="col-xs-8">
      <h2 class="text-primary text-center">CatPhotoApp</h2>
    </div>
    <div class="col-xs-4">
      <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
    </div>
  </div>
  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
    </div>
  </div>
  <p>Things cats <span class="text-danger">love:</span></p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <label><input type="radio" name="indoor-outdoor"> Indoor</label>
    <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 16. Responsively Style Checkboxes

## Description
<section id='description'>
  Since Bootstrap's <code>col-xs-*</code> classes are applicable to all <code>form</code> elements, you can use them on your checkboxes too! This way, the checkboxes will be evenly spread out across the page, regardless of how wide the screen resolution is.
</section>

## Instructions
<section id='instructions'>
Nest all three of your checkboxes in a <code>&#60;div class="row"&#62;</code> element. Then nest each of them in a <code>&#60;div class="col-xs-4"&#62;</code> element.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

</style>

<div class="container-fluid">
  <div class="row">
    <div class="col-xs-8">
      <h2 class="text-primary text-center">CatPhotoApp</h2>
    </div>
    <div class="col-xs-4">
      <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
    </div>
  </div>
  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
    </div>
  </div>
  <p>Things cats <span class="text-danger">love:</span></p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <div class="row">
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Indoor</label>
      </div>
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
      </div>
    </div>
    <label><input type="checkbox" name="personality"> Loving</label>
    <label><input type="checkbox" name="personality"> Lazy</label>
    <label><input type="checkbox" name="personality"> Crazy</label>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 17. Style Text Inputs as Form Controls

## Description
<section id='description'>
You can add the <code>fa-paper-plane</code> Font Awesome icon by adding <code>&#60;i class="fa fa-paper-plane"&#62;&#60;/i&#62;</code> within your submit <code>button</code> element.
Give your form's text input field a class of <code>form-control</code>. Give your form's submit button the classes <code>btn btn-primary</code>. Also give this button the Font Awesome icon of <code>fa-paper-plane</code>.
All textual <code>&lt;input&gt;</code>, <code>&lt;textarea&gt;</code>, and <code>&lt;select&gt;</code> elements with the class <code>.form-control</code> have a width of 100%.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

</style>

<div class="container-fluid">
  <div class="row">
    <div class="col-xs-8">
      <h2 class="text-primary text-center">CatPhotoApp</h2>
    </div>
    <div class="col-xs-4">
      <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
    </div>
  </div>
  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
    </div>
  </div>
  <p>Things cats <span class="text-danger">love:</span></p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <div class="row">
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Indoor</label>
      </div>
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Loving</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Lazy</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Crazy</label>
      </div>
    </div>
    <input type="text" placeholder="cat photo URL" required>
    <button type="submit">Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 18. Line up Form Elements Responsively with Bootstrap

## Description
<section id='description'>
Now let's get your form <code>input</code> and your submission <code>button</code> on the same line. We'll do this the same way we have previously: by using a <code>div</code> element with the class <code>row</code>, and other <code>div</code> elements within it using the <code>col-xs-*</code> class.
Nest both your form's text <code>input</code> and submit <code>button</code> within a <code>div</code> with the class <code>row</code>. Nest your form's text <code>input</code> within a div with the class of <code>col-xs-7</code>. Nest your form's submit <code>button</code> in a <code>div</code> with the class <code>col-xs-5</code>.
This is the last challenge we'll do for our Cat Photo App for now. We hope you've enjoyed learning Font Awesome, Bootstrap, and responsive design!
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
<style>
  h2 {
    font-family: Lobster, Monospace;
  }

  .thick-green-border {
    border-color: green;
    border-width: 10px;
    border-style: solid;
    border-radius: 50%;
  }

</style>

<div class="container-fluid">
  <div class="row">
    <div class="col-xs-8">
      <h2 class="text-primary text-center">CatPhotoApp</h2>
    </div>
    <div class="col-xs-4">
      <a href="#"><img class="img-responsive thick-green-border" src="https://bit.ly/fcc-relaxing-cat" alt="A cute orange cat lying on its back."></a>
    </div>
  </div>
  <img src="https://bit.ly/fcc-running-cats" class="img-responsive" alt="Three kittens running towards the camera.">
  <div class="row">
    <div class="col-xs-4">
      <button class="btn btn-block btn-primary"><i class="fa fa-thumbs-up"></i> Like</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-info"><i class="fa fa-info-circle"></i> Info</button>
    </div>
    <div class="col-xs-4">
      <button class="btn btn-block btn-danger"><i class="fa fa-trash"></i> Delete</button>
    </div>
  </div>
  <p>Things cats <span class="text-danger">love:</span></p>
  <ul>
    <li>cat nip</li>
    <li>laser pointers</li>
    <li>lasagna</li>
  </ul>
  <p>Top 3 things cats hate:</p>
  <ol>
    <li>flea treatment</li>
    <li>thunder</li>
    <li>other cats</li>
  </ol>
  <form action="/submit-cat-photo">
    <div class="row">
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Indoor</label>
      </div>
      <div class="col-xs-6">
        <label><input type="radio" name="indoor-outdoor"> Outdoor</label>
      </div>
    </div>
    <div class="row">
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Loving</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Lazy</label>
      </div>
      <div class="col-xs-4">
        <label><input type="checkbox" name="personality"> Crazy</label>
      </div>
    </div>
    <input type="text" class="form-control" placeholder="cat photo URL" required>
    <button type="submit" class="btn btn-primary"><i class="fa fa-paper-plane"></i> Submit</button>
  </form>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 19. Create a Bootstrap Headline

## Description
<section id='description'>
Now let's build something from scratch to practice our HTML, CSS and Bootstrap skills.
We'll build a jQuery playground, which we'll soon put to use in our jQuery challenges.
To start with, create an <code>h3</code> element, with the text <code>jQuery Playground</code>.
Color your <code>h3</code> element with the <code>text-primary</code> Bootstrap class, and center it with the <code>text-center</code> Bootstrap class.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html

```

</div>

</section>

## Solution
<section id='solution'>

```html
<h3 class="text-primary text-center">jQuery Playground</h3>
```

</section>
<hr>

# 20. House our page within a Bootstrap container-fluid div

## Description
<section id='description'>
Now let's make sure all the content on your page is mobile-responsive.
Let's nest your <code>h3</code> element within a <code>div</code> element with the class <code>container-fluid</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<h3 class="text-primary text-center">jQuery Playground</h3>


```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 21. Create a Bootstrap Row

## Description
<section id='description'>
Now we'll create a Bootstrap row for our inline elements.
Create a <code>div</code> element below the <code>h3</code> tag, with a class of <code>row</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>

</div>

```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 22. Split Your Bootstrap Row

## Description
<section id='description'>
Now that we have a Bootstrap Row, let's split it into two columns to house our elements.
Create two <code>div</code> elements within your row, both with the class <code>col-xs-6</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">


  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 23. Create Bootstrap Wells

## Description
<section id='description'>
Bootstrap has a class called <code>well</code> that can create a visual sense of depth for your columns.
Nest one <code>div</code> element with the class <code>well</code> within each of your <code>col-xs-6</code> <code>div</code> elements.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">

    </div>
    <div class="col-xs-6">

    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 24. Add Elements within Your Bootstrap Wells

## Description
<section id='description'>
Now we're several <code>div</code> elements deep on each column of our row. This is as deep as we'll need to go. Now we can add our <code>button</code> elements.
Nest three <code>button</code> elements within each of your <code>well</code> <code>div</code> elements.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">



      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">



      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 25. Apply the Default Bootstrap Button Style

## Description
<section id='description'>
Bootstrap has another button class called <code>btn-default</code>.
Apply both the <code>btn</code> and <code>btn-default</code> classes to each of your <code>button</code> elements.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button></button>
        <button></button>
        <button></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button></button>
        <button></button>
        <button></button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 26. Create a Class to Target with jQuery Selectors

## Description
<section id='description'>
Not every class needs to have corresponding CSS. Sometimes we create classes just for the purpose of selecting these elements more easily using jQuery.
Give each of your <code>button</code> elements the class <code>target</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
        <button class="btn btn-default"></button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 27. Add id Attributes to Bootstrap Elements

## Description
<section id='description'>
Recall that in addition to class attributes, you can give each of your elements an <code>id</code> attribute.
Each id must be unique to a specific element and used only once per page.
Let's give a unique id to each of our <code>div</code> elements of class <code>well</code>.
Remember that you can give an element an id like this:
<code>&#60;div class="well" id="center-well"&#62;</code>
Give the well on the left the id of <code>left-well</code>. Give the well on the right the id of <code>right-well</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <div class="well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 28. Label Bootstrap Wells

## Description
<section id='description'>
For the sake of clarity, let's label both of our wells with their ids.
Above your left-well, inside its <code>col-xs-6</code> <code>div</code> element, add a <code>h4</code> element with the text <code>#left-well</code>.
Above your right-well, inside its <code>col-xs-6</code> <code>div</code> element, add a <code>h4</code> element with the text <code>#right-well</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">

      <div class="well" id="left-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">

      <div class="well" id="right-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 29. Give Each Element a Unique id

## Description
<section id='description'>
We will also want to be able to use jQuery to target each button by its unique id.
Give each of your buttons a unique id, starting with <code>target1</code> and ending with <code>target6</code>.
Make sure that <code>target1</code> to <code>target3</code> are in <code>#left-well</code>, and <code>target4</code> to <code>target6</code> are in <code>#right-well</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
        <button class="btn btn-default target"></button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 30. Label Bootstrap Buttons

## Description
<section id='description'>
Just like we labeled our wells, we want to label our buttons.
Give each of your <code>button</code> elements text that corresponds to its <code>id</code>'s selector.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1"></button>
        <button class="btn btn-default target" id="target2"></button>
        <button class="btn btn-default target" id="target3"></button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4"></button>
        <button class="btn btn-default target" id="target5"></button>
        <button class="btn btn-default target" id="target6"></button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 31. Use Comments to Clarify Code

## Description
<section id='description'>
When we start using jQuery, we will modify HTML elements without needing to actually change them in HTML.
Let's make sure that everyone knows they shouldn't actually modify any of this code directly.
Remember that you can start a comment with <code>&#60;!--</code> and end a comment with <code>--&#62;</code>
Add a comment at the top of your HTML that says <code>Only change code above this line.</code>
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# jQuery
# 1. Learn How Script Tags and Document Ready Work

## Description
<section id='description'>
Now we're ready to learn jQuery, the most popular JavaScript tool of all time.
Before we can start using jQuery, we need to add some things to our HTML.
First, add a <code>script</code> element at the top of your page. Be sure to close it on the following line.
Your browser will run any JavaScript inside a <code>script</code> element, including jQuery.
Inside your <code>script</code> element, add this code: <code>$(document).ready(function() {</code> to your <code>script</code>. Then close it on the following line (still inside your <code>script</code> element) with: <code>});</code>
We'll learn more about <code>functions</code> later. The important thing to know is that code you put inside this <code>function</code> will run as soon as your browser has loaded your page.
This is important because without your <code>document ready function</code>, your code may run before your HTML is rendered, which would cause bugs.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 2. Target HTML Elements with Selectors Using jQuery

## Description
<section id='description'>
Now we have a <code>document ready function</code>.
Now let's write our first jQuery statement. All jQuery functions start with a <code>$</code>, usually referred to as a <code>dollar sign operator</code>, or as <code>bling</code>.
jQuery often selects an HTML element with a <code>selector</code>, then does something to that element.
For example, let's make all of your <code>button</code> elements bounce. Just add this code inside your document ready function:
<code>$("button").addClass("animated bounce");</code>
Note that we've already included both the jQuery library and the Animate.css library in the background so that you can use them in the editor. So you are using jQuery to apply the Animate.css <code>bounce</code> class to your <code>button</code> elements.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 3. Target Elements by Class Using jQuery

## Description
<section id='description'>
You see how we made all of your <code>button</code> elements bounce? We selected them with <code>$("button")</code>, then we added some CSS classes to them with <code>.addClass("animated bounce");</code>.
You just used jQuery's <code>.addClass()</code> function, which allows you to add classes to elements.
First, let's target your <code>div</code> elements with the class <code>well</code> by using the <code>$(".well")</code> selector.
Note that, just like with CSS declarations, you type a <code>.</code> before the class's name.
Then use jQuery's <code>.addClass()</code> function to add the classes <code>animated</code> and <code>shake</code>.
For example, you could make all the elements with the class <code>text-primary</code> shake by adding the following to your <code>document ready function</code>:
<code>$(".text-primary").addClass("animated shake");</code>
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce");
  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 4. Target Elements by id Using jQuery

## Description
<section id='description'>
You can also target elements by their id attributes.
First target your <code>button</code> element with the id <code>target3</code> by using the <code>$("#target3")</code> selector.
Note that, just like with CSS declarations, you type a <code>#</code> before the id's name.
Then use jQuery's <code>.addClass()</code> function to add the classes <code>animated</code> and <code>fadeOut</code>.
Here's how you'd make the <code>button</code> element with the id <code>target6</code> fade out:
<code>$("#target6").addClass("animated fadeOut")</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce");
    $(".well").addClass("animated shake");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 5. Delete Your jQuery Functions

## Description
<section id='description'>
These animations were cool at first, but now they're getting kind of distracting.
Delete all three of these jQuery functions from your <code>document ready function</code>, but leave your <code>document ready function</code> itself intact.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce");
    $(".well").addClass("animated shake");
    $("#target3").addClass("animated fadeOut");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 6. Target the Same Element with Multiple jQuery Selectors

## Description
<section id='description'>
Now you know three ways of targeting elements: by type: <code>$("button")</code>, by class: <code>$(".btn")</code>, and by id <code>$("#target1")</code>.
Although it is possible to add multiple classes in a single <code>.addClass()</code> call, let's add them to the same element in <em>three separate ways</em>.
Using <code>.addClass()</code>, add only one class at a time to the same element, three different ways:
Add the <code>animated</code> class to all elements with type <code>button</code>.
Add the <code>shake</code> class to all the buttons with class <code>.btn</code>.
Add the <code>btn-primary</code> class to the button with id <code>#target1</code>.
<strong>Note</strong><br>You should only be targeting one element and adding only one class at a time. Altogether, your three individual selectors will end up adding the three classes <code>shake</code>, <code>animated</code>, and <code>btn-primary</code> to <code>#target1</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 7. Remove Classes from an Element with jQuery

## Description
<section id='description'>
In the same way you can add classes to an element with jQuery's <code>addClass()</code> function, you can remove them with jQuery's <code>removeClass()</code> function.
Here's how you would do this for a specific button:
<code>$("#target2").removeClass("btn-default");</code>
Let's remove the <code>btn-default</code> class from all of our <code>button</code> elements.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce");
    $(".well").addClass("animated shake");
    $("#target3").addClass("animated fadeOut");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 8. Change the CSS of an Element Using jQuery

## Description
<section id='description'>
We can also change the CSS of an HTML element directly with jQuery.
jQuery has a function called <code>.css()</code> that allows you to change the CSS of an element.
Here's how we would change its color to blue:
<code>$("#target1").css("color", "blue");</code>
This is slightly different from a normal CSS declaration, because the CSS property and its value are in quotes, and separated with a comma instead of a colon.
Delete your jQuery selectors, leaving an empty <code>document ready function</code>.
Select <code>target1</code> and change its color to red.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("button").addClass("animated bounce");
    $(".well").addClass("animated shake");
    $("#target3").addClass("animated fadeOut");
    $("button").removeClass("btn-default");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 9. Disable an Element Using jQuery

## Description
<section id='description'>
You can also change the non-CSS properties of HTML elements with jQuery. For example, you can disable buttons.
When you disable a button, it will become grayed-out and can no longer be clicked.
jQuery has a function called <code>.prop()</code> that allows you to adjust the properties of elements.
Here's how you would disable all buttons:
<code>$("button").prop("disabled", true);</code>
Disable only the <code>target1</code> button.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 10. Change Text Inside an Element Using jQuery

## Description
<section id='description'>
Using jQuery, you can change the text between the start and end tags of an element. You can even change HTML markup.
jQuery has a function called <code>.html()</code> that lets you add HTML tags and text within an element. Any content previously within the element will be completely replaced with the content you provide using this function.
Here's how you would rewrite and emphasize the text of our heading:
<code>$("h3").html("&#60;em&#62;jQuery Playground&#60;/em&#62;");</code>
jQuery also has a similar function called <code>.text()</code> that only alters text without adding tags. In other words, this function will not evaluate any HTML tags passed to it, but will instead treat it as the text you want to replace the existing content with.
Change the button with id <code>target4</code> by emphasizing its text.
Check this <a href="https://developer.mozilla.org/en/docs/Web/HTML/Element/em" target="_blank">link</a> to know more on the difference between <code>&#60;i&#62;</code> and <code>&#60;em&#62;</code> and their uses.
Note that while the <code>&#60;i&#62;</code> tag has traditionally been used to emphasize text, it has since been coopted for use as a tag for icons. The <code>&#60;em&#62;</code> tag is now widely accepted as the tag for emphasis. Either will work for this challenge.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target4").html('<em>#target4</em>');
  });
</script>

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```
</section>
<hr>

# 11. Remove an Element Using jQuery

## Description
<section id='description'>
Now let's remove an HTML element from your page using jQuery.
jQuery has a function called <code>.remove()</code> that will remove an HTML element entirely
Remove element <code>target4</code> from the page by using the <code>.remove()</code> function.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 12. Use appendTo to Move Elements with jQuery

## Description
<section id='description'>
Now let's try moving elements from one <code>div</code> to another.
jQuery has a function called <code>appendTo()</code> that allows you to select HTML elements and append them to another element.
For example, if we wanted to move <code>target4</code> from our right well to our left well, we would use:
<code>$("#target4").appendTo("#left-well");</code>
Move your <code>target2</code> element from your <code>left-well</code> to your <code>right-well</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 13. Clone an Element Using jQuery

## Description
<section id='description'>
In addition to moving elements, you can also copy them from one place to another.
jQuery has a function called <code>clone()</code> that makes a copy of an element.
For example, if we wanted to copy <code>target2</code> from our <code>left-well</code> to our <code>right-well</code>, we would use:
<code>$("#target2").clone().appendTo("#right-well");</code>
Did you notice this involves sticking two jQuery functions together? This is called <code>function chaining</code> and it's a convenient way to get things done with jQuery.
Clone your <code>target5</code> element and append it to your <code>left-well</code>.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 14. Target the Parent of an Element Using jQuery

## Description
<section id='description'>
Every HTML element has a <code>parent</code> element from which it <code>inherits</code> properties.
For example, your <code>jQuery Playground</code> <code>h3</code> element has the parent element of <code>&#60;div class="container-fluid"&#62</code>, which itself has the parent <code>body</code>.
jQuery has a function called <code>parent()</code> that allows you to access the parent of whichever element you've selected.
Here's an example of how you would use the <code>parent()</code> function if you wanted to give the parent element of the <code>left-well</code> element a background color of blue:
<code>$("#left-well").parent().css("background-color", "blue")</code>
Give the parent of the <code>#target1</code> element a background-color of red.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");

  });
</script>

<!-- Only change code above this line. -->

<body>
  <div class="container-fluid">
    <h3 class="text-primary text-center">jQuery Playground</h3>
    <div class="row">
      <div class="col-xs-6">
        <h4>#left-well</h4>
        <div class="well" id="left-well">
          <button class="btn btn-default target" id="target1">#target1</button>
          <button class="btn btn-default target" id="target2">#target2</button>
          <button class="btn btn-default target" id="target3">#target3</button>
        </div>
      </div>
      <div class="col-xs-6">
        <h4>#right-well</h4>
        <div class="well" id="right-well">
          <button class="btn btn-default target" id="target4">#target4</button>
          <button class="btn btn-default target" id="target5">#target5</button>
          <button class="btn btn-default target" id="target6">#target6</button>
        </div>
      </div>
    </div>
  </div>
</body>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 15. Target the Children of an Element Using jQuery

## Description
<section id='description'>
When HTML elements are placed one level below another they are called <code>children</code> of that element. For example, the button elements in this challenge with the text "#target1", "#target2", and "#target3" are all <code>children</code> of the <code>&#60;div class="well" id="left-well"&#62;</code> element.
jQuery has a function called <code>children()</code> that allows you to access the children of whichever element you've selected.
Here's an example of how you would use the <code>children()</code> function to give the children of your <code>left-well</code> element the color <code>blue</code>:
<code>$("#left-well").children().css("color", "blue")</code>
</section>

## Instructions
<section id='instructions'>
Give all the children of your <code>right-well</code> element the color orange.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
    $("#target1").parent().css("background-color", "red");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 16. Target a Specific Child of an Element Using jQuery

## Description
<section id='description'>
You've seen why id attributes are so convenient for targeting with jQuery selectors. But you won't always have such neat ids to work with.
Fortunately, jQuery has some other tricks for targeting the right elements.
jQuery uses CSS Selectors to target elements. The <code>target:nth-child(n)</code> CSS selector allows you to select all the nth elements with the target class or element type.
Here's how you would give the third element in each well the bounce class:
<code>$(".target:nth-child(3)").addClass("animated bounce");</code>
Make the second child in each of your well elements bounce. You must select the elements' children with the <code>target</code> class.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
    $("#target1").parent().css("background-color", "red");
    $("#right-well").children().css("color", "orange");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 17. Target Even Elements Using jQuery

## Description
<section id='description'>
You can also target elements based on their positions using <code>:odd</code> or <code>:even</code> selectors.
Note that jQuery is zero-indexed which means the first element in a selection has a position of 0. This can be a little confusing as, counter-intuitively, <code>:odd</code> selects the second element (position 1), fourth element (position 3), and so on.
Here's how you would target all the odd elements with class <code>target</code> and give them classes:
<code>$(".target:odd").addClass("animated shake");</code>
Try selecting all the even <code>target</code> elements and giving them the classes of <code>animated</code> and <code>shake</code>. Remember that <strong>even</strong> refers to the position of elements with a zero-based system in mind.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
    $("#target1").parent().css("background-color", "red");
    $("#right-well").children().css("color", "orange");
    $("#left-well").children().css("color", "green");
    $(".target:nth-child(2)").addClass("animated bounce");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 18. Use jQuery to Modify the Entire Page

## Description
<section id='description'>
We're done playing with our jQuery playground. Let's tear it down!
jQuery can target the <code>body</code> element as well.
Here's how we would make the entire body fade out: <code> $("body").addClass("animated fadeOut");</code>
But let's do something more dramatic. Add the classes <code>animated</code> and <code>hinge</code> to your <code>body</code> element.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
    $("#target1").parent().css("background-color", "red");
    $("#right-well").children().css("color", "orange");
    $("#left-well").children().css("color", "green");
    $(".target:nth-child(2)").addClass("animated bounce");
    $(".target:even").addClass("animated shake");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# Sass
# 1. Store Data with Sass Variables

## Description
<section id='description'>
One feature of Sass that's different than CSS is it uses variables. They are declared and set to store data, similar to JavaScript.
In JavaScript, variables are defined using the <code>let</code> and <code>const</code> keywords. In Sass, variables start with a <code>$</code> followed by the variable name.
Here are a couple examples:
<blockquote>$main-fonts: Arial, sans-serif;<br>$headings-color: green;<br><br>//To use variables:<br>h1 {<br>&nbsp;&nbsp;font-family: $main-fonts;<br>&nbsp;&nbsp;color: $headings-color;<br>}</blockquote>
One example where variables are useful is when a number of elements need to be the same color. If that color is changed, the only place to edit the code is the variable value.
</section>

## Instructions
<section id='instructions'>
Create a variable <code>$text-color</code> and set it to red. Then change the value of the <code>color</code> property for the <code>.blog-post</code> and <code>h2</code> to the <code>$text-color</code> variable.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style type='text/sass'>


  .header{
    text-align: center;
  }
  .blog-post, h2 {
    color: red;
  }
</style>

<h1 class="header">Learn Sass</h1>
<div class="blog-post">
  <h2>Some random title</h2>
  <p>This is a paragraph with some random text in it</p>
</div>
<div class="blog-post">
  <h2>Header #2</h2>
  <p>Here is some more random text.</p>
</div>
<div class="blog-post">
  <h2>Here is another header</h2>
  <p>Even more random text within a paragraph</p>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 2. Nest CSS with Sass

## Description
<section id='description'>
Sass allows <code>nesting</code> of CSS rules, which is a useful way of organizing a style sheet.
Normally, each element is targeted on a different line to style it, like so:
<blockquote>nav {<br>&nbsp;&nbsp;background-color: red;<br>}<br><br>nav ul {<br>&nbsp;&nbsp;list-style: none;<br>}<br><br>nav ul li {<br>&nbsp;&nbsp;display: inline-block;<br>}</blockquote>
For a large project, the CSS file will have many lines and rules. This is where <code>nesting</code> can help organize your code by placing child style rules within the respective parent elements:
<blockquote>nav {<br>&nbsp;&nbsp;background-color: red;<br><br>&nbsp;&nbsp;ul {<br>&nbsp;&nbsp;&nbsp;&nbsp;list-style: none;<br><br>&nbsp;&nbsp;&nbsp;&nbsp;li {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;display: inline-block;<br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;}<br>}<br></blockquote>
</section>

## Instructions
<section id='instructions'>
Use the <code>nesting</code> technique shown above to re-organize the CSS rules for both children of <code>.blog-post</code> element. For testing purposes, the <code>h1</code> should come before the <code>p</code> element.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style type='text/sass'>
  .blog-post {

  }
  h1 {
    text-align: center;
    color: blue;
  }
  p {
    font-size: 20px;
  }
</style>

<div class="blog-post">
  <h1>Blog Title</h1>
  <p>This is a paragraph</p>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 3. Create Reusable CSS with Mixins

## Description
<section id='description'>
In Sass, a <code>mixin</code> is a group of CSS declarations that can be reused throughout the style sheet.
Newer CSS features take time before they are fully adopted and ready to use in all browsers. As features are added to browsers, CSS rules using them may need vendor prefixes. Consider "box-shadow":
<blockquote>div {<br>&nbsp;&nbsp;-webkit-box-shadow: 0px 0px 4px #fff;<br>&nbsp;&nbsp;-moz-box-shadow: 0px 0px 4px #fff;<br>&nbsp;&nbsp;-ms-box-shadow: 0px 0px 4px #fff;<br>&nbsp;&nbsp;box-shadow: 0px 0px 4px #fff;<br>}</blockquote>
It's a lot of typing to re-write this rule for all the elements that have a <code>box-shadow</code>, or to change each value to test different effects.
<code>Mixins</code> are like functions for CSS. Here is how to write one:
<blockquote>@mixin box-shadow($x, $y, $blur, $c){ <br>&nbsp;&nbsp;-webkit-box-shadow: $x, $y, $blur, $c;<br>&nbsp;&nbsp;-moz-box-shadow: $x, $y, $blur, $c;<br>&nbsp;&nbsp;-ms-box-shadow: $x, $y, $blur, $c;<br>&nbsp;&nbsp;box-shadow: $x, $y, $blur, $c;<br>}</blockquote>
The definition starts with <code>@mixin</code> followed by a custom name. The parameters (the <code>$x</code>, <code>$y</code>, <code>$blur</code>, and <code>$c</code> in the example above) are optional.
Now any time a <code>box-shadow</code> rule is needed, only a single line calling the <code>mixin</code> replaces having to type all the vendor prefixes. A <code>mixin</code> is called with the <code>@include</code> directive:
<blockquote>div {<br>&nbsp;&nbsp;@include box-shadow(0px, 0px, 4px, #fff);<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Write a <code>mixin</code> for <code>border-radius</code> and give it a <code>$radius</code> parameter. It should use all the vendor prefixes from the example. Then use the <code>border-radius</code> <code>mixin</code> to give the <code>#awesome</code> element a border radius of 15px.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style type='text/sass'>



  #awesome {
    width: 150px;
    height: 150px;
    background-color: green;

  }
</style>

<div id="awesome"></div>

```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 4. Use @if and @else to Add Logic To Your Styles

## Description
<section id='description'>
The <code>@if</code> directive in Sass is useful to test for a specific case - it works just like the <code>if</code> statement in JavaScript</code>.
<blockquote>@mixin make-bold($bool) {<br>&nbsp;&nbsp;@if $bool == true {<br>&nbsp;&nbsp;&nbsp;&nbsp;font-weight: bold;<br>&nbsp;&nbsp;}<br>}</blockquote>
And just like in JavaScript, <code>@else if</code> and <code>@else</code> test for more conditions:
<blockquote>@mixin text-effect($val) {<br>&nbsp;&nbsp;@if $val == danger {<br>&nbsp;&nbsp;&nbsp;&nbsp;color: red;<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;@else if $val == alert {<br>&nbsp;&nbsp;&nbsp;&nbsp;color: yellow;<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;@else if $val == success {<br>&nbsp;&nbsp;&nbsp;&nbsp;color: green;<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;@else {<br>&nbsp;&nbsp;&nbsp;&nbsp;color: black;<br>&nbsp;&nbsp;}<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Create a <code>mixin</code> called <code>border-stroke</code> that takes a parameter <code>$val</code>. The <code>mixin</code> should check for the following conditions using <code>@if</code>, <code>@else if</code>, and <code>@else</code>:
<blockquote>light - 1px solid black<br>medium - 3px solid black<br>heavy - 6px solid black</blockquote>
If <code>$val</code> is not <code>light</code>, <code>medium</code>, or <code>heavy</code>, the border should be set to <code>none</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style type='text/sass'>



  #box {
    width: 150px;
    height: 150px;
    background-color: red;
    @include border-stroke(medium);
  }
</style>

<div id="box"></div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 5. Use @for to Create a Sass Loop

## Description
<section id='description'>
The <code>@for</code> directive adds styles in a loop, very similar to a <code>for</code> loop in JavaScript.
<code>@for</code> is used in two ways: "start through end" or "start to end". The main difference is that the "start <b>to</b> end" <em>excludes</em> the end number as part of the count, and "start <b>through</b> end" <em>includes</em> the end number as part of the count.
Here's a start <b>through</b> end example:
<blockquote>@for $i from 1 through 12 {<br>&nbsp;&nbsp;.col-#{$i} { width: 100%/12 * $i; }<br>}</blockquote>
The <code>#{$i}</code> part is the syntax to combine a variable (<code>i</code>) with text to make a string. When the Sass file is converted to CSS, it looks like this:
<blockquote>.col-1 {<br>&nbsp;&nbsp;width: 8.33333%;<br>}<br><br>.col-2 {<br>&nbsp;&nbsp;width: 16.66667%;<br>}<br><br>...<br><br>.col-12 {<br>&nbsp;&nbsp;width: 100%;<br>}</blockquote>
This is a powerful way to create a grid layout. Now you have twelve options for column widths available as CSS classes.
</section>

## Instructions
<section id='instructions'>
Write a <code>@for</code> directive that takes a variable <code>$j</code> that goes from 1 <b>to</b> 6.
It should create 5 classes called <code>.text-1</code> to <code>.text-5</code> where each has a <code>font-size</code> set to 10px multiplied by the index.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style type='text/sass'>



</style>

<p class="text-1">Hello</p>
<p class="text-2">Hello</p>
<p class="text-3">Hello</p>
<p class="text-4">Hello</p>
<p class="text-5">Hello</p>
```

</div>



</section>

## Solution
<section id='solution'>

```html
<style type='text/sass'>

@for $i from 1 through 5 {
  .text-#{$i} { font-size: 10px * $i; }
}

</style>

<p class="text-1">Hello</p>
<p class="text-2">Hello</p>
<p class="text-3">Hello</p>
<p class="text-4">Hello</p>
<p class="text-5">Hello</p>
```

```html
<style type='text/sass'>

@for $i from 1 to 6 {
  .text-#{$i} { font-size: 10px * $i; }
}

</style>

<p class="text-1">Hello</p>
<p class="text-2">Hello</p>
<p class="text-3">Hello</p>
<p class="text-4">Hello</p>
<p class="text-5">Hello</p>
```
</section>
<hr>

# 6. Use @each to Map Over Items in a List

## Description
<section id='description'>
The last challenge showed how the <code>@for</code> directive uses a starting and ending value to loop a certain number of times. Sass also offers the <code>@each</code> directive which loops over each item in a list or map.
On each iteration, the variable gets assigned to the current value from the list or map.
<blockquote>@each $color in blue, red, green {<br>&nbsp;&nbsp;.#{$color}-text {color: $color;}<br>}</blockquote>
A map has slightly different syntax. Here's an example:
<blockquote>$colors: (color1: blue, color2: red, color3: green);<br><br>@each $key, $color in $colors {<br>&nbsp;&nbsp;.#{$color}-text {color: $color;}<br>}</blockquote>
Note that the <code>$key</code> variable is needed to reference the keys in the map. Otherwise, the compiled CSS would have <code>color1</code>, <code>color2</code>... in it.
Both of the above code examples are converted into the following CSS:
<blockquote>.blue-text {<br>&nbsp;&nbsp;color: blue;<br>}<br><br>.red-text {<br>&nbsp;&nbsp;color: red;<br>}<br><br>.green-text {<br>&nbsp;&nbsp;color: green;<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Write an <code>@each</code> directive that goes through a list: <code>blue, black, red</code> and assigns each variable to a <code>.color-bg</code> class, where the "color" part changes for each item.
Each class should set the <code>background-color</code> the respective color.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style type='text/sass'>



  div {
    height: 200px;
    width: 200px;
  }
</style>

<div class="blue-bg"></div>
<div class="black-bg"></div>
<div class="red-bg"></div>
```

</div>

</section>

## Solution
<section id='solution'>

The solution requires using the $color variable twice: once for the class name and once for setting the background color. You can use either the list or map data type.

### List Data type
```html
<style type='text/sass'>

  @each $color in blue, black, red {
    .#{$color}-bg {background-color: $color;}
  }

  div {
    height: 200px;
    width: 200px;
  }
</style>

<div class="blue-bg"></div>
<div class="black-bg"></div>
<div class="red-bg"></div>
```

### Map Data type
```html
<style type='text/sass'>

  $colors: (color1: blue, color2: black, color3: red);

  @each $key, $color in $colors {
    .#{$color}-bg {background-color: $color;}
  }

  div {
    height: 200px;
    width: 200px;
  }
</style>

<div class="blue-bg"></div>
<div class="black-bg"></div>
<div class="red-bg"></div>
```

</section>
<hr>

# 7. Apply a Style Until a Condition is Met with @while

## Description
<section id='description'>
The <code>@while</code> directive is an option with similar functionality to the JavaScript <code>while</code> loop. It creates CSS rules until a condition is met.
The <code>@for</code> challenge gave an example to create a simple grid system. This can also work with <code>@while</code>.
<blockquote>$x: 1;<br>@while $x < 13 {<br>&nbsp;&nbsp;.col-#{$x} { width: 100%/12 * $x;}<br>&nbsp;&nbsp;$x: $x + 1;<br>}</blockquote>
First, define a variable <code>$x</code> and set it to 1. Next, use the <code>@while</code> directive to create the grid system <i>while</i> <code>$x</code> is less than 13.
After setting the CSS rule for <code>width</code>, <code>$x</code> is incremented by 1 to avoid an infinite loop.
</section>

## Instructions
<section id='instructions'>
Use <code>@while</code> to create a series of classes with different <code>font-sizes</code>.
There should be 10 different classes from <code>text-1</code> to <code>text-10</code>. Then set <code>font-size</code> to 5px multiplied by the current index number. Make sure to avoid an infinite loop!
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style type='text/sass'>



</style>

<p class="text-1">Hello</p>
<p class="text-2">Hello</p>
<p class="text-3">Hello</p>
<p class="text-4">Hello</p>
<p class="text-5">Hello</p>
<p class="text-6">Hello</p>
<p class="text-7">Hello</p>
<p class="text-8">Hello</p>
<p class="text-9">Hello</p>
<p class="text-10">Hello</p>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 8. Split Your Styles into Smaller Chunks with Partials

## Description
<section id='description'>
<code>Partials</code> in Sass are separate files that hold segments of CSS code. These are imported and used in other Sass files. This is a great way to group similar code into a module to keep it organized.
Names for <code>partials</code> start with the underscore (<code>_</code>) character, which tells Sass it is a small segment of CSS and not to convert it into a CSS file. Also, Sass files end with the <code>.scss</code> file extension. To bring the code in the <code>partial</code> into another Sass file, use the <code>@import</code> directive.
For example, if all your <code>mixins</code> are saved in a <code>partial</code> named "_mixins.scss", and they are needed in the "main.scss" file, this is how to use them in the main file:
<blockquote>// In the main.scss file<br><br>@import 'mixins'</blockquote>
Note that the underscore is not needed in the <code>import</code> statement - Sass understands it is a <code>partial</code>. Once a <code>partial</code> is imported into a file, all variables, <code>mixins</code>, and other code are available to use.
</section>

## Instructions
<section id='instructions'>
Write an <code>@import</code> statement to import a <code>partial</code> named <code>_variables.scss</code> into the main.scss file.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
// The main.scss file




```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 9. Extend One Set of CSS Styles to Another Element

## Description
<section id='description'>
Sass has a feature called <code>extend</code> that makes it easy to borrow the CSS rules from one element and build upon them in another.
For example, the below block of CSS rules style a <code>.panel</code> class. It has a <code>background-color</code>, <code>height</code> and <code>border</code>.
<blockquote>.panel{<br>&nbsp;&nbsp;background-color: red;<br>&nbsp;&nbsp;height: 70px;<br>&nbsp;&nbsp;border: 2px solid green;<br>}</blockquote>
Now you want another panel called <code>.big-panel</code>. It has the same base properties as <code>.panel</code>, but also needs a <code>width</code> and <code>font-size</code>.
It's possible to copy and paste the initial CSS rules from <code>.panel</code>, but the code becomes repetitive as you add more types of panels.
The <code>extend</code> directive is a simple way to reuse the rules written for one element, then add more for another:
<blockquote>.big-panel{<br>&nbsp;&nbsp;@extend .panel;<br>&nbsp;&nbsp;width: 150px;<br>&nbsp;&nbsp;font-size: 2em;<br>}</blockquote>
The <code>.big-panel</code> will have the same properties as <code>.panel</code> in addition to the new styles.
</section>

## Instructions
<section id='instructions'>
Make a class <code>.info-important</code> that extends <code>.info</code> and also has a <code>background-color</code> set to magenta.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style type='text/sass'>
  h3{
    text-align: center;
  }
  .info{
    width: 200px;
    border: 1px solid black;
    margin: 0 auto;
  }




</style>
<h3>Posts</h3>
<div class="info-important">
  <p>This is an important post. It should extend the class ".info" and have its own CSS styles.</p>
</div>

<div class="info">
  <p>This is a simple post. It has basic styling and can be extended for other uses.</p>
</div>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# React
# 1. Create a Simple JSX Element

## Description
<section id='description'>
<strong>Intro:</strong> React is an Open Source view library created and maintained by Facebook. It's a great tool to render the User Interface (UI) of modern web applications.
React uses a syntax extension of JavaScript called JSX that allows you to write HTML directly within JavaScript. This has several benefits. It lets you use the full programmatic power of JavaScript within HTML, and helps to keep your code readable. For the most part, JSX is similar to the HTML that you have already learned, however there are a few key differences that will be covered throughout these challenges.
For instance, because JSX is a syntactic extension of JavaScript, you can actually write JavaScript directly within JSX. To do this, you simply include the code you want to be treated as JavaScript within curly braces: <code>{ 'this is treated as JavaScript code' }</code>. Keep this in mind, since it's used in several future challenges.
However, because JSX is not valid JavaScript, JSX code must be compiled into JavaScript. The transpiler Babel is a popular tool for this process. For your convenience, it's already added behind the scenes for these challenges. If you happen to write syntactically invalid JSX, you will see the first test in these challenges fail.
It's worth noting that under the hood the challenges are calling <code>ReactDOM.render(JSX, document.getElementById('root'))</code>. This function call is what places your JSX into React's own lightweight representation of the DOM. React then uses snapshots of its own DOM to optimize updating only specific parts of the actual DOM.
</section>

## Instructions
<section id='instructions'>
<strong>Instructions:</strong> The current code uses JSX to assign a <code>div</code> element to the constant <code>JSX</code>. Replace the <code>div</code> with an <code>h1</code> element and add the text <code>Hello JSX!</code> inside it.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

const JSX = <div></div>;

```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(JSX, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const JSX = <h1>Hello JSX!</h1>;
```

</section>
<hr>

# 2. Create a Complex JSX Element

## Description
<section id='description'>
The last challenge was a simple example of JSX, but JSX can represent more complex HTML as well.
One important thing to know about nested JSX is that it must return a single element.
This one parent element would wrap all of the other levels of nested elements.
For instance, several JSX elements written as siblings with no parent wrapper element will not transpile.
Here's an example:
<b>Valid JSX:</b>
<blockquote>&lt;div&gt;<br>&nbsp;&nbsp;&lt;p&gt;Paragraph One&lt;/p&gt;<br>&nbsp;&nbsp;&lt;p&gt;Paragraph Two&lt;/p&gt;<br>&nbsp;&nbsp;&lt;p&gt;Paragraph Three&lt;/p&gt;<br>&lt;/div&gt;</blockquote>
<b>Invalid JSX:</b>
<blockquote>&lt;p&gt;Paragraph One&lt;/p&gt;<br>&lt;p&gt;Paragraph Two&lt;/p&gt;<br>&lt;p&gt;Paragraph Three&lt;/p&gt;<br></blockquote>
</section>

## Instructions
<section id='instructions'>
Define a new constant <code>JSX</code> that renders a <code>div</code> which contains the following elements in order:
An <code>h1</code>, a <code>p</code>, and an unordered list that contains three <code>li</code> items. You can include any text you want within each element.
<strong>Note:</strong>&nbsp;When rendering multiple elements like this, you can wrap them all in parentheses, but it's not strictly required. Also notice this challenge uses a <code>div</code> tag to wrap all the child elements within a single parent element. If you remove the <code>div</code>, the JSX will no longer transpile. Keep this in mind, since it will also apply when you return JSX elements in React components.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
// write your code here

```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(JSX, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const JSX = (
<div>
  <h1>Hello JSX!</h1>
  <p>Some info</p>
  <ul>
    <li>An item</li>
    <li>Another item</li>
    <li>A third item</li>
  </ul>
</div>);
```

</section>
<hr>

# 3. Add Comments in JSX

## Description
<section id='description'>
JSX is a syntax that gets compiled into valid JavaScript. Sometimes, for readability, you might need to add comments to your code. Like most programming languages, JSX has its own way to do this.
To put comments inside JSX, you use the syntax <code>{/* */}</code> to wrap around the comment text.
</section>

## Instructions
<section id='instructions'>
The code editor has a JSX element similar to what you created in the last challenge. Add a comment somewhere within the provided <code>div</code> element, without modifying the existing <code>h1</code> or <code>p</code> elements.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const JSX = (
  <div>
    <h1>This is a block of JSX</h1>
    <p>Here's a subtitle</p>
  </div>
);
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(JSX, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const JSX = (
<div>
  <h1>This is a block of JSX</h1>
  { /* this is a JSX comment */ }
  <p>Here's a subtitle</p>
</div>);
```

</section>
<hr>

# 4. Render HTML Elements to the DOM

## Description
<section id='description'>
So far, you've learned that JSX is a convenient tool to write readable HTML within JavaScript. With React, we can render this JSX directly to the HTML DOM using React's rendering API known as ReactDOM.
ReactDOM offers a simple method to render React elements to the DOM which looks like this: <code>ReactDOM.render(componentToRender, targetNode)</code>, where the first argument is the React element or component that you want to render, and the second argument is the DOM node that you want to render the component to.
As you would expect, <code>ReactDOM.render()</code> must be called after the JSX element declarations, just like how you must declare variables before using them.
</section>

## Instructions
<section id='instructions'>
The code editor has a simple JSX component. Use the <code>ReactDOM.render()</code> method to render this component to the page. You can pass defined JSX elements directly in as the first argument and use <code>document.getElementById()</code> to select the DOM node to render them to. There is a <code>div</code> with <code>id='challenge-node'</code> available for you to use. Make sure you don't change the <code>JSX</code> constant.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const JSX = (
  <div>
    <h1>Hello World</h1>
    <p>Lets render this to the DOM</p>
  </div>
);
// change code below this line

```

</div>



</section>

## Solution
<section id='solution'>


```js
const JSX = (
<div>
  <h1>Hello World</h1>
  <p>Lets render this to the DOM</p>
</div>
);
// change code below this line
ReactDOM.render(JSX, document.getElementById('challenge-node'));
```

</section>
<hr>

# 5. Define an HTML Class in JSX

## Description
<section id='description'>
Now that you're getting comfortable writing JSX, you may be wondering how it differs from HTML.
So far, it may seem that HTML and JSX are exactly the same.
One key difference in JSX is that you can no longer use the word <code>class</code> to define HTML classes. This is because <code>class</code> is a reserved word in JavaScript. Instead, JSX uses <code>className</code>.
In fact, the naming convention for all HTML attributes and event references in JSX become camelCase. For example, a click event in JSX is <code>onClick</code>, instead of <code>onclick</code>. Likewise, <code>onchange</code> becomes <code>onChange</code>. While this is a subtle difference, it is an important one to keep in mind moving forward.
</section>

## Instructions
<section id='instructions'>
Apply a class of <code>myDiv</code> to the <code>div</code> provided in the JSX code.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const JSX = (
  <div>
    <h1>Add a class to this div</h1>
  </div>
);
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(JSX, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const JSX = (
<div className = 'myDiv'>
  <h1>Add a class to this div</h1>
</div>);
```

</section>
<hr>

# 6. Learn About Self-Closing JSX Tags

## Description
<section id='description'>
So far, you’ve seen how JSX differs from HTML in a key way with the use of <code>className</code> vs. <code>class</code> for defining HTML classes.
Another important way in which JSX differs from HTML is in the idea of the self-closing tag.
In HTML, almost all tags have both an opening and closing tag: <code>&lt;div&gt;&lt;/div&gt;</code>; the closing tag always has a forward slash before the tag name that you are closing. However, there are special instances in HTML called “self-closing tags”, or tags that don’t require both an opening and closing tag before another tag can start.
For example the line-break tag can be written as <code>&lt;br&gt;</code> or as <code>&lt;br /&gt;</code>, but should never be written as <code>&lt;br&gt;&lt;/br&gt;</code>, since it doesn't contain any content.
In JSX, the rules are a little different. Any JSX element can be written with a self-closing tag, and every element must be closed. The line-break tag, for example, must always be written as <code>&lt;br /&gt;</code> in order to be valid JSX that can be transpiled. A <code>&lt;div&gt;</code>, on the other hand, can be written as <code>&lt;div /&gt;</code> or <code>&lt;div&gt;&lt;/div&gt;</code>. The difference is that in the first syntax version there is no way to include anything in the <code>&lt;div /&gt;</code>. You will see in later challenges that this syntax is useful when rendering React components.
</section>

## Instructions
<section id='instructions'>
Fix the errors in the code editor so that it is valid JSX and successfully transpiles. Make sure you don't change any of the content - you only need to close tags where they are needed.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const JSX = (
  <div>
    {/* remove comment and change code below this line
    <h2>Welcome to React!</h2> <br >
    <p>Be sure to close all tags!</p>
    <hr >
    remove comment and change code above this line */}
  </div>
);

```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(JSX, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const JSX = (
<div>
  {/* change code below this line */}
  <h2>Welcome to React!</h2> <br />
  <p>Be sure to close all tags!</p>
  <hr />
  {/* change code above this line */}
</div>
);
```

</section>
<hr>

# 7. Create a Stateless Functional Component

## Description
<section id='description'>
Components are the core of React. Everything in React is a component and here you will learn how to create one.
There are two ways to create a React component. The first way is to use a JavaScript function. Defining a component in this way creates a <em>stateless functional component</em>. The concept of state in an application will be covered in later challenges. For now, think of a stateless component as one that can receive data and render it, but does not manage or track changes to that data. (We'll cover the second way to create a React component in the next challenge.)
To create a component with a function, you simply write a JavaScript function that returns either JSX or <code>null</code>. One important thing to note is that React requires your function name to begin with a capital letter. Here's an example of a stateless functional component that assigns an HTML class in JSX:
<blockquote>// After being transpiled, the &lt;div&gt; will have a CSS class of 'customClass'<br>const DemoComponent = function() {<br>&nbsp;&nbsp;return (<br>&nbsp;&nbsp;&nbsp;&nbsp;&lt;div className='customClass' /&gt;<br>&nbsp;&nbsp;);<br>};</blockquote>
Because a JSX component represents HTML, you could put several components together to create a more complex HTML page. This is one of the key advantages of the component architecture React provides. It allows you to compose your UI from many separate, isolated components. This makes it easier to build and maintain complex user interfaces.
</section>

## Instructions
<section id='instructions'>
The code editor has a function called <code>MyComponent</code>. Complete this function so it returns a single <code>div</code> element which contains some string of text.
<strong>Note:</strong>&nbsp;The text is considered a child of the <code>div</code> element, so you will not be able to use a self-closing tag.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const MyComponent = function() {
  // change code below this line



  // change code above this line
}
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const MyComponent = function() {
  // change code below this line
  return (
    <div>
      Demo Solution
    </div>
  );
  // change code above this line
}
```

</section>
<hr>

# 8. Create a React Component

## Description
<section id='description'>
The other way to define a React component is with the ES6 <code>class</code> syntax. In the following example, <code>Kitten</code> extends <code>React.Component</code>:
<blockquote>class Kitten extends React.Component {<br>&nbsp;&nbsp;constructor(props) {<br>&nbsp;&nbsp;&nbsp;&nbsp;super(props);<br>&nbsp;&nbsp;}<br><br>&nbsp;&nbsp;render() {<br>&nbsp;&nbsp;&nbsp;&nbsp;return (<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&lt;h1&gt;Hi&lt;/h1&gt;<br>&nbsp;&nbsp;&nbsp;&nbsp;);<br>&nbsp;&nbsp;}<br>}</blockquote>
This creates an ES6 class <code>Kitten</code> which extends the <code>React.Component</code> class. So the <code>Kitten</code> class now has access to many useful React features, such as local state and lifecycle hooks. Don't worry if you aren't familiar with these terms yet, they will be covered in greater detail in later challenges.
Also notice the <code>Kitten</code> class has a <code>constructor</code> defined within it that calls <code>super()</code>. It uses <code>super()</code> to call the constructor of the parent class, in this case <code>React.Component</code>. The constructor is a special method used during the initialization of objects that are created with the <code>class</code> keyword. It is best practice to call a component's <code>constructor</code> with <code>super</code>, and pass <code>props</code> to both. This makes sure the component is initialized properly. For now, know that it is standard for this code to be included. Soon you will see other uses for the constructor as well as <code>props</code>.
</section>

## Instructions
<section id='instructions'>
<code>MyComponent</code> is defined in the code editor using class syntax. Finish writing the <code>render</code> method so it returns a <code>div</code> element that contains an <code>h1</code> with the text <code>Hello React!</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

class MyComponent extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    // change code below this line



    // change code above this line
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    // change code below this line
    return (
      <div>
        <h1>Hello React!</h1>
      </div>
    );
    // change code above this line
  }
};
```

</section>
<hr>

# 9. Create a Component with Composition

## Description
<section id='description'>
Now we will look at how we can compose multiple React components together. Imagine you are building an App and have created three components, a <code>Navbar</code>, <code>Dashboard</code>, and <code>Footer</code>.
To compose these components together, you could create an <code>App</code> <i>parent</i> component which renders each of these three components as <i>children</i>. To render a component as a child in a React component, you include the component name written as a custom HTML tag in the JSX. For example, in the <code>render</code> method you could write:
<blockquote>return (<br> &lt;App&gt;<br>&nbsp;&nbsp;&lt;Navbar /&gt;<br>&nbsp;&nbsp;&lt;Dashboard /&gt;<br>&nbsp;&nbsp;&lt;Footer /&gt;<br> &lt;/App&gt;<br>)</blockquote>
When React encounters a custom HTML tag that references another component (a component name wrapped in <code>&lt; /&gt;</code> like in this example), it renders the markup for that component in the location of the tag. This should illustrate the parent/child relationship between the <code>App</code> component and the <code>Navbar</code>, <code>Dashboard</code>, and <code>Footer</code>.
</section>

## Instructions
<section id='instructions'>
In the code editor, there is a simple functional component called <code>ChildComponent</code> and a React component called <code>ParentComponent</code>. Compose the two together by rendering the <code>ChildComponent</code> within the <code>ParentComponent</code>. Make sure to close the <code>ChildComponent</code> tag with a forward slash.
<strong>Note:</strong>&nbsp;<code>ChildComponent</code> is defined with an ES6 arrow function because this is a very common practice when using React. However, know that this is just a function. If you aren't familiar with the arrow function syntax, please refer to the JavaScript section.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const ChildComponent = () => {
  return (
    <div>
      <p>I am the child</p>
    </div>
  );
};

class ParentComponent extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h1>I am the parent</h1>
        { /* change code below this line */ }


        { /* change code above this line */ }
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<ParentComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const ChildComponent = () => {
  return (
    <div>
      <p>I am the child</p>
    </div>
  );
};

class ParentComponent extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h1>I am the parent</h1>
        { /* change code below this line */ }
        <ChildComponent />
        { /* change code above this line */ }
      </div>
    );
  }
};
```

</section>
<hr>

# 10. Use React to Render Nested Components

## Description
<section id='description'>
The last challenge showed a simple way to compose two components, but there are many different ways you can compose components with React.
Component composition is one of React's powerful features. When you work with React, it is important to start thinking about your user interface in terms of components like the App example in the last challenge. You break down your UI into its basic building blocks, and those pieces become the components. This helps to separate the code responsible for the UI from the code responsible for handling your application logic. It can greatly simplify the development and maintenance of complex projects.
</section>

## Instructions
<section id='instructions'>
There are two functional components defined in the code editor, called <code>TypesOfFruit</code> and <code>Fruits</code>. Take the <code>TypesOfFruit</code> component and compose it, or <em>nest</em> it, within the <code>Fruits</code> component. Then take the <code>Fruits</code> component and nest it within the <code>TypesOfFood</code> component. The result should be a child component, nested within a parent component, which is nested within a parent component of its own!
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const TypesOfFruit = () => {
  return (
    <div>
      <h2>Fruits:</h2>
      <ul>
        <li>Apples</li>
        <li>Blueberries</li>
        <li>Strawberries</li>
        <li>Bananas</li>
      </ul>
    </div>
  );
};

const Fruits = () => {
  return (
    <div>
      { /* change code below this line */ }

      { /* change code above this line */ }
    </div>
  );
};

class TypesOfFood extends React.Component {
  constructor(props) {
    super(props);
  }

  render() {
    return (
      <div>
        <h1>Types of Food:</h1>
        { /* change code below this line */ }

        { /* change code above this line */ }
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<TypesOfFood />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const TypesOfFruit = () => {
  return (
    <div>
      <h2>Fruits:</h2>
      <ul>
        <li>Apples</li>
        <li>Blueberries</li>
        <li>Strawberries</li>
        <li>Bananas</li>
      </ul>
    </div>
  );
};

const Fruits = () => {
  return (
    <div>
      { /* change code below this line */ }
        <TypesOfFruit />
      { /* change code above this line */ }
    </div>
  );
};

class TypesOfFood extends React.Component {
  constructor(props) {
    super(props);
  }

  render() {
    return (
      <div>
        <h1>Types of Food:</h1>
        { /* change code below this line */ }
        <Fruits />
        { /* change code above this line */ }
      </div>
    );
  }
};
```

</section>
<hr>

# 11. Compose React Components

## Description
<section id='description'>
As the challenges continue to use more complex compositions with React components and JSX, there is one important point to note. Rendering ES6 style class components within other components is no different than rendering the simple components you used in the last few challenges. You can render JSX elements, stateless functional components, and ES6 class components within other components.
</section>

## Instructions
<section id='instructions'>
In the code editor, the <code>TypesOfFood</code> component is already rendering a component called <code>Vegetables</code>. Also, there is the <code>Fruits</code> component from the last challenge.
Nest two components inside of <code>Fruits</code> &mdash; first <code>NonCitrus</code>, and then <code>Citrus</code>. Both of these components are provided for you in the background. Next, nest the <code>Fruits</code> class component into the <code>TypesOfFood</code> component, below the <code>h1</code> header and above <code>Vegetables</code>. The result should be a series of nested components, which uses two different component types.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class Fruits extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h2>Fruits:</h2>
        { /* change code below this line */ }

        { /* change code above this line */ }
      </div>
    );
  }
};

class TypesOfFood extends React.Component {
  constructor(props) {
     super(props);
  }
  render() {
    return (
      <div>
        <h1>Types of Food:</h1>
        { /* change code below this line */ }

        { /* change code above this line */ }
        <Vegetables />
      </div>
    );
  }
};
```

</div>

### Before Test
<div id='jsx-setup'>

```jsx
class NonCitrus extends React.Component {
  render() {
    return (
      <div>
        <h4>Non-Citrus:</h4>
        <ul>
          <li>Apples</li>
          <li>Blueberries</li>
          <li>Strawberries</li>
          <li>Bananas</li>
        </ul>
      </div>
    );
  }
};
class Citrus extends React.Component {
  render() {
    return (
      <div>
        <h4>Citrus:</h4>
        <ul>
          <li>Lemon</li>
          <li>Lime</li>
          <li>Orange</li>
          <li>Grapefruit</li>
        </ul>
      </div>
    );
  }
};
class Vegetables extends React.Component {
  render() {
    return (
      <div>
        <h2>Vegetables:</h2>
        <ul>
          <li>Brussel Sprouts</li>
          <li>Broccoli</li>
          <li>Squash</li>
        </ul>
      </div>
    );
     }
};
```

</div>

### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<TypesOfFood />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class Fruits extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h2>Fruits:</h2>
        { /* change code below this line */ }
        <NonCitrus />
        <Citrus />
        { /* change code above this line */ }
      </div>
    )
  }
}

class TypesOfFood extends React.Component {
  constructor(props) {
     super(props);
  }
    render() {
      return (
        <div>
        <h1>Types of Food:</h1>
          { /* change code below this line */ }
          <Fruits />
          { /* change code above this line */ }
          <Vegetables />
        </div>
      );
    }
};
```

</section>
<hr>

# 12. Render a Class Component to the DOM

## Description
<section id='description'>
You may remember using the ReactDOM API in an earlier challenge to render JSX elements to the DOM. The process for rendering React components will look very similar. The past few challenges focused on components and composition, so the rendering was done for you behind the scenes. However, none of the React code you write will render to the DOM without making a call to the ReactDOM API.
Here's a refresher on the syntax: <code>ReactDOM.render(componentToRender, targetNode)</code>. The first argument is the React component that you want to render. The second argument is the DOM node that you want to render that component within.
React components are passed into <code>ReactDOM.render()</code> a little differently than JSX elements. For JSX elements, you pass in the name of the element that you want to render. However, for React components, you need to use the same syntax as if you were rendering a nested component, for example <code>ReactDOM.render(&lt;ComponentToRender /&gt;, targetNode)</code>. You use this syntax for both ES6 class components and functional components.
</section>

## Instructions
<section id='instructions'>
Both the <code>Fruits</code> and <code>Vegetables</code> components are defined for you behind the scenes. Render both components as children of the <code>TypesOfFood</code> component, then render <code>TypesOfFood</code> to the DOM. There is a <code>div</code> with <code>id='challenge-node'</code> available for you to use.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

class TypesOfFood extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h1>Types of Food:</h1>
        {/* change code below this line */}

        {/* change code above this line */}
      </div>
    );
  }
};

// change code below this line

```

</div>

### Before Test
<div id='jsx-setup'>

```jsx

const Fruits = () => {
  return (
    <div>
      <h2>Fruits:</h2>
      <h4>Non-Citrus:</h4>
        <ul>
          <li>Apples</li>
          <li>Blueberries</li>
          <li>Strawberries</li>
          <li>Bananas</li>
        </ul>
      <h4>Citrus:</h4>
        <ul>
          <li>Lemon</li>
          <li>Lime</li>
          <li>Orange</li>
          <li>Grapefruit</li>
        </ul>
    </div>
  );
};
const Vegetables = () => {
  return (
    <div>
      <h2>Vegetables:</h2>
      <ul>
        <li>Brussel Sprouts</li>
        <li>Broccoli</li>
        <li>Squash</li>
      </ul>
    </div>
  );
};

```

</div>


</section>

## Solution
<section id='solution'>


```js
class TypesOfFood extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h1>Types of Food:</h1>
        {/* change code below this line */}
          <Fruits />
           <Vegetables />
         {/* change code above this line */}
      </div>
    );
  }
};

// change code below this line
ReactDOM.render(<TypesOfFood />, document.getElementById('challenge-node'));
```

</section>
<hr>

# 13. Write a React Component from Scratch

## Description
<section id='description'>
Now that you've learned the basics of JSX and React components, it's time to write a component on your own. React components are the core building blocks of React applications so it's important to become very familiar with writing them. Remember, a typical React component is an ES6 <code>class</code> which extends <code>React.Component</code>. It has a render method that returns HTML (from JSX) or <code>null</code>. This is the basic form of a React component. Once you understand this well, you will be prepared to start building more complex React projects.
</section>

## Instructions
<section id='instructions'>
Define a class <code>MyComponent</code> that extends <code>React.Component</code>. Its render method should return a <code>div</code> that contains an <code>h1</code> tag with the text: <code>My First React Component!</code> in it. Use this text exactly, the case and punctuation matter. Make sure to call the constructor for your component, too.
Render this component to the DOM using <code>ReactDOM.render()</code>. There is a <code>div</code> with <code>id='challenge-node'</code> available for you to use.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
// change code below this line

```

</div>



</section>

## Solution
<section id='solution'>


```js
// change code below this line
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h1>My First React Component!</h1>
      </div>
    );
  }
};

ReactDOM.render(<MyComponent />, document.getElementById('challenge-node'));
```

</section>
<hr>

# 14. Pass Props to a Stateless Functional Component

## Description
<section id='description'>
The previous challenges covered a lot about creating and composing JSX elements, functional components, and ES6 style class components in React. With this foundation, it's time to look at another feature very common in React: <b>props</b>. In React, you can pass props, or properties, to child components. Say you have an <code>App</code> component which renders a child component called <code>Welcome</code> which is a stateless functional component. You can pass <code>Welcome</code> a <code>user</code> property by writing:
<blockquote>&lt;App&gt;<br>&nbsp;&nbsp;&lt;Welcome user='Mark' /&gt;<br>&lt;/App&gt;</blockquote>
You use <strong>custom HTML attributes</strong> created by you and supported by React to be passed to the component. In this case, the created property <code>user</code> is passed to the component <code>Welcome</code>. Since <code>Welcome</code> is a stateless functional component, it has access to this value like so:
<blockquote>const Welcome = (props) => &lt;h1&gt;Hello, {props.user}!&lt;/h1&gt;</blockquote>
It is standard to call this value <code>props</code> and when dealing with stateless functional components, you basically consider it as an argument to a function which returns JSX. You can access the value of the argument in the function body. With class components, you will see this is a little different.
</section>

## Instructions
<section id='instructions'>
There are <code>Calendar</code> and <code>CurrentDate</code> components in the code editor. When rendering <code>CurrentDate</code> from the <code>Calendar</code> component, pass in a property of <code>date</code> assigned to the current date from JavaScript's <code>Date</code> object. Then access this <code>prop</code> in the <code>CurrentDate</code> component, showing its value within the <code>p</code> tags. Note that for <code>prop</code> values to be evaluated as JavaScript, they must be enclosed in curly brackets, for instance <code>date={Date()}</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

const CurrentDate = (props) => {
  return (
    <div>
      { /* change code below this line */ }
      <p>The current date is: </p>
      { /* change code above this line */ }
    </div>
  );
};

class Calendar extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h3>What date is it?</h3>
        { /* change code below this line */ }
        <CurrentDate />
        { /* change code above this line */ }
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<Calendar />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const CurrentDate = (props) => {
  return (
    <div>
      { /* change code below this line */ }
      <p>The current date is: {props.date}</p>
      { /* change code above this line */ }
    </div>
  );
};

class Calendar extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h3>What date is it?</h3>
        { /* change code below this line */ }
        <CurrentDate date={Date()} />
        { /* change code above this line */ }
      </div>
    );
  }
};
```

</section>
<hr>

# 15. Pass an Array as Props

## Description
<section id='description'>
The last challenge demonstrated how to pass information from a parent component to a child component as <code>props</code> or properties. This challenge looks at how arrays can be passed as <code>props</code>.  To pass an array to a JSX element, it must be treated as JavaScript and wrapped in curly braces.
<blockquote>&lt;ParentComponent&gt;<br>&nbsp;&nbsp;&lt;ChildComponent colors={["green", "blue", "red"]} /&gt;<br>&lt;/ParentComponent&gt;</blockquote>
The child component then has access to the array property <code>colors</code>.  Array methods such as <code>join()</code> can be used when accessing the property.
<code>const ChildComponent = (props) => &lt;p&gt{props.colors.join(', ')}&lt;/p&gt</code>
This will join all <code>colors</code> array items into a comma separated string and produce:
 <code> &lt;p&gt;green, blue, red&lt;/p&gt;</code>
Later, we will learn about other common methods to render arrays of data in React.
</section>

## Instructions
<section id='instructions'>
There are <code>List</code> and <code>ToDo</code> components in the code editor. When rendering each <code>List</code> from the <code>ToDo</code> component, pass in a <code>tasks</code> property assigned to an array of to-do tasks, for example <code>["walk dog", "workout"]</code>. Then access this <code>tasks</code> array in the <code>List</code> component, showing its value within the <code>p</code> element.  Use <code>join(", ")</code> to display the <code>props.tasks</code>array in the <code>p</code> element as a comma separated list. Today's list should have at least 2 tasks and tomorrow's should have at least 3 tasks.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const List= (props) => {
  { /* change code below this line */ }
  return <p>{}</p>
  { /* change code above this line */ }
};

class ToDo extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h1>To Do Lists</h1>
        <h2>Today</h2>
        { /* change code below this line */ }
        <List/>
        <h2>Tomorrow</h2>
        <List/>
        { /* change code above this line */ }
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<ToDo />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const List= (props) => {
  return <p>{props.tasks.join(', ')}</p>
};

class ToDo extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h1>To Do Lists</h1>
        <h2>Today</h2>
        <List tasks={['study', 'exercise']} />
        <h2>Tomorrow</h2>
        <List tasks={['call Sam', 'grocery shopping', 'order tickets']} />
      </div>
    );
  }
};
```

</section>
<hr>

# 16. Use Default Props

## Description
<section id='description'>
React also has an option to set default props. You can assign default props to a component as a property on the component itself and React assigns the default prop if necessary. This allows you to specify what a prop value should be if no value is explicitly provided. For example, if you declare <code>MyComponent.defaultProps = { location: 'San Francisco' }</code>, you have defined a location prop that's set to the string <code>San Francisco</code>, unless you specify otherwise. React assigns default props if props are undefined, but if you pass <code>null</code> as the value for a prop, it will remain <code>null</code>.
</section>

## Instructions
<section id='instructions'>
The code editor shows a <code>ShoppingCart</code> component. Define default props on this component which specify a prop <code>items</code> with a value of <code>0</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const ShoppingCart = (props) => {
  return (
    <div>
      <h1>Shopping Cart Component</h1>
    </div>
  )
};
// change code below this line

```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<ShoppingCart />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const ShoppingCart = (props) => {
  return (
    <div>
      <h1>Shopping Cart Component</h1>
    </div>
  )
};

// change code below this line
ShoppingCart.defaultProps = {
  items: 0
}
```

</section>
<hr>

# 17. Override Default Props

## Description
<section id='description'>
The ability to set default props is a useful feature in React. The way to override the default props is to explicitly set the prop values for a component.
</section>

## Instructions
<section id='instructions'>
The <code>ShoppingCart</code> component now renders a child component <code>Items</code>. This <code>Items</code> component has a default prop <code>quantity</code> set to the integer <code>0</code>. Override the default prop by passing in a value of <code>10</code> for <code>quantity</code>.
<strong>Note:</strong>&nbsp;Remember that the syntax to add a prop to a component looks similar to how you add HTML attributes. However, since the value for <code>quantity</code> is an integer, it won't go in quotes but it should be wrapped in curly braces. For example, <code>{100}</code>. This syntax tells JSX to interpret the value within the braces directly as JavaScript.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const Items = (props) => {
  return <h1>Current Quantity of Items in Cart: {props.quantity}</h1>
}

Items.defaultProps = {
  quantity: 0
}

class ShoppingCart extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    { /* change code below this line */ }
    return <Items />
    { /* change code above this line */ }
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<ShoppingCart />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const Items = (props) => {
  return <h1>Current Quantity of Items in Cart: {props.quantity}</h1>
}

Items.defaultProps = {
  quantity: 0
}

class ShoppingCart extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    { /* change code below this line */ }
    return <Items quantity = {10} />
    { /* change code above this line */ }
  }
};
```

</section>
<hr>

# 18. Use PropTypes to Define the Props You Expect

## Description
<section id='description'>
React provides useful type-checking features to verify that components receive props of the correct type. For example, your application makes an API call to retrieve data that you expect to be in an array, which is then passed to a component as a prop. You can set <code>propTypes</code> on your component to require the data to be of type <code>array</code>. This will throw a useful warning when the data is of any other type.
It's considered a best practice to set <code>propTypes</code> when you know the type of a prop ahead of time. You can define a <code>propTypes</code> property for a component in the same way you defined <code>defaultProps</code>. Doing this will check that props of a given key are present with a given type. Here's an example to require the type <code>function</code> for a prop called <code>handleClick</code>:
<code>MyComponent.propTypes = { handleClick: PropTypes.func.isRequired }</code>
In the example above, the <code>PropTypes.func</code> part checks that <code>handleClick</code> is a function. Adding <code>isRequired</code> tells React that <code>handleClick</code> is a required property for that component. You will see a warning if that prop isn't provided. Also notice that <code>func</code> represents <code>function</code>. Among the seven JavaScript primitive types, <code>function</code> and <code>boolean</code> (written as <code>bool</code>) are the only two that use unusual spelling. In addition to the primitive types, there are other types available. For example, you can check that a prop is a React element. Please refer to the [documentation](https://reactjs.org/docs/jsx-in-depth.html#specifying-the-react-element-type) for all of the options.
<strong>Note:</strong> As of React v15.5.0, <code>PropTypes</code> is imported independently from React, like this:
<code>import React, { PropTypes } from 'react';</code>
</section>

## Instructions
<section id='instructions'>
Define <code>propTypes</code> for the <code>Items</code> component to require <code>quantity</code> as a prop and verify that it is of type <code>number</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const Items = (props) => {
  return <h1>Current Quantity of Items in Cart: {props.quantity}</h1>
};

// change code below this line

// change code above this line

Items.defaultProps = {
  quantity: 0
};

class ShoppingCart extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return <Items />
  }
};
```

</div>

### Before Test
<div id='jsx-setup'>

```jsx
var PropTypes = {
  number: { isRequired: true }
};

```

</div>

### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<ShoppingCart />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const Items = (props) => {
  return <h1>Current Quantity of Items in Cart: {props.quantity}</h1>
};

// change code below this line
Items.propTypes = {
  quantity: PropTypes.number.isRequired
};
// change code above this line

Items.defaultProps = {
  quantity: 0
};

class ShoppingCart extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return <Items />
  }
};
```

</section>
<hr>

# 19. Access Props Using this.props

## Description
<section id='description'>
The last several challenges covered the basic ways to pass props to child components. But what if the child component that you're passing a prop to is an ES6 class component, rather than a stateless functional component? The ES6 class component uses a slightly different convention to access props.
Anytime you refer to a class component within itself, you use the <code>this</code> keyword. To access props within a class component, you preface the code that you use to access it with <code>this</code>. For example, if an ES6 class component has a prop called <code>data</code>, you write <code>{this.props.data}</code> in JSX.
</section>

## Instructions
<section id='instructions'>
Render an instance of the <code>ReturnTempPassword</code> component in the parent component <code>ResetPassword</code>. Here, give <code>ReturnTempPassword</code> a prop of <code>tempPassword</code> and assign it a value of a string that is at least 8 characters long. Within the child, <code>ReturnTempPassword</code>, access the <code>tempPassword</code> prop within the <code>strong</code> tags to make sure the user sees the temporary password.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class ReturnTempPassword extends React.Component {
  constructor(props) {
    super(props);

  }
  render() {
    return (
        <div>
            { /* change code below this line */ }
            <p>Your temporary password is: <strong></strong></p>
            { /* change code above this line */ }
        </div>
    );
  }
};

class ResetPassword extends React.Component {
  constructor(props) {
    super(props);

  }
  render() {
    return (
        <div>
          <h2>Reset Password</h2>
          <h3>We've generated a new temporary password for you.</h3>
          <h3>Please reset this password from your account settings ASAP.</h3>
          { /* change code below this line */ }

          { /* change code above this line */ }
        </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<ResetPassword />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class ReturnTempPassword extends React.Component {
  constructor(props) {
    super(props);

  }
  render() {
    return (
        <div>
            <p>Your temporary password is: <strong>{this.props.tempPassword}</strong></p>
        </div>
    );
  }
};

class ResetPassword extends React.Component {
  constructor(props) {
    super(props);

  }
  render() {
    return (
        <div>
          <h2>Reset Password</h2>
          <h3>We've generated a new temporary password for you.</h3>
          <h3>Please reset this password from your account settings ASAP.</h3>
          { /* change code below this line */ }
          <ReturnTempPassword tempPassword="serrPbqrPnzc" />
          { /* change code above this line */ }
        </div>
    );
  }
};
```

</section>
<hr>

# 20. Review Using Props with Stateless Functional Components

## Description
<section id='description'>
Except for the last challenge, you've been passing props to stateless functional components. These components act like pure functions. They accept props as input and return the same view every time they are passed the same props. You may be wondering what state is, and the next challenge will cover it in more detail. Before that, here's a review of the terminology for components.
A <em>stateless functional component</em> is any function you write which accepts props and returns JSX. A <em>stateless component</em>, on the other hand, is a class that extends <code>React.Component</code>, but does not use internal state (covered in the next challenge). Finally, a <em>stateful component</em> is any component that does maintain its own internal state. You may see stateful components referred to simply as components or React components.
A common pattern is to try to minimize statefulness and to create stateless functional components wherever possible. This helps contain your state management to a specific area of your application. In turn, this improves development and maintenance of your app by making it easier to follow how changes to state affect its behavior.
</section>

## Instructions
<section id='instructions'>
The code editor has a <code>CampSite</code> component that renders a <code>Camper</code> component as a child. Define the <code>Camper</code> component and assign it default props of <code>{ name: 'CamperBot' }</code>. Inside the <code>Camper</code> component, render any code that you want, but make sure to have one <code>p</code> element that includes only the <code>name</code> value that is passed in as a <code>prop</code>. Finally, define <code>propTypes</code> on the <code>Camper</code> component to require <code>name</code> to be provided as a prop and verify that it is of type <code>string</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class CampSite extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <Camper/>
      </div>
    );
  }
};
// change code below this line

```

</div>

### Before Test
<div id='jsx-setup'>

```jsx
var PropTypes = {
   string: { isRequired: true }
};
```

</div>

### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<CampSite />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class CampSite extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <Camper/>
      </div>
    );
  }
};
// change code below this line

const Camper = (props) => {
   return (
     <div>
       <p>{props.name}</p>
     </div>
   );
};

Camper.propTypes = {
  name: PropTypes.string.isRequired
};

Camper.defaultProps = {
  name: 'CamperBot'
};

```

</section>
<hr>

# 21. Create a Stateful Component

## Description
<section id='description'>
One of the most important topics in React is <code>state</code>. State consists of any data your application needs to know about, that can change over time. You want your apps to respond to state changes and present an updated UI when necessary. React offers a nice solution for the state management of modern web applications.
You create state in a React component by declaring a <code>state</code> property on the component class in its <code>constructor</code>. This initializes the component with <code>state</code> when it is created. The <code>state</code> property must be set to a JavaScript <code>object</code>. Declaring it looks like this:
<blockquote>this.state = {<br>&nbsp;&nbsp;// describe your state here<br>}</code>
You have access to the <code>state</code> object throughout the life of your component. You can update it, render it in your UI, and pass it as props to child components. The <code>state</code> object can be as complex or as simple as you need it to be. Note that you must create a class component by extending <code>React.Component</code> in order to create <code>state</code> like this.
</section>

## Instructions
<section id='instructions'>
There is a component in the code editor that is trying to render a <code>name</code> property from its <code>state</code>. However, there is no <code>state</code> defined. Initialize the component with <code>state</code> in the <code>constructor</code> and assign your name to a property of <code>name</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

class StatefulComponent extends React.Component {
  constructor(props) {
    super(props);
    // initialize state here

  }
  render() {
    return (
      <div>
        <h1>{this.state.name}</h1>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<StatefulComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class StatefulComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      name: 'freeCodeCamp!'
    }
  }
  render() {
    return (
      <div>
        <h1>{this.state.name}</h1>
      </div>
    );
  }
};
```

</section>
<hr>

# 22. Render State in the User Interface

## Description
<section id='description'>
Once you define a component's initial state, you can display any part of it in the UI that is rendered. If a component is stateful, it will always have access to the data in <code>state</code> in its <code>render()</code> method. You can access the data with <code>this.state</code>.
If you want to access a state value within the <code>return</code> of the render method, you have to enclose the value in curly braces.
<code>State</code> is one of the most powerful features of components in React. It allows you to track important data in your app and render a UI in response to changes in this data. If your data changes, your UI will change. React uses what is called a virtual DOM, to keep track of changes behind the scenes. When state data updates, it triggers a re-render of the components using that data - including child components that received the data as a prop. React updates the actual DOM, but only where necessary. This means you don't have to worry about changing the DOM. You simply declare what the UI should look like.
Note that if you make a component stateful, no other components are aware of its <code>state</code>. Its <code>state</code> is completely encapsulated, or local to that component, unless you pass state data to a child component as <code>props</code>. This notion of encapsulated <code>state</code> is very important because it allows you to write certain logic, then have that logic contained and isolated in one place in your code.
</section>

## Instructions
<section id='instructions'>
In the code editor, <code>MyComponent</code> is already stateful. Define an <code>h1</code> tag in the component's render method which renders the value of <code>name</code> from the component's state.
<strong>Note:</strong>&nbsp;The <code>h1</code> should only render the value from <code>state</code> and nothing else. In JSX, any code you write with curly braces <code>{ }</code> will be treated as JavaScript. So to access the value from <code>state</code> just enclose the reference in curly braces.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      name: 'freeCodeCamp'
    }
  }
  render() {
    return (
      <div>
        { /* change code below this line */ }

        { /* change code above this line */ }
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      name: 'freeCodeCamp'
    }
  }
  render() {
    return (
      <div>
        { /* change code below this line */ }
        <h1>{this.state.name}</h1>
        { /* change code above this line */ }
      </div>
    );
  }
};
```

</section>
<hr>

# 23. Render State in the User Interface Another Way

## Description
<section id='description'>
There is another way to access <code>state</code> in a component. In the <code>render()</code> method, before the <code>return</code> statement, you can write JavaScript directly. For example, you could declare functions, access data from <code>state</code> or <code>props</code>, perform computations on this data, and so on. Then, you can assign any data to variables, which you have access to in the <code>return</code> statement.
</section>

## Instructions
<section id='instructions'>
In the <code>MyComponent</code> render method, define a <code>const</code> called <code>name</code> and set it equal to the name value in the component's <code>state</code>. Because you can write JavaScript directly in this part of the code, you don't have to enclose this reference in curly braces.
Next, in the return statement, render this value in an <code>h1</code> tag using the variable <code>name</code>. Remember, you need to use the JSX syntax (curly braces for JavaScript) in the return statement.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      name: 'freeCodeCamp'
    }
  }
  render() {
    // change code below this line

    // change code above this line
    return (
      <div>
        { /* change code below this line */ }

        { /* change code above this line */ }
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      name: 'freeCodeCamp'
    }
  }
  render() {
    // change code below this line
    const name = this.state.name;
    // change code above this line
    return (
      <div>
        { /* change code below this line */ }
        <h1>{name}</h1>
        { /* change code above this line */ }
      </div>
    );
  }
};
```

</section>
<hr>

# 24. Set State with this.setState

## Description
<section id='description'>
The previous challenges covered component <code>state</code> and how to initialize state in the <code>constructor</code>. There is also a way to change the component's <code>state</code>. React provides a method for updating component <code>state</code> called <code>setState</code>. You call the <code>setState</code> method within your component class like so: <code>this.setState()</code>, passing in an object with key-value pairs. The keys are your state properties and the values are the updated state data. For instance, if we were storing a <code>username</code> in state and wanted to update it, it would look like this:
<blockquote>this.setState({<br>&nbsp;&nbsp;username: 'Lewis'<br>});</blockquote>
React expects you to never modify <code>state</code> directly, instead always use <code>this.setState()</code> when state changes occur. Also, you should note that React may batch multiple state updates in order to improve performance. What this means is that state updates through the <code>setState</code> method can be asynchronous. There is an alternative syntax for the <code>setState</code> method which provides a way around this problem. This is rarely needed but it's good to keep it in mind! Please consult the <a target="_blank" href="https://facebook.github.io/react/docs/state-and-lifecycle.html">React documentation</a> for further details.
</section>

## Instructions
<section id='instructions'>
There is a <code>button</code> element in the code editor which has an <code>onClick()</code> handler. This handler is triggered when the <code>button</code> receives a click event in the browser, and runs the <code>handleClick</code> method defined on <code>MyComponent</code>. Within the <code>handleClick</code> method, update the component <code>state</code> using <code>this.setState()</code>. Set the <code>name</code> property in <code>state</code> to equal the string <code>React Rocks!</code>.
Click the button and watch the rendered state update. Don't worry if you don't fully understand how the click handler code works at this point. It's covered in upcoming challenges.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      name: 'Initial State'
    };
    this.handleClick = this.handleClick.bind(this);
  }
  handleClick() {
    // change code below this line

    // change code above this line
  }
  render() {
    return (
      <div>
        <button onClick={this.handleClick}>Click Me</button>
        <h1>{this.state.name}</h1>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      name: 'Initial State'
    };
    this.handleClick = this.handleClick.bind(this);
  }
  handleClick() {
     // change code below this line
    this.setState({
      name: 'React Rocks!'
    });
    // change code above this line
  }
  render() {
    return (
      <div>
        <button onClick = {this.handleClick}>Click Me</button>
        <h1>{this.state.name}</h1>
      </div>
    );
  }
};
```

</section>
<hr>

# 25. Bind 'this' to a Class Method

## Description
<section id='description'>
In addition to setting and updating <code>state</code>, you can also define methods for your component class. A class method typically needs to use the <code>this</code> keyword so it can access properties on the class (such as <code>state</code> and <code>props</code>) inside the scope of the method. There are a few ways to allow your class methods to access <code>this</code>.
One common way is to explicitly bind <code>this</code> in the constructor so <code>this</code> becomes bound to the class methods when the component is initialized. You may have noticed the last challenge used <code>this.handleClick = this.handleClick.bind(this)</code> for its <code>handleClick</code> method in the constructor. Then, when you call a function like <code>this.setState()</code> within your class method, <code>this</code> refers to the class and will not be <code>undefined</code>.
<strong>Note:</strong>&nbsp;The <code>this</code> keyword is one of the most confusing aspects of JavaScript but it plays an important role in React. Although its behavior here is totally normal, these lessons aren't the place for an in-depth review of <code>this</code> so please refer to other lessons if the above is confusing!
</section>

## Instructions
<section id='instructions'>
The code editor has a component with a <code>state</code> that keeps track of an item count. It also has a method which allows you to increment this item count. However, the method doesn't work because it's using the <code>this</code> keyword that is undefined. Fix it by explicitly binding <code>this</code> to the <code>addItem()</code> method in the component's constructor.
Next, add a click handler to the <code>button</code> element in the render method. It should trigger the <code>addItem()</code> method when the button receives a click event. Remember that the method you pass to the <code>onClick</code> handler needs curly braces because it should be interpreted directly as JavaScript.
Once you complete the above steps you should be able to click the button and see the item count increment in the HTML.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      itemCount: 0
    };
    // change code below this line

    // change code above this line
  }
  addItem() {
    this.setState({
      itemCount: this.state.itemCount + 1
    });
  }
  render() {
    return (
      <div>
        { /* change code below this line */ }
        <button>Click Me</button>
        { /* change code above this line */ }
        <h1>Current Item Count: {this.state.itemCount}</h1>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      itemCount: 0
    };
    this.addItem = this.addItem.bind(this);
  }
  addItem() {
    this.setState({
      itemCount: this.state.itemCount + 1
    });
  }
  render() {
    return (
      <div>
        <button onClick = {this.addItem}>Click Me</button>
        <h1>Current Item Count: {this.state.itemCount}</h1>
      </div>
    );
  }
};
```

</section>
<hr>

# 26. Use State to Toggle an Element

## Description
<section id='description'>
You can use <code>state</code> in React applications in more complex ways than what you've seen so far. One example is to monitor the status of a value, then render the UI conditionally based on this value. There are several different ways to accomplish this, and the code editor shows one method.
</section>

## Instructions
<section id='instructions'>
<code>MyComponent</code> has a <code>visibility</code> property which is initialized to <code>false</code>. The render method returns one view if the value of <code>visibility</code> is true, and a different view if it is false.
Currently, there is no way of updating the <code>visibility</code> property in the component's <code>state</code>. The value should toggle back and forth between true and false. There is a click handler on the button which triggers a class method called <code>toggleVisibility()</code>. Define this method so the <code>state</code> of <code>visibility</code> toggles to the opposite value when the method is called. If <code>visibility</code> is <code>false</code>, the method sets it to <code>true</code>, and vice versa.
Finally, click the button to see the conditional rendering of the component based on its <code>state</code>.
<strong>Hint:</strong>&nbsp;Don't forget to bind the <code>this</code> keyword to the method in the constructor!
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      visibility: false
    };
    // change code below this line

    // change code above this line
  }
  // change code below this line

  // change code above this line
  render() {
    if (this.state.visibility) {
      return (
        <div>
          <button onClick={this.toggleVisibility}>Click Me</button>
          <h1>Now you see me!</h1>
        </div>
      );
    } else {
      return (
        <div>
          <button onClick={this.toggleVisibility}>Click Me</button>
        </div>
      );
    }
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      visibility: false
    };
    this.toggleVisibility = this.toggleVisibility.bind(this);
   }
  toggleVisibility() {
    this.setState({
      visibility: !this.state.visibility
    });
  }
  render() {
    if (this.state.visibility) {
      return (
        <div>
          <button onClick = {this.toggleVisibility}>Click Me</button>
          <h1>Now you see me!</h1>
        </div>
      );
    } else {
      return (
        <div>
          <button onClick = {this.toggleVisibility}>Click Me</button>
        </div>
      );
    }
  }
};
```

</section>
<hr>

# 27. Write a Simple Counter

## Description
<section id='description'>
You can design a more complex stateful component by combining the concepts covered so far. These include initializing <code>state</code>, writing methods that set <code>state</code>, and assigning click handlers to trigger these methods.
</section>

## Instructions
<section id='instructions'>
The <code>Counter</code> component keeps track of a <code>count</code> value in <code>state</code>. There are two buttons which call methods <code>increment()</code> and <code>decrement()</code>. Write these methods so the counter value is incremented or decremented by 1 when the appropriate button is clicked. Also, create a <code>reset()</code> method so when the reset button is clicked, the count is set to 0.
<strong>Note:</strong>&nbsp;Make sure you don't modify the <code>classNames</code> of the buttons. Also, remember to add the necessary bindings for the newly-created methods in the constructor.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class Counter extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
    // change code below this line

    // change code above this line
  }
  // change code below this line

  // change code above this line
  render() {
    return (
      <div>
        <button className='inc' onClick={this.increment}>Increment!</button>
        <button className='dec' onClick={this.decrement}>Decrement!</button>
        <button className='reset' onClick={this.reset}>Reset</button>
        <h1>Current Count: {this.state.count}</h1>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<Counter />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class Counter extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0
    };
  this.increment = this.increment.bind(this);
 this.decrement = this.decrement.bind(this);
 this.reset = this.reset.bind(this);
 }
  reset() {
    this.setState({
      count: 0
    });
  }
  increment() {
    this.setState({
      count: this.state.count + 1
    });
  }
  decrement() {
    this.setState({
      count: this.state.count - 1
    });
  }
  render() {
    return (
      <div>
        <button className='inc' onClick={this.increment}>Increment!</button>
        <button className='dec' onClick={this.decrement}>Decrement!</button>
        <button className='reset' onClick={this.reset}>Reset</button>
        <h1>Current Count: {this.state.count}</h1>
      </div>
    );
  }
};
```

</section>
<hr>

# 28. Create a Controlled Input

## Description
<section id='description'>
Your application may have more complex interactions between <code>state</code> and the rendered UI. For example, form control elements for text input, such as <code>input</code> and <code>textarea</code>, maintain their own state in the DOM as the user types. With React, you can move this mutable state into a React component's <code>state</code>. The user's input becomes part of the application <code>state</code>, so React controls the value of that input field. Typically, if you have React components with input fields the user can type into, it will be a controlled input form.
</section>

## Instructions
<section id='instructions'>
The code editor has the skeleton of a component called <code>ControlledInput</code> to create a controlled <code>input</code> element. The component's <code>state</code> is already initialized with an <code>input</code> property that holds an empty string. This value represents the text a user types into the <code>input</code> field.
First, create a method called <code>handleChange()</code> that has a parameter called <code>event</code>. When the method is called, it receives an <code>event</code> object that contains a string of text from the <code>input</code> element. You can access this string with <code>event.target.value</code> inside the method. Update the <code>input</code> property of the component's <code>state</code> with this new string.
In the render method, create the <code>input</code> element above the <code>h4</code> tag. Add a <code>value</code> attribute which is equal to the <code>input</code> property of the component's <code>state</code>. Then add an <code>onChange()</code> event handler set to the <code>handleChange()</code> method.
When you type in the input box, that text is processed by the <code>handleChange()</code> method, set as the <code>input</code> property in the local <code>state</code>, and rendered as the value in the <code>input</code> box on the page. The component <code>state</code> is the single source of truth regarding the input data.
Last but not least, don't forget to add the necessary bindings in the constructor.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class ControlledInput extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: ''
    };
    // change code below this line

    // change code above this line
  }
  // change code below this line

  // change code above this line
  render() {
    return (
      <div>
        { /* change code below this line */}

        { /* change code above this line */}
        <h4>Controlled Input:</h4>
        <p>{this.state.input}</p>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<ControlledInput />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class ControlledInput extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: ''
    };
    this.handleChange = this.handleChange.bind(this);
  }
  handleChange(event) {
    this.setState({
      input: event.target.value
    });
  }
  render() {
    return (
      <div>
        <input
          value={this.state.input}
          onChange={this.handleChange} />
        <h4>Controlled Input:</h4>

        <p>{this.state.input}</p>
      </div>
    );
  }
};
```

</section>
<hr>

# 29. Create a Controlled Form

## Description
<section id='description'>
The last challenge showed that React can control the internal state for certain elements like <code>input</code> and <code>textarea</code>, which makes them controlled components. This applies to other form elements as well, including the regular HTML <code>form</code> element.
</section>

## Instructions
<section id='instructions'>
The <code>MyForm</code> component is set up with an empty <code>form</code> with a submit handler. The submit handler will be called when the form is submitted.
We've added a button which submits the form. You can see it has the <code>type</code> set to <code>submit</code> indicating it is the button controlling the form. Add the <code>input</code> element in the <code>form</code> and set its <code>value</code> and <code>onChange()</code> attributes like the last challenge. You should then complete the <code>handleSubmit</code> method so that it sets the component state property <code>submit</code> to the current input value in the local <code>state</code>.
<strong>Note:</strong>&nbsp; You also must call <code>event.preventDefault()</code> in the submit handler, to prevent the default form submit behavior which will refresh the web page.
Finally, create an <code>h1</code> tag after the <code>form</code> which renders the <code>submit</code> value from the component's <code>state</code>. You can then type in the form and click the button (or press enter), and you should see your input rendered to the page.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: '',
      submit: ''
    };
    this.handleChange = this.handleChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }
  handleChange(event) {
    this.setState({
      input: event.target.value
    });
  }
  handleSubmit(event) {
    // change code below this line

    // change code above this line
  }
  render() {
    return (
      <div>
        <form onSubmit={this.handleSubmit}>
          { /* change code below this line */ }

          { /* change code above this line */ }
          <button type='submit'>Submit!</button>
        </form>
        { /* change code below this line */ }

        { /* change code above this line */ }
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyForm />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyForm extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: '',
      submit: ''
    };
    this.handleChange = this.handleChange.bind(this);
    this.handleSubmit = this.handleSubmit.bind(this);
  }
  handleChange(event) {
    this.setState({
      input: event.target.value
    });
  }
  handleSubmit(event) {
    event.preventDefault()
    this.setState({
      submit: this.state.input
    });
  }
  render() {
    return (
      <div>
        <form onSubmit={this.handleSubmit}>
          <input
            value={this.state.input}
            onChange={this.handleChange} />
          <button type='submit'>Submit!</button>
        </form>
        <h1>{this.state.submit}</h1>
      </div>
    );
  }
};
```

</section>
<hr>

# 30. Pass State as Props to Child Components

## Description
<section id='description'>
You saw a lot of examples that passed props to child JSX elements and child React components in previous challenges. You may be wondering where those props come from. A common pattern is to have a stateful component containing the <code>state</code> important to your app, that then renders child components. You want these components to have access to some pieces of that <code>state</code>, which are passed in as props.
For example, maybe you have an <code>App</code> component that renders a <code>Navbar</code>, among other components. In your <code>App</code>, you have <code>state</code> that contains a lot of user information, but the <code>Navbar</code> only needs access to the user's username so it can display it. You pass that piece of <code>state</code> to the <code>Navbar</code> component as a prop.
This pattern illustrates some important paradigms in React. The first is <em>unidirectional data flow</em>. State flows in one direction down the tree of your application's components, from the stateful parent component to child components. The child components only receive the state data they need. The second is that complex stateful apps can be broken down into just a few, or maybe a single, stateful component. The rest of your components simply receive state from the parent as props, and render a UI from that state. It begins to create a separation where state management is handled in one part of code and UI rendering in another. This principle of separating state logic from UI logic is one of React's key principles. When it's used correctly, it makes the design of complex, stateful applications much easier to manage.
</section>

## Instructions
<section id='instructions'>
The <code>MyApp</code> component is stateful and renders a <code>Navbar</code> component as a child. Pass the <code>name</code> property in its <code>state</code> down to the child component, then show the <code>name</code> in the <code>h1</code> tag that's part of the <code>Navbar</code> render method.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyApp extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      name: 'CamperBot'
    }
  }
  render() {
    return (
       <div>
         <Navbar /* your code here */ />
       </div>
    );
  }
};

class Navbar extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
    <div>
      <h1>Hello, my name is: {/* your code here */} </h1>
    </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyApp />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyApp extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      name: 'CamperBot'
    }
  }
  render() {
    return (
       <div>
         <Navbar name={this.state.name}/>
       </div>
    );
  }
};
class Navbar extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
    <div>
      <h1>Hello, my name is: {this.props.name}</h1>
    </div>
    );
  }
};
```

</section>
<hr>

# 31. Pass a Callback as Props

## Description
<section id='description'>
You can pass <code>state</code> as props to child components, but you're not limited to passing data. You can also pass handler functions or any method that's defined on a React component to a child component. This is how you allow child components to interact with their parent components. You pass methods to a child just like a regular prop. It's assigned a name and you have access to that method name under <code>this.props</code> in the child component.
</section>

## Instructions
<section id='instructions'>
There are three components outlined in the code editor. The <code>MyApp</code> component is the parent that will render the <code>GetInput</code> and <code>RenderInput</code> child components. Add the <code>GetInput</code> component to the render method in <code>MyApp</code>, then pass it a prop called <code>input</code> assigned to <code>inputValue</code> from <code>MyApp</code>&apos;s <code>state</code>. Also create a prop called <code>handleChange</code> and pass the input handler <code>handleChange</code> to it.
Next, add <code>RenderInput</code> to the render method in <code>MyApp</code>, then create a prop called <code>input</code> and pass the <code>inputValue</code> from <code>state</code> to it. Once you are finished you will be able to type in the <code>input</code> field in the <code>GetInput</code> component, which then calls the handler method in its parent via props. This updates the input in the <code>state</code> of the parent, which is passed as props to both children. Observe how the data flows between the components and how the single source of truth remains the <code>state</code> of the parent component. Admittedly, this example is a bit contrived, but should serve to illustrate how data and callbacks can be passed between React components.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyApp extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      inputValue: ''
    }
    this.handleChange = this.handleChange.bind(this);
  }
  handleChange(event) {
    this.setState({
      inputValue: event.target.value
    });
  }
  render() {
    return (
       <div>
        { /* change code below this line */ }

        { /* change code above this line */ }
       </div>
    );
  }
};

class GetInput extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h3>Get Input:</h3>
        <input
          value={this.props.input}
          onChange={this.props.handleChange}/>
      </div>
    );
  }
};

class RenderInput extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h3>Input Render:</h3>
        <p>{this.props.input}</p>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyApp />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyApp extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      inputValue: ''
    }
  this.handleChange = this.handleChange.bind(this);
  }
  handleChange(event) {
    this.setState({
      inputValue: event.target.value
    });
  }
  render() {
    return (
       <div>
         <GetInput
           input={this.state.inputValue}
           handleChange={this.handleChange}/>
         <RenderInput
           input={this.state.inputValue}/>
       </div>
    );
  }
};

class GetInput extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h3>Get Input:</h3>
        <input
          value={this.props.input}
          onChange={this.props.handleChange}/>
      </div>
    );
  }
};

class RenderInput extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <div>
        <h3>Input Render:</h3>
        <p>{this.props.input}</p>
      </div>
    );
  }
};
```

</section>
<hr>

# 32. Use the Lifecycle Method componentWillMount

## Description
<section id='description'>
React components have several special methods that provide opportunities to perform actions at specific points in the lifecycle of a component. These are called lifecycle methods, or lifecycle hooks, and allow you to catch components at certain points in time. This can be before they are rendered, before they update, before they receive props, before they unmount, and so on. Here is a list of some of the main lifecycle methods:
<code>componentWillMount()</code>
<code>componentDidMount()</code>
<code>componentWillReceiveProps()</code>
<code>shouldComponentUpdate()</code>
<code>componentWillUpdate()</code>
<code>componentDidUpdate()</code>
<code>componentWillUnmount()</code>
The next several lessons will cover some of the basic use cases for these lifecycle methods.
  
##### Note: The ``` componentWillMount ``` Lifecycle method will be deprecated in a future version of 16.X and removed in version 17. [(Source)](https://reactjs.org/blog/2018/03/27/update-on-async-rendering.html)
</section>

## Instructions
<section id='instructions'>
The <code>componentWillMount()</code> method is called before the <code>render()</code> method when a component is being mounted to the DOM. Log something to the console within <code>componentWillMount()</code> - you may want to have your browser console open to see the output.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
  }
  componentWillMount() {
    // change code below this line

    // change code above this line
  }
  render() {
    return <div />
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
  }
  componentWillMount() {
    // change code below this line
    console.log('Component is mounting...');
    // change code above this line
  }
  render() {
    return <div />
  }
};
```

</section>
<hr>

# 33. Use the Lifecycle Method componentDidMount

## Description
<section id='description'>
Most web developers, at some point, need to call an API endpoint to retrieve data. If you're working with React, it's important to know where to perform this action.
The best practice with React is to place API calls or any calls to your server in the lifecycle method <code>componentDidMount()</code>. This method is called after a component is mounted to the DOM. Any calls to <code>setState()</code> here will trigger a re-rendering of your component. When you call an API in this method, and set your state with the data that the API returns, it will automatically trigger an update once you receive the data.
</section>

## Instructions
<section id='instructions'>
There is a mock API call in <code>componentDidMount()</code>. It sets state after 2.5 seconds to simulate calling a server to retrieve data. This example requests the current total active users for a site. In the render method, render the value of <code>activeUsers</code> in the <code>h1</code>. Watch what happens in the preview, and feel free to change the timeout to see the different effects.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      activeUsers: null
    };
  }
  componentDidMount() {
    setTimeout( () => {
      this.setState({
        activeUsers: 1273
      });
    }, 2500);
  }
  render() {
    return (
      <div>
        <h1>Active Users: { /* change code here */ }</h1>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      activeUsers: null
    };
  }
  componentDidMount() {
    setTimeout( () => {
      this.setState({
        activeUsers: 1273
      });
    }, 2500);
  }
  render() {
    return (
      <div>
        <h1>Active Users: {this.state.activeUsers}</h1>
      </div>
    );
  }
};
```

</section>
<hr>

# 34. Add Event Listeners

## Description
<section id='description'>
The <code>componentDidMount()</code> method is also the best place to attach any event listeners you need to add for specific functionality. React provides a synthetic event system which wraps the native event system present in browsers. This means that the synthetic event system behaves exactly the same regardless of the user's browser - even if the native events may behave differently between different browsers.
You've already been using some of these synthetic event handlers such as <code>onClick()</code>. React's synthetic event system is great to use for most interactions you'll manage on DOM elements. However, if you want to attach an event handler to the document or window objects, you have to do this directly.
</section>

## Instructions
<section id='instructions'>
Attach an event listener in the <code>componentDidMount()</code> method for <code>keydown</code> events and have these events trigger the callback <code>handleKeyPress()</code>. You can use <code>document.addEventListener()</code> which takes the event (in quotes) as the first argument and the callback as the second argument.
Then, in <code>componentWillUnmount()</code>, remove this same event listener. You can pass the same arguments to <code>document.removeEventListener()</code>. It's good practice to use this lifecycle method to do any clean up on React components before they are unmounted and destroyed. Removing event listeners is an example of one such clean up action.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      message: ''
    };
    this.handleEnter = this.handleEnter.bind(this);
    this.handleKeyPress = this.handleKeyPress.bind(this);
  }
  // change code below this line
  componentDidMount() {

  }
  componentWillUnmount() {

  }
  // change code above this line
  handleEnter() {
    this.setState({
      message: this.state.message + 'You pressed the enter key! '
    });
  }
  handleKeyPress(event) {
    if (event.keyCode === 13) {
      this.handleEnter();
    }
  }
  render() {
    return (
      <div>
        <h1>{this.state.message}</h1>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      message: ''
    };
    this.handleKeyPress = this.handleKeyPress.bind(this);
    this.handleEnter = this.handleEnter.bind(this);  }
  componentDidMount() {
    // change code below this line
    document.addEventListener('keydown', this.handleKeyPress);
    // change code above this line
  }
  componentWillUnmount() {
    // change code below this line
    document.removeEventListener('keydown', this.handleKeyPress);
    // change code above this line
  }
  handleEnter() {
    this.setState({
      message: this.state.message + 'You pressed the enter key! '
    });
  }
  handleKeyPress(event) {
    if (event.keyCode === 13) {
      this.handleEnter();
    }
  }
  render() {
    return (
      <div>
        <h1>{this.state.message}</h1>
      </div>
    );
  }
};
```

</section>
<hr>

# 35. Manage Updates with Lifecycle Methods

## Description
<section id='description'>
Another lifecycle method is <code>componentWillReceiveProps()</code> which is called whenever a component is receiving new props. This method receives the new props as an argument, which is usually written as <code>nextProps</code>. You can use this argument and compare with <code>this.props</code> and perform actions before the component updates. For example, you may call <code>setState()</code> locally before the update is processed.
Another method is <code>componentDidUpdate()</code>, and is called immediately after a component re-renders. Note that rendering and mounting are considered different things in the component lifecycle. When a page first loads, all components are mounted and this is where methods like <code>componentWillMount()</code> and <code>componentDidMount()</code> are called. After this, as state changes, components re-render themselves. The next challenge covers this in more detail.
</section>

## Instructions
<section id='instructions'>
The child component <code>Dialog</code> receives <code>message</code> props from its parent, the <code>Controller</code> component. Write the <code>componentWillReceiveProps()</code> method in the <code>Dialog</code> component and have it log <code>this.props</code> and <code>nextProps</code> to the console. You'll need to pass <code>nextProps</code> as an argument to this method and although it's possible to name it anything, name it <code>nextProps</code> here.
Next, add <code>componentDidUpdate()</code> in the <code>Dialog</code> component, and log a statement that says the component has updated. This method works similar to <code>componentWillUpdate()</code>, which is provided for you. Now click the button to change the message and watch your browser console. The order of the console statements show the order the methods are called.
<strong>Note:</strong>&nbsp;You'll need to write the lifecycle methods as normal functions and not as arrow functions to pass the tests (there is also no advantage to writing lifecycle methods as arrow functions).
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class Dialog extends React.Component {
  constructor(props) {
    super(props);
  }
  componentWillUpdate() {
    console.log('Component is about to update...');
  }
  // change code below this line

  // change code above this line
  render() {
    return <h1>{this.props.message}</h1>
  }
};

class Controller extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      message: 'First Message'
    };
    this.changeMessage = this.changeMessage.bind(this);
  }
  changeMessage() {
    this.setState({
      message: 'Second Message'
    });
  }
  render() {
    return (
      <div>
        <button onClick={this.changeMessage}>Update</button>
        <Dialog message={this.state.message}/>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<Controller />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class Dialog extends React.Component {
  constructor(props) {
    super(props);
  }
  componentWillUpdate() {
    console.log('Component is about to update...');
  }
  // change code below this line
  componentWillReceiveProps(nextProps) {
    console.log(this.props, nextProps);
  }
  componentDidUpdate() {
    console.log('Component re-rendered');
  }
  // change code above this line
  render() {
    return <h1>{this.props.message}</h1>
  }
};

class Controller extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      message: 'First Message'
    };
 this.changeMessage = this.changeMessage.bind(this);
  }
  changeMessage() {
    this.setState({
      message: 'Second Message'
    });
  }
  render() {
    return (
      <div>
        <button onClick={this.changeMessage}>Update</button>
        <Dialog message={this.state.message}/>
      </div>
    );
  }
};
```

</section>
<hr>

# 36. Optimize Re-Renders with shouldComponentUpdate

## Description
<section id='description'>
So far, if any component receives new <code>state</code> or new <code>props</code>, it re-renders itself and all its children. This is usually okay. But React provides a lifecycle method you can call when child components receive new <code>state</code> or <code>props</code>, and declare specifically if the components should update or not. The method is <code>shouldComponentUpdate()</code>, and it takes <code>nextProps</code> and <code>nextState</code> as parameters.
This method is a useful way to optimize performance. For example, the default behavior is that your component re-renders when it receives new <code>props</code>, even if the <code>props</code> haven't changed. You can use <code>shouldComponentUpdate()</code> to prevent this by comparing the <code>props</code>. The method must return a <code>boolean</code> value that tells React whether or not to update the component. You can compare the current props (<code>this.props</code>) to the next props (<code>nextProps</code>) to determine if you need to update or not, and return <code>true</code> or <code>false</code> accordingly.
</section>

## Instructions
<section id='instructions'>
The <code>shouldComponentUpdate()</code> method is added in a component called <code>OnlyEvens</code>. Currently, this method returns <code>true</code> so <code>OnlyEvens</code> re-renders every time it receives new <code>props</code>. Modify the method so <code>OnlyEvens</code> updates only if the <code>value</code> of its new props is even. Click the <code>Add</code> button and watch the order of events in your browser's console as the other lifecycle hooks are triggered.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class OnlyEvens extends React.Component {
  constructor(props) {
    super(props);
  }
  shouldComponentUpdate(nextProps, nextState) {
    console.log('Should I update?');
     // change code below this line
    return true;
     // change code above this line
  }
  componentWillReceiveProps(nextProps) {
    console.log('Receiving new props...');
  }
  componentDidUpdate() {
    console.log('Component re-rendered.');
  }
  render() {
    return <h1>{this.props.value}</h1>
  }
};

class Controller extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      value: 0
    };
    this.addValue = this.addValue.bind(this);
  }
  addValue() {
    this.setState({
      value: this.state.value + 1
    });
  }
  render() {
    return (
      <div>
        <button onClick={this.addValue}>Add</button>
        <OnlyEvens value={this.state.value}/>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<Controller />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class OnlyEvens extends React.Component {
  constructor(props) {
    super(props);
  }
  shouldComponentUpdate(nextProps, nextState) {
    console.log('Should I update?');
    // change code below this line
    return nextProps.value % 2 === 0;
    // change code above this line
  }
  componentWillReceiveProps(nextProps) {
    console.log('Receiving new props...');
  }
  componentDidUpdate() {
    console.log('Component re-rendered.');
  }
  render() {
    return <h1>{this.props.value}</h1>
  }
};

class Controller extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      value: 0
    };
  this.addValue = this.addValue.bind(this);
  }
  addValue() {
    this.setState({
      value: this.state.value + 1
    });
  }
  render() {
    return (
      <div>
        <button onClick={this.addValue}>Add</button>
        <OnlyEvens value={this.state.value}/>
      </div>
    );
  }
};
```

</section>
<hr>

# 37. Introducing Inline Styles

## Description
<section id='description'>
There are other complex concepts that add powerful capabilities to your React code. But you may be wondering about the more simple problem of how to style those JSX elements you create in React. You likely know that it won't be exactly the same as working with HTML because of <a target="_blank" href="learn/front-end-libraries/react/define-an-html-class-in-jsx"> the way you apply classes to JSX elements</a>.
If you import styles from a stylesheet, it isn't much different at all. You apply a class to your JSX element using the <code>className</code> attribute, and apply styles to the class in your stylesheet. Another option is to apply <strong><em>inline</em></strong> styles, which are very common in ReactJS development.
You apply inline styles to JSX elements similar to how you do it in HTML, but with a few JSX differences. Here's an example of an inline style in HTML:
<code>&lt;div style="color: yellow; font-size: 16px"&gt;Mellow Yellow&lt;/div&gt;</code>
JSX elements use the <code>style</code> attribute, but because of the way JSX is transpiled, you can't set the value to a <code>string</code>. Instead, you set it equal to a JavaScript <code>object</code>. Here's an example:
<code>&lt;div style={{color: "yellow", fontSize: 16}}&gt;Mellow Yellow&lt;/div&gt;</code>
Notice how we camelCase the "fontSize" property? This is because React will not accept kebab-case keys in the style object. React will apply the correct property name for us in the HTML.
</section>

## Instructions
<section id='instructions'>
Add a <code>style</code> attribute to the <code>div</code> in the code editor to give the text a color of red and font size of 72px.
Note that you can optionally set the font size to be a number, omitting the units "px", or write it as "72px".
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

class Colorful extends React.Component {
  render() {
    return (
      <div>Big Red</div>
    );
  }
};

```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<Colorful />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class Colorful extends React.Component {
  render() {
    return (
      <div style={{color: "red", fontSize: 72}}>Big Red</div>
    );
  }
};

```

</section>
<hr>

# 38. Add Inline Styles in React

## Description
<section id='description'>
You may have noticed in the last challenge that there were several other syntax differences from HTML inline styles in addition to the <code>style</code> attribute set to a JavaScript object. First, the names of certain CSS style properties use camel case. For example, the last challenge set the size of the font with <code>fontSize</code> instead of <code>font-size</code>. Hyphenated words like <code>font-size</code> are invalid syntax for JavaScript object properties, so React uses camel case. As a rule, any hyphenated style properties are written using camel case in JSX.
All property value length units (like <code>height</code>, <code>width</code>, and <code>fontSize</code>) are assumed to be in <code>px</code> unless otherwise specified. If you want to use <code>em</code>, for example, you wrap the value and the units in quotes, like <code>{fontSize: "4em"}</code>. Other than the length values that default to <code>px</code>, all other property values should be wrapped in quotes.
</section>

## Instructions
<section id='instructions'>
If you have a large set of styles, you can assign a style <code>object</code> to a constant to keep your code organized. Uncomment the <code>styles</code> constant and declare an <code>object</code> with three style properties and their values. Give the <code>div</code> a color of <code>"purple"</code>, a font-size of <code>40</code>, and a border of <code>"2px solid purple"</code>. Then set the <code>style</code> attribute equal to the <code>styles</code> constant.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

// const styles =
// change code above this line
class Colorful extends React.Component {
  render() {
    // change code below this line
    return (
      <div style={{color: "yellow", fontSize: 24}}>Style Me!</div>
    );
    // change code above this line
  }
};

```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<Colorful />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const styles = {
  color: "purple",
  fontSize: 40,
  border: "2px solid purple"
};
// change code above this line
class Colorful extends React.Component {
  render() {
    // change code below this line
    return (
      <div style={styles}>Style Me!</div>
  // change code above this line
    );
  }
};

```

</section>
<hr>

# 39. Use Advanced JavaScript in React Render Method

## Description
<section id='description'>
In previous challenges, you learned how to inject JavaScript code into JSX code using curly braces, <code>{ }</code>, for tasks like accessing props, passing props, accessing state, inserting comments into your code, and most recently, styling your components. These are all common use cases to put JavaScript in JSX, but they aren't the only way that you can utilize JavaScript code in your React components.
You can also write JavaScript directly in your <code>render</code> methods, before the <code>return</code> statement, <strong><em>without</em></strong> inserting it inside of curly braces. This is because it is not yet within the JSX code. When you want to use a variable later in the JSX code <em>inside</em> the <code>return</code> statement, you place the variable name inside curly braces.
</section>

## Instructions
<section id='instructions'>
In the code provided, the <code>render</code> method has an array that contains 20 phrases to represent the answers found in the classic 1980's Magic Eight Ball toy. The button click event is bound to the <code>ask</code> method, so each time the button is clicked a random number will be generated and stored as the <code>randomIndex</code> in state. On line 52, delete the string <code>"change me!"</code> and reassign the <code>answer</code> const so your code randomly accesses a different index of the <code>possibleAnswers</code> array each time the component updates. Finally, insert the <code>answer</code> const inside the <code>p</code> tags.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const inputStyle = {
  width: 235,
  margin: 5
}

class MagicEightBall extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      userInput: '',
      randomIndex: ''
    }
    this.ask = this.ask.bind(this);
    this.handleChange = this.handleChange.bind(this);
  }
  ask() {
    if (this.state.userInput) {
      this.setState({
        randomIndex: Math.floor(Math.random() * 20),
        userInput: ''
      });
    }
  }
  handleChange(event) {
    this.setState({
      userInput: event.target.value
    });
  }
  render() {
    const possibleAnswers = [
      'It is certain',
      'It is decidedly so',
      'Without a doubt',
      'Yes, definitely',
      'You may rely on it',
      'As I see it, yes',
      'Outlook good',
      'Yes',
      'Signs point to yes',
      'Reply hazy try again',
      'Ask again later',
      'Better not tell you now',
      'Cannot predict now',
      'Concentrate and ask again',
      'Don\'t count on it',
      'My reply is no',
      'My sources say no',
      'Most likely',
      'Outlook not so good',
      'Very doubtful'
    ];
    const answer = 'change me!' // << change code here
    return (
      <div>
        <input
          type="text"
          value={this.state.userInput}
          onChange={this.handleChange}
          style={inputStyle} /><br />
        <button onClick={this.ask}>
          Ask the Magic Eight Ball!
        </button><br />
        <h3>Answer:</h3>
        <p>
          { /* change code below this line */ }

          { /* change code above this line */ }
        </p>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
var possibleAnswers = [ 'It is certain', 'It is decidedly so', 'Without a doubt', 'Yes, definitely', 'You may rely on it', 'As I see it, yes', 'Outlook good', 'Yes', 'Signs point to yes', 'Reply hazy try again', 'Ask again later', 'Better not tell you now', 'Cannot predict now', 'Concentrate and ask again', 'Don\'t count on it', 'My reply is no', 'My sources say no', 'Outlook not so good','Very doubtful', 'Most likely' ];
ReactDOM.render(<MagicEightBall />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const inputStyle = {
  width: 235,
  margin: 5
}

class MagicEightBall extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      userInput: '',
      randomIndex: ''
    }
    this.ask = this.ask.bind(this);
    this.handleChange = this.handleChange.bind(this);
  }
  ask() {
    if (this.state.userInput) {
      this.setState({
        randomIndex: Math.floor(Math.random() * 20),
        userInput: ''
      });
    }
  }
  handleChange(event) {
    this.setState({
      userInput: event.target.value
    });
  }
  render() {
    const possibleAnswers = [
      "It is certain", "It is decidedly so", "Without a doubt",
      "Yes, definitely", "You may rely on it", "As I see it, yes",
      "Outlook good", "Yes", "Signs point to yes", "Reply hazy try again",
      "Ask again later", "Better not tell you now", "Cannot predict now",
      "Concentrate and ask again", "Don't count on it", "My reply is no",
      "My sources say no", "Outlook not so good","Very doubtful", "Most likely"
    ];
    const answer = possibleAnswers[this.state.randomIndex];
    return (
      <div>
        <input
          type="text"
          value={this.state.userInput}
          onChange={this.handleChange}
          style={inputStyle} /><br />
        <button onClick={this.ask}>Ask the Magic Eight Ball!</button><br />
        <h3>Answer:</h3>
        <p>
          {answer}
        </p>
      </div>
    );
  }
};
```

</section>
<hr>

# 40. Render with an If/Else Condition

## Description
<section id='description'>
Another application of using JavaScript to control your rendered view is to tie the elements that are rendered to a condition. When the condition is true, one view renders. When it's false, it's a different view. You can do this with a standard <code>if/else</code> statement in the <code>render()</code> method of a React component.
</section>

## Instructions
<section id='instructions'>
MyComponent contains a <code>boolean</code> in its state which tracks whether you want to display some element in the UI or not. The <code>button</code> toggles the state of this value. Currently, it renders the same UI every time. Rewrite the <code>render()</code> method with an <code>if/else</code> statement so that if <code>display</code> is <code>true</code>, you return the current markup. Otherwise, return the markup without the <code>h1</code> element.
<strong>Note:</strong>&nbsp;You must write an <code>if/else</code> to pass the tests. Use of the ternary operator will not pass here.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      display: true
    }
    this.toggleDisplay = this.toggleDisplay.bind(this);
  }
  toggleDisplay() {
    this.setState({
      display: !this.state.display
    });
  }
  render() {
    // change code below this line

    return (
       <div>
         <button onClick={this.toggleDisplay}>Toggle Display</button>
         <h1>Displayed!</h1>
       </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      display: true
    }
 this.toggleDisplay = this.toggleDisplay.bind(this);
 }
  toggleDisplay() {
    this.setState({
      display: !this.state.display
    });
  }
  render() {
    // change code below this line
    if (this.state.display) {
      return (
         <div>
           <button onClick={this.toggleDisplay}>Toggle Display</button>
           <h1>Displayed!</h1>
         </div>
      );
    } else {
      return (
        <div>
           <button onClick={this.toggleDisplay}>Toggle Display</button>
         </div>
      );
    }
  }
};
```

</section>
<hr>

# 41. Use && for a More Concise Conditional

## Description
<section id='description'>
The if/else statements worked in the last challenge, but there's a more concise way to achieve the same result. Imagine that you are tracking several conditions in a component and you want different elements to render depending on each of these conditions. If you write a lot of <code>else if</code> statements to return slightly different UIs, you may repeat code which leaves room for error. Instead, you can use the <code>&&</code> logical operator to perform conditional logic in a more concise way. This is possible because you want to check if a condition is <code>true</code>, and if it is, return some markup. Here's an example:
<code>{condition && &lt;p&gt;markup&lt;/p&gt;}</code>
If the <code>condition</code> is <code>true</code>, the markup will be returned. If the condition is <code>false</code>, the operation will immediately return <code>false</code> after evaluating the <code>condition</code> and return nothing. You can include these statements directly in your JSX and string multiple conditions together by writing <code>&&</code> after each one. This allows you to handle more complex conditional logic in your <code>render()</code> method without repeating a lot of code.
</section>

## Instructions
<section id='instructions'>
Solve the previous example again, so the <code>h1</code> only renders if <code>display</code> is <code>true</code>, but use the <code>&&</code> logical operator instead of an <code>if/else</code> statement.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      display: true
    }
    this.toggleDisplay = this.toggleDisplay.bind(this);
  }
  toggleDisplay() {
    this.setState({
      display: !this.state.display
    });
  }
  render() {
    // change code below this line
    return (
       <div>
         <button onClick={this.toggleDisplay}>Toggle Display</button>
         <h1>Displayed!</h1>
       </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      display: true
    }
 this.toggleDisplay = this.toggleDisplay.bind(this);
  }
  toggleDisplay() {
    this.setState({
      display: !this.state.display
    });
  }
  render() {
    // change code below this line
    return (
       <div>
         <button onClick={this.toggleDisplay}>Toggle Display</button>
         {this.state.display && <h1>Displayed!</h1>}
       </div>
    );
  }
};
```

</section>
<hr>

# 42. Use a Ternary Expression for Conditional Rendering

## Description
<section id='description'>
Before moving on to dynamic rendering techniques, there's one last way to use built-in JavaScript conditionals to render what you want: the <em><strong>ternary operator</strong></em>. The ternary operator is often utilized as a shortcut for <code>if/else</code> statements in JavaScript. They're not quite as robust as traditional <code>if/else</code> statements, but they are very popular among React developers. One reason for this is because of how JSX is compiled, <code>if/else</code> statements can't be inserted directly into JSX code. You might have noticed this a couple challenges ago &mdash; when an <code>if/else</code> statement was required, it was always <em>outside</em> the <code>return</code> statement. Ternary expressions can be an excellent alternative if you want to implement conditional logic within your JSX. Recall that a ternary operator has three parts, but you can combine several ternary expressions together. Here's the basic syntax:
<blockquote>condition ? expressionIfTrue : expressionIfFalse</blockquote>
</section>

## Instructions
<section id='instructions'>
The code editor has three constants defined within the <code>CheckUserAge</code> component's <code>render()</code> method. They are called <code>buttonOne</code>, <code>buttonTwo</code>, and <code>buttonThree</code>. Each of these is assigned a simple JSX expression representing a button element. First, initialize the state of <code>CheckUserAge</code> with <code>input</code> and <code>userAge</code> both set to values of an empty string.
Once the component is rendering information to the page, users should have a way to interact with it. Within the component's <code>return</code> statement, set up a ternary expression that implements the following logic: when the page first loads, render the submit button, <code>buttonOne</code>, to the page. Then, when a user enters their age and clicks the button, render a different button based on the age. If a user enters a number less than <code>18</code>, render <code>buttonThree</code>. If a user enters a number greater than or equal to <code>18</code>, render <code>buttonTwo</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

const inputStyle = {
  width: 235,
  margin: 5
}

class CheckUserAge extends React.Component {
  constructor(props) {
    super(props);
    // change code below this line

    // change code above this line
    this.submit = this.submit.bind(this);
    this.handleChange = this.handleChange.bind(this);
  }
  handleChange(e) {
    this.setState({
      input: e.target.value,
      userAge: ''
    });
  }
  submit() {
    this.setState({
      userAge: this.state.input
    });
  }
  render() {
    const buttonOne = <button onClick={this.submit}>Submit</button>;
    const buttonTwo = <button>You May Enter</button>;
    const buttonThree = <button>You Shall Not Pass</button>;
    return (
      <div>
        <h3>Enter Your Age to Continue</h3>
        <input
          style={inputStyle}
          type="number"
          value={this.state.input}
          onChange={this.handleChange} /><br />
        {
          /* change code here */
        }
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<CheckUserAge />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const inputStyle = {
  width: 235,
  margin: 5
}

class CheckUserAge extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      userAge: '',
      input: ''
    }
    this.submit = this.submit.bind(this);
    this.handleChange = this.handleChange.bind(this);
  }
  handleChange(e) {
    this.setState({
      input: e.target.value,
      userAge: ''
    });
  }
  submit() {
    this.setState({
      userAge: this.state.input
    });
  }
  render() {
    const buttonOne = <button onClick={this.submit}>Submit</button>;
    const buttonTwo = <button>You May Enter</button>;
    const buttonThree = <button>You Shall Not Pass</button>;
    return (
      <div>
        <h3>Enter Your Age to Continue</h3>
        <input
          style={inputStyle}
          type="number"
          value={this.state.input}
          onChange={this.handleChange} /><br />
          {
            this.state.userAge === '' ?
            buttonOne :
            this.state.userAge >= 18 ?
            buttonTwo :
            buttonThree
          }
      </div>
    );
  }
};
```

</section>
<hr>

# 43. Render Conditionally from Props

## Description
<section id='description'>
So far, you've seen how to use <code>if/else</code>, <code>&&,</code> <code>null</code> and the ternary operator (<code>condition ? expressionIfTrue : expressionIfFalse</code>) to make conditional decisions about what to render and when. However, there's one important topic left to discuss that lets you combine any or all of these concepts with another powerful React feature: props. Using props to conditionally render code is very common with React developers &mdash; that is, they use the value of a given prop to automatically make decisions about what to render.
In this challenge, you'll set up a child component to make rendering decisions based on props. You'll also use the ternary operator, but you can see how several of the other concepts that were covered in the last few challenges might be just as useful in this context.
</section>

## Instructions
<section id='instructions'>
The code editor has two components that are partially defined for you: a parent called <code>GameOfChance</code>, and a child called <code>Results</code>. They are used to create a simple game where the user presses a button to see if they win or lose.
First, you'll need a simple expression that randomly returns a different value every time it is run. You can use <code>Math.random()</code>. This method returns a value between <code>0</code> (inclusive) and <code>1</code> (exclusive) each time it is called. So for 50/50 odds, use <code>Math.random() > .5</code> in your expression. Statistically speaking, this expression will return <code>true</code> 50% of the time, and <code>false</code> the other 50%. On line 30, replace the comment with this expression to complete the variable declaration.
Now you have an expression that you can use to make a randomized decision in the code. Next you need to implement this. Render the <code>Results</code> component as a child of <code>GameOfChance</code>, and pass in <code>expression</code> as a prop called <code>fiftyFifty</code>. In the <code>Results</code> component, write a ternary expression to render the text <code>"You Win!"</code> or <code>"You Lose!"</code> based on the <code>fiftyFifty</code> prop that's being passed in from <code>GameOfChance</code>. Finally, make sure the <code>handleClick()</code> method is correctly counting each turn so the user knows how many times they've played. This also serves to let the user know the component has actually updated in case they win or lose twice in a row.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class Results extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <h1>
      {
        /* change code here */
      }
      </h1>
    )
  };
};

class GameOfChance extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      counter: 1
    }
    this.handleClick = this.handleClick.bind(this);
  }
  handleClick() {
    this.setState({
      counter: 0 // change code here
    });
  }
  render() {
    let expression = null; // change code here
    return (
      <div>
        <button onClick={this.handleClick}>Play Again</button>
        { /* change code below this line */ }

        { /* change code above this line */ }
        <p>{'Turn: ' + this.state.counter}</p>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<GameOfChance />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class Results extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return (
      <h1>
      {
        this.props.fiftyFifty ?
        'You Win!' :
        'You Lose!'
      }
      </h1>
    )
  };
};

class GameOfChance extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      counter: 1
    }
    this.handleClick = this.handleClick.bind(this);
  }
  handleClick() {
    this.setState({
      counter: this.state.counter + 1
    });
  }
  render() {
    const expression = Math.random() > .5;
    return (
      <div>
        <button onClick={this.handleClick}>Play Again</button>
        <Results fiftyFifty={expression} />
        <p>{'Turn: ' + this.state.counter}</p>
      </div>
    );
  }
};
```

</section>
<hr>

# 44. Change Inline CSS Conditionally Based on Component State

## Description
<section id='description'>
At this point, you've seen several applications of conditional rendering and the use of inline styles. Here's one more example that combines both of these topics. You can also render CSS conditionally based on the state of a React component. To do this, you check for a condition, and if that condition is met, you modify the styles object that's assigned to the JSX elements in the render method.
This paradigm is important to understand because it is a dramatic shift from the more traditional approach of applying styles by modifying DOM elements directly (which is very common with jQuery, for example). In that approach, you must keep track of when elements change and also handle the actual manipulation directly. It can become difficult to keep track of changes, potentially making your UI unpredictable. When you set a style object based on a condition, you describe how the UI should look as a function of the application's state. There is a clear flow of information that only moves in one direction. This is the preferred method when writing applications with React.
</section>

## Instructions
<section id='instructions'>
The code editor has a simple controlled input component with a styled border. You want to style this border red if the user types more than 15 characters of text in the input box. Add a condition to check for this and, if the condition is valid, set the input border style to <code>3px solid red</code>. You can try it out by entering text in the input.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

class GateKeeper extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: ''
    };
    this.handleChange = this.handleChange.bind(this);
  }
  handleChange(event) {
    this.setState({ input: event.target.value })
  }
  render() {
    let inputStyle = {
      border: '1px solid black'
    };
    // change code below this line

    // change code above this line
    return (
      <div>
        <h3>Don't Type Too Much:</h3>
        <input
          type="text"
          style={inputStyle}
          value={this.state.input}
          onChange={this.handleChange} />
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<GateKeeper />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class GateKeeper extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: ''
    };
    this.handleChange = this.handleChange.bind(this);
  }
  handleChange(event) {
    this.setState({ input: event.target.value })
  }
  render() {
    let inputStyle = {
      border: '1px solid black'
    };
    if (this.state.input.length > 15) {
      inputStyle.border = '3px solid red';
    };
    return (
      <div>
        <h3>Don't Type Too Much:</h3>
        <input
          type="text"
          style={inputStyle}
          value={this.state.input}
          onChange={this.handleChange} />
      </div>
    );
  }
};
```

</section>
<hr>

# 45. Use Array.map() to Dynamically Render Elements

## Description
<section id='description'>
Conditional rendering is useful, but you may need your components to render an unknown number of elements. Often in reactive programming, a programmer has no way to know what the state of an application is until runtime, because so much depends on a user's interaction with that program. Programmers need to write their code to correctly handle that unknown state ahead of time. Using <code>Array.map()</code> in React illustrates this concept.
For example, you create a simple "To Do List" app. As the programmer, you have no way of knowing how many items a user might have on their list. You need to set up your component to <em><strong>dynamically render</strong></em> the correct number of list elements long before someone using the program decides that today is laundry day.
</section>

## Instructions
<section id='instructions'>
The code editor has most of the <code>MyToDoList</code> component set up. Some of this code should look familiar if you completed the controlled form challenge. You'll notice a <code>textarea</code> and a <code>button</code>, along with a couple of methods that track their states, but nothing is rendered to the page yet.
Inside the <code>constructor</code>, create a <code>this.state</code> object and define two states: <code>userInput</code> should be initialized as an empty string, and <code>toDoList</code> should be initialized as an empty array. Next, delete the comment in the <code>render()</code> method next to the <code>items</code> variable. In its place, map over the <code>toDoList</code> array stored in the component's internal state and dynamically render a <code>li</code> for each item. Try entering the string <code>eat, code, sleep, repeat</code> into the <code>textarea</code>, then click the button and see what happens.
<strong>Note:</strong>&nbsp;You may know that all sibling child elements created by a mapping operation like this do need to be supplied with a unique <code>key</code> attribute. Don't worry, this is the topic of the next challenge.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const textAreaStyles = {
  width: 235,
  margin: 5
};

class MyToDoList extends React.Component {
  constructor(props) {
    super(props);
    // change code below this line

    // change code above this line
    this.handleSubmit = this.handleSubmit.bind(this);
    this.handleChange = this.handleChange.bind(this);
  }
  handleSubmit() {
    const itemsArray = this.state.userInput.split(',');
    this.setState({
      toDoList: itemsArray
    });
  }
  handleChange(e) {
    this.setState({
      userInput: e.target.value
    });
  }
  render() {
    const items = null; // change code here
    return (
      <div>
        <textarea
          onChange={this.handleChange}
          value={this.state.userInput}
          style={textAreaStyles}
          placeholder="Separate Items With Commas" /><br />
        <button onClick={this.handleSubmit}>Create List</button>
        <h1>My "To Do" List:</h1>
        <ul>
          {items}
        </ul>
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyToDoList />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const textAreaStyles = {
  width: 235,
  margin: 5
};

class MyToDoList extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      toDoList: [],
      userInput: ''
    }
    this.handleSubmit = this.handleSubmit.bind(this);
    this.handleChange = this.handleChange.bind(this);
  }
  handleSubmit() {
    const itemsArray = this.state.userInput.split(',');
    this.setState({
      toDoList: itemsArray
    });
  }
  handleChange(e) {
    this.setState({
      userInput: e.target.value
    });
  }
  render() {
    const items = this.state.toDoList.map( (item, i) => {
      return <li key={i}>{item}</li>
    });
    return (
      <div>
        <textarea
          onChange={this.handleChange}
          value={this.state.userInput}
          style={textAreaStyles}
          placeholder="Separate Items With Commas" /><br />
        <button onClick={this.handleSubmit}>Create List</button>
        <h1>My "To Do" List:</h1>
        <ul>
          {items}
        </ul>
      </div>
    );
  }
};
```

</section>
<hr>

# 46. Give Sibling Elements a Unique Key Attribute

## Description
<section id='description'>
The last challenge showed how the <code>map</code> method is used to dynamically render a number of elements based on user input. However, there was an important piece missing from that example. When you create an array of elements, each one needs a <code>key</code> attribute set to a unique value. React uses these keys to keep track of which items are added, changed, or removed. This helps make the re-rendering process more efficient when the list is modified in any way.<br><br><strong>Note:</strong> Keys only need to be unique between sibling elements, they don't need to be globally unique in your application.
</section>

## Instructions
<section id='instructions'>
The code editor has an array with some front end frameworks and a stateless functional component named <code>Frameworks()</code>. <code>Frameworks()</code> needs to map the array to an unordered list, much like in the last challenge. Finish writing the <code>map</code> callback to return an <code>li</code> element for each framework in the <code>frontEndFrameworks</code> array. This time, make sure to give each <code>li</code> a <code>key</code> attribute, set to a unique value. The <code>li</code> elements should also contain text from <code>frontEndFrameworks</code>.
Normally, you want to make the key something that uniquely identifies the element being rendered. As a last resort the array index may be used, but typically you should try to use a unique identification.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

const frontEndFrameworks = [
  'React',
  'Angular',
  'Ember',
  'Knockout',
  'Backbone',
  'Vue'
];

function Frameworks() {
  const renderFrameworks = null; // change code here
  return (
    <div>
      <h1>Popular Front End JavaScript Frameworks</h1>
      <ul>
        {renderFrameworks}
      </ul>
    </div>
  );
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<Frameworks />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const frontEndFrameworks = [
  'React',
  'Angular',
  'Ember',
  'Knockout',
  'Backbone',
  'Vue'
];

function Frameworks() {
  const renderFrameworks = frontEndFrameworks.map((fw, i) => <li key={i}>{fw}</li>);
  return (
    <div>
      <h1>Popular Front End JavaScript Frameworks</h1>
      <ul>
        {renderFrameworks}
      </ul>
    </div>
  );
};
```

</section>
<hr>

# 47. Use Array.filter() to Dynamically Filter an Array

## Description
<section id='description'>
The <code>map</code> array method is a powerful tool that you will use often when working with React. Another method related to <code>map</code> is <code>filter</code>, which filters the contents of an array based on a condition, then returns a new array. For example, if you have an array of users that all have a property <code>online</code> which can be set to <code>true</code> or <code>false</code>, you can filter only those users that are online by writing:
<code>let onlineUsers = users.filter(user => user.online);</code>
</section>

## Instructions
<section id='instructions'>
In the code editor, <code>MyComponent</code>&apos;s <code>state</code> is initialized with an array of users. Some users are online and some aren't. Filter the array so you see only the users who are online. To do this, first use <code>filter</code> to return a new array containing only the users whose <code>online</code> property is <code>true</code>. Then, in the <code>renderOnline</code> variable, map over the filtered array, and return a <code>li</code> element for each user that contains the text of their <code>username</code>. Be sure to include a unique <code>key</code> as well, like in the last challenges.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      users: [
        {
          username: 'Jeff',
          online: true
        },
        {
          username: 'Alan',
          online: false
        },
        {
          username: 'Mary',
          online: true
        },
        {
          username: 'Jim',
          online: false
        },
        {
          username: 'Sara',
          online: true
        },
        {
          username: 'Laura',
          online: true
        }
      ]
    }
  }
  render() {
    const usersOnline = null; // change code here
    const renderOnline = null; // change code here
    return (
       <div>
         <h1>Current Online Users:</h1>
         <ul>
           {renderOnline}
         </ul>
       </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<MyComponent />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      users: [
        {
          username: 'Jeff',
          online: true
        },
        {
          username: 'Alan',
          online: false
        },
        {
          username: 'Mary',
          online: true
        },
        {
          username: 'Jim',
          online: false
        },
        {
          username: 'Sara',
          online: true
        },
        {
          username: 'Laura',
          online: true
        }
      ]
    }
  }
  render() {
    const usersOnline = this.state.users.filter(user => {
      return user.online;
    });
    const renderOnlineUsers = usersOnline.map(user => {
      return (
        <li key={user.username}>{user.username}</li>
      );
    });
    return (
       <div>
         <h1>Current Online Users:</h1>
         <ul>
          {renderOnlineUsers}
        </ul>
       </div>
    );
  }
};
```

</section>
<hr>

# 48. Render React on the Server with renderToString

## Description
<section id='description'>
So far, you have been rendering React components on the client. Normally, this is what you will always do. However, there are some use cases where it makes sense to render a React component on the server. Since React is a JavaScript view library and you can run JavaScript on the server with Node, this is possible. In fact, React provides a <code>renderToString()</code> method you can use for this purpose.
There are two key reasons why rendering on the server may be used in a real world app. First, without doing this, your React apps would consist of a relatively empty HTML file and a large bundle of JavaScript when it's initially loaded to the browser. This may not be ideal for search engines that are trying to index the content of your pages so people can find you. If you render the initial HTML markup on the server and send this to the client, the initial page load contains all of the page's markup which can be crawled by search engines. Second, this creates a faster initial page load experience because the rendered HTML is smaller than the JavaScript code of the entire app. React will still be able to recognize your app and manage it after the initial load.
</section>

## Instructions
<section id='instructions'>
The <code>renderToString()</code> method is provided on <code>ReactDOMServer</code>, which is available here as a global object. The method takes one argument which is a React element. Use this to render <code>App</code> to a string.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx

class App extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return <div/>
  }
};

// change code below this line

```

</div>

### Before Test
<div id='jsx-setup'>

```jsx
var ReactDOMServer = { renderToString(x) { return null; } };
```

</div>

### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<App />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class App extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return <div/>
  }
};

// change code below this line
ReactDOMServer.renderToString(<App/>);
```

</section>
<hr>

# Redux
# 1. Create a Redux Store

## Description
<section id='description'>
Redux is a state management framework that can be used with a number of different web technologies, including React.
In Redux, there is a single state object that's responsible for the entire state of your application. This means if you had a React app with ten components, and each component had its own local state, the entire state of your app would be defined by a single state object housed in the Redux <code>store</code>. This is the first important principle to understand when learning Redux: the Redux store is the single source of truth when it comes to application state.
This also means that any time any piece of your app wants to update state, it <strong>must</strong> do so through the Redux store. The unidirectional data flow makes it easier to track state management in your app.
</section>

## Instructions
<section id='instructions'>
The Redux <code>store</code> is an object which holds and manages application <code>state</code>. There is a method called <code>createStore()</code> on the Redux object, which you use to create the Redux <code>store</code>. This method takes a <code>reducer</code> function as a required argument. The <code>reducer</code> function is covered in a later challenge, and is already defined for you in the code editor. It simply takes <code>state</code> as an argument and returns <code>state</code>.
Declare a <code>store</code> variable and assign it to the <code>createStore()</code> method, passing in the <code>reducer</code> as an argument.
<strong>Note:</strong>&nbsp;The code in the editor uses ES6 default argument syntax to initialize this state to hold a value of <code>5</code>. If you're not familiar with default arguments, you can refer to the <a target="_blank" href="https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/es6/set-default-parameters-for-your-functions">ES6 section in the Curriculum</a> which covers this topic.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const reducer = (state = 5) => {
  return state;
}

// Redux methods are available from a Redux object
// For example: Redux.createStore()
// Define the store here:


```

</div>



</section>

## Solution
<section id='solution'>


```js
const reducer = (state = 5) => {
  return state;
}

// Redux methods are available from a Redux object
// For example: Redux.createStore()
// Define the store here:

const store = Redux.createStore(reducer);
```

</section>
<hr>

# 2. Get State from the Redux Store

## Description
<section id='description'>
The Redux store object provides several methods that allow you to interact with it. For example, you can retrieve the current <code>state</code> held in the Redux store object with the <code>getState()</code> method.
</section>

## Instructions
<section id='instructions'>
The code from the previous challenge is re-written more concisely in the code editor. Use <code>store.getState()</code> to retrieve the <code>state</code> from the <code>store</code>, and assign this to a new variable <code>currentState</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const store = Redux.createStore(
  (state = 5) => state
);

// change code below this line

```

</div>



</section>

## Solution
<section id='solution'>


```js
const store = Redux.createStore(
  (state = 5) => state
);

// change code below this line
const currentState = store.getState();
```

</section>
<hr>

# 3. Define a Redux Action

## Description
<section id='description'>
Since Redux is a state management framework, updating state is one of its core tasks. In Redux, all state updates are triggered by dispatching actions. An action is simply a JavaScript object that contains information about an action event that has occurred. The Redux store receives these action objects, then updates its state accordingly. Sometimes a Redux action also carries some data. For example, the action carries a username after a user logs in. While the data is optional, actions must carry a <code>type</code> property that specifies the 'type' of action that occurred.
Think of Redux actions as messengers that deliver information about events happening in your app to the Redux store. The store then conducts the business of updating state based on the action that occurred.
</section>

## Instructions
<section id='instructions'>
Writing a Redux action is as simple as declaring an object with a type property. Declare an object <code>action</code> and give it a property <code>type</code> set to the string <code>'LOGIN'</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
// Define an action here:

```

</div>



</section>

## Solution
<section id='solution'>


```js
const action = {
  type: 'LOGIN'
}
```

</section>
<hr>

# 4. Define an Action Creator

## Description
<section id='description'>
After creating an action, the next step is sending the action to the Redux store so it can update its state. In Redux, you define action creators to accomplish this. An action creator is simply a JavaScript function that returns an action. In other words, action creators create objects that represent action events.
</section>

## Instructions
<section id='instructions'>
Define a function named <code>actionCreator()</code> that returns the <code>action</code> object when called.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const action = {
  type: 'LOGIN'
}
// Define an action creator here:

```

</div>



</section>

## Solution
<section id='solution'>


```js
const action = {
  type: 'LOGIN'
}
// Define an action creator here:
const actionCreator = () => {
  return action;
};
```

</section>
<hr>

# 5. Dispatch an Action Event

## Description
<section id='description'>
<code>dispatch</code> method is what you use to dispatch actions to the Redux store. Calling <code>store.dispatch()</code> and passing the value returned from an action creator sends an action back to the store.
Recall that action creators return an object with a type property that specifies the action that has occurred. Then the method dispatches an action object to the Redux store. Based on the previous challenge's example, the following lines are equivalent, and both dispatch the action of type <code>LOGIN</code>:
<blockquote>store.dispatch(actionCreator());<br>store.dispatch({ type: 'LOGIN' });</blockquote>
</section>

## Instructions
<section id='instructions'>
The Redux store in the code editor has an initialized state that's an object containing a <code>login</code> property currently set to <code>false</code>. There's also an action creator called <code>loginAction()</code> which returns an action of type <code>LOGIN</code>. Dispatch the <code>LOGIN</code> action to the Redux store by calling the <code>dispatch</code> method, and pass in the action created by <code>loginAction()</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const store = Redux.createStore(
  (state = {login: false}) => state
);

const loginAction = () => {
  return {
    type: 'LOGIN'
  }
};

// Dispatch the action here:

```

</div>



</section>

## Solution
<section id='solution'>


```js
const store = Redux.createStore(
  (state = {login: false}) => state
);

const loginAction = () => {
  return {
    type: 'LOGIN'
  }
};

// Dispatch the action here:
store.dispatch(loginAction());
```

</section>
<hr>

# 6. Handle an Action in the Store

## Description
<section id='description'>
After an action is created and dispatched, the Redux store needs to know how to respond to that action. This is the job of a <code>reducer</code> function. Reducers in Redux are responsible for the state modifications that take place in response to actions. A <code>reducer</code> takes <code>state</code> and <code>action</code> as arguments, and it always returns a new <code>state</code>. It is important to see that this is the <strong>only</strong> role of the reducer. It has no side effects &mdash; it never calls an API endpoint and it never has any hidden surprises. The reducer is simply a pure function that takes state and action, then returns new state.
Another key principle in Redux is that <code>state</code> is read-only. In other words, the <code>reducer</code> function must <strong>always</strong> return a new copy of <code>state</code> and never modify state directly. Redux does not enforce state immutability, however, you are responsible for enforcing it in the code of your reducer functions. You'll practice this in later challenges.
</section>

## Instructions
<section id='instructions'>
The code editor has the previous example as well as the start of a <code>reducer</code> function for you. Fill in the body of the <code>reducer</code> function so that if it receives an action of type <code>'LOGIN'</code> it returns a state object with <code>login</code> set to <code>true</code>. Otherwise, it returns the current <code>state</code>. Note that the current <code>state</code> and the dispatched <code>action</code> are passed to the reducer, so you can access the action's type directly with <code>action.type</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const defaultState = {
  login: false
};

const reducer = (state = defaultState, action) => {
  // change code below this line

  // change code above this line
};

const store = Redux.createStore(reducer);

const loginAction = () => {
  return {
    type: 'LOGIN'
  }
};
```

</div>



</section>

## Solution
<section id='solution'>


```js
const defaultState = {
  login: false
};

const reducer = (state = defaultState, action) => {

  if (action.type === 'LOGIN') {
    return {login: true}
  }

  else {
    return state
  }

};

const store = Redux.createStore(reducer);

const loginAction = () => {
  return {
    type: 'LOGIN'
  }
};
```

</section>
<hr>

# 7. Use a Switch Statement to Handle Multiple Actions

## Description
<section id='description'>
You can tell the Redux store how to handle multiple action types. Say you are managing user authentication in your Redux store. You want to have a state representation for when users are logged in and when they are logged out. You represent this with a single state object with the property <code>authenticated</code>. You also need action creators that create actions corresponding to user login and user logout, along with the action objects themselves.
</section>

## Instructions
<section id='instructions'>
The code editor has a store, actions, and action creators set up for you. Fill in the <code>reducer</code> function to handle multiple authentication actions. Use a JavaScript <code>switch</code> statement in the <code>reducer</code> to respond to different action events. This is a standard pattern in writing Redux reducers. The switch statement should switch over <code>action.type</code> and return the appropriate authentication state.
<strong>Note:</strong>&nbsp;At this point, don't worry about state immutability, since it is small and simple in this example. For each action, you can return a new object &mdash; for example, <code>{authenticated: true}</code>. Also, don't forget to write a <code>default</code> case in your switch statement that returns the current <code>state</code>. This is important because once your app has multiple reducers, they are all run any time an action dispatch is made, even when the action isn't related to that reducer. In such a case, you want to make sure that you return the current <code>state</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const defaultState = {
  authenticated: false
};

const authReducer = (state = defaultState, action) => {
  // change code below this line

  // change code above this line
};

const store = Redux.createStore(authReducer);

const loginUser = () => {
  return {
    type: 'LOGIN'
  }
};

const logoutUser = () => {
  return {
    type: 'LOGOUT'
  }
};
```

</div>



</section>

## Solution
<section id='solution'>


```js
const defaultState = {
  authenticated: false
};

const authReducer = (state = defaultState, action) => {

  switch (action.type) {

    case 'LOGIN':
      return {
        authenticated: true
      }

    case 'LOGOUT':
      return {
        authenticated: false
      }

    default:
      return state;

  }

};

const store = Redux.createStore(authReducer);

const loginUser = () => {
  return {
    type: 'LOGIN'
  }
};

const logoutUser = () => {
  return {
    type: 'LOGOUT'
  }
};
```

</section>
<hr>

# 8. Use const for Action Types

## Description
<section id='description'>
A common practice when working with Redux is to assign action types as read-only constants, then reference these constants wherever they are used. You can refactor the code you're working with to write the action types as <code>const</code> declarations.
</section>

## Instructions
<section id='instructions'>
Declare <code>LOGIN</code> and <code>LOGOUT</code> as <code>const</code> values and assign them to the strings <code>'LOGIN'</code> and <code>'LOGOUT'</code>, respectively. Then, edit the <code>authReducer()</code> and the action creators to reference these constants instead of string values.
<strong>Note:</strong>&nbsp;It's generally a convention to write constants in all uppercase, and this is standard practice in Redux as well.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
// change code below this line

// change code above this line

const defaultState = {
  authenticated: false
};

const authReducer = (state = defaultState, action) => {

  switch (action.type) {

    case 'LOGIN':
      return {
        authenticated: true
      }

    case 'LOGOUT':
      return {
        authenticated: false
      }

    default:
      return state;

  }

};

const store = Redux.createStore(authReducer);

const loginUser = () => {
  return {
    type: 'LOGIN'
  }
};

const logoutUser = () => {
  return {
    type: 'LOGOUT'
  }
};
```

</div>



</section>

## Solution
<section id='solution'>


```js
const LOGIN = 'LOGIN';
const LOGOUT = 'LOGOUT';

const defaultState = {
  authenticated: false
};

const authReducer = (state = defaultState, action) => {

  switch (action.type) {

    case LOGIN:
      return {
        authenticated: true
      }

    case LOGOUT:
      return {
        authenticated: false
      }

    default:
      return state;

  }

};

const store = Redux.createStore(authReducer);

const loginUser = () => {
  return {
    type: LOGIN
  }
};

const logoutUser = () => {
  return {
    type: LOGOUT
  }
};
```

</section>
<hr>

# 9. Register a Store Listener

## Description
<section id='description'>
Another method you have access to on the Redux <code>store</code> object is <code>store.subscribe()</code>. This allows you to subscribe listener functions to the store, which are called whenever an action is dispatched against the store. One simple use for this method is to subscribe a function to your store that simply logs a message every time an action is received and the store is updated.
</section>

## Instructions
<section id='instructions'>
Write a callback function that increments the global variable <code>count</code> every time the store receives an action, and pass this function in to the <code>store.subscribe()</code> method. You'll see that <code>store.dispatch()</code> is called three times in a row, each time directly passing in an action object. Watch the console output between the action dispatches to see the updates take place.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const ADD = 'ADD';

const reducer = (state = 0, action) => {
  switch(action.type) {
    case ADD:
      return state + 1;
    default:
      return state;
  }
};

const store = Redux.createStore(reducer);

// global count variable:
let count = 0;

// change code below this line

// change code above this line

store.dispatch({type: ADD});
console.log(count);
store.dispatch({type: ADD});
console.log(count);
store.dispatch({type: ADD});
console.log(count);
```

</div>

### Before Test
<div id='jsx-setup'>

```jsx
count = 0;
```

</div>


</section>

## Solution
<section id='solution'>


```js
const ADD = 'ADD';

const reducer = (state = 0, action) => {
  switch(action.type) {
    case ADD:
      return state + 1;
    default:
      return state;
  }
};

const store = Redux.createStore(reducer);
 let count = 0;
// change code below this line

store.subscribe( () =>
 {
 count++;
 }
);

// change code above this line

store.dispatch({type: ADD});
store.dispatch({type: ADD});
store.dispatch({type: ADD});
```

</section>
<hr>

# 10. Combine Multiple Reducers

## Description
<section id='description'>
When the state of your app begins to grow more complex, it may be tempting to divide state into multiple pieces. Instead, remember the first principle of Redux: all app state is held in a single state object in the store. Therefore, Redux provides reducer composition as a solution for a complex state model. You define multiple reducers to handle different pieces of your application's state, then compose these reducers together into one root reducer. The root reducer is then passed into the Redux <code>createStore()</code> method.
In order to let us combine multiple reducers together, Redux provides the <code>combineReducers()</code> method. This method accepts an object as an argument in which you define properties which associate keys to specific reducer functions. The name you give to the keys will be used by Redux as the name for the associated piece of state.
Typically, it is a good practice to create a reducer for each piece of application state when they are distinct or unique in some way. For example, in a note-taking app with user authentication, one reducer could handle authentication while another handles the text and notes that the user is submitting. For such an application, we might write the <code>combineReducers()</code> method like this:
<blockquote>const rootReducer = Redux.combineReducers({<br>&nbsp;&nbsp;auth: authenticationReducer,<br>&nbsp;&nbsp;notes: notesReducer<br>});</blockquote>
Now, the key <code>notes</code> will contain all of the state associated with our notes and handled by our <code>notesReducer</code>. This is how multiple reducers can be composed to manage more complex application state. In this example, the state held in the Redux store would then be a single object containing <code>auth</code> and <code>notes</code> properties.
</section>

## Instructions
<section id='instructions'>
There are <code>counterReducer()</code> and <code>authReducer()</code> functions provided in the code editor, along with a Redux store. Finish writing the <code>rootReducer()</code> function using the <code>Redux.combineReducers()</code> method. Assign <code>counterReducer</code> to a key called <code>count</code> and <code>authReducer</code> to a key called <code>auth</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const INCREMENT = 'INCREMENT';
const DECREMENT = 'DECREMENT';

const counterReducer = (state = 0, action) => {
  switch(action.type) {
    case INCREMENT:
      return state + 1;
    case DECREMENT:
      return state - 1;
    default:
      return state;
  }
};

const LOGIN = 'LOGIN';
const LOGOUT = 'LOGOUT';

const authReducer = (state = {authenticated: false}, action) => {
  switch(action.type) {
    case LOGIN:
      return {
        authenticated: true
      }
    case LOGOUT:
      return {
        authenticated: false
      }
    default:
      return state;
  }
};

const rootReducer = // define the root reducer here

const store = Redux.createStore(rootReducer);

```

</div>



</section>

## Solution
<section id='solution'>


```js
const INCREMENT = 'INCREMENT';
const DECREMENT = 'DECREMENT';

const counterReducer = (state = 0, action) => {
  switch(action.type) {
    case INCREMENT:
      return state + 1;
    case DECREMENT:
      return state - 1;
    default:
      return state;
  }
};

const LOGIN = 'LOGIN';
const LOGOUT = 'LOGOUT';

const authReducer = (state = {authenticated: false}, action) => {
  switch(action.type) {
    case LOGIN:
      return {
        authenticated: true
      }
    case LOGOUT:
      return {
        authenticated: false
      }
    default:
      return state;
  }
};

const rootReducer = Redux.combineReducers({
  count: counterReducer,
  auth: authReducer
});

const store = Redux.createStore(rootReducer);
```

</section>
<hr>

# 11. Send Action Data to the Store

## Description
<section id='description'>
By now you've learned how to dispatch actions to the Redux store, but so far these actions have not contained any information other than a <code>type</code>. You can also send specific data along with your actions. In fact, this is very common because actions usually originate from some user interaction and tend to carry some data with them. The Redux store often needs to know about this data.
</section>

## Instructions
<section id='instructions'>
There's a basic <code>notesReducer()</code> and an <code>addNoteText()</code> action creator defined in the code editor. Finish the body of the <code>addNoteText()</code> function so that it returns an <code>action</code> object. The object should include a <code>type</code> property with a value of <code>ADD_NOTE</code>, and also a <code>text</code> property set to the <code>note</code> data that's passed into the action creator. When you call the action creator, you'll pass in specific note information that you can access for the object.
Next, finish writing the <code>switch</code> statement in the <code>notesReducer()</code>. You need to add a case that handles the <code>addNoteText()</code> actions. This case should be triggered whenever there is an action of type <code>ADD_NOTE</code> and it should return the <code>text</code> property on the incoming <code>action</code> as the new <code>state</code>.
The action is dispatched at the bottom of the code. Once you're finished, run the code and watch the console. That's all it takes to send action-specific data to the store and use it when you update store <code>state</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const ADD_NOTE = 'ADD_NOTE';

const notesReducer = (state = 'Initial State', action) => {
  switch(action.type) {
    // change code below this line

    // change code above this line
    default:
      return state;
  }
};

const addNoteText = (note) => {
  // change code below this line

  // change code above this line
};

const store = Redux.createStore(notesReducer);

console.log(store.getState());
store.dispatch(addNoteText('Hello!'));
console.log(store.getState());
```

</div>



</section>

## Solution
<section id='solution'>


```js
const ADD_NOTE = 'ADD_NOTE';

const notesReducer = (state = 'Initial State', action) => {
  switch(action.type) {
    // change code below this line
    case ADD_NOTE:
      return action.text;
    // change code above this line
    default:
      return state;
  }
};

const addNoteText = (note) => {
  // change code below this line
  return {
    type: ADD_NOTE,
    text: note
  }
  // change code above this line
};

const store = Redux.createStore(notesReducer);

console.log(store.getState());
store.dispatch(addNoteText('Hello Redux!'));
console.log(store.getState());
```

</section>
<hr>

# 12. Use Middleware to Handle Asynchronous Actions

## Description
<section id='description'>
So far these challenges have avoided discussing asynchronous actions, but they are an unavoidable part of web development. At some point you'll need to call asynchronous endpoints in your Redux app, so how do you handle these types of requests? Redux provides middleware designed specifically for this purpose, called Redux Thunk middleware. Here's a brief description how to use this with Redux.
To include Redux Thunk middleware, you pass it as an argument to <code>Redux.applyMiddleware()</code>. This statement is then provided as a second optional parameter to the <code>createStore()</code> function. Take a look at the code at the bottom of the editor to see this. Then, to create an asynchronous action, you return a function in the action creator that takes <code>dispatch</code> as an argument. Within this function, you can dispatch actions and perform asynchronous requests.
In this example, an asynchronous request is simulated with a <code>setTimeout()</code> call. It's common to dispatch an action before initiating any asynchronous behavior so that your application state knows that some data is being requested (this state could display a loading icon, for instance). Then, once you receive the data, you dispatch another action which carries the data as a payload along with information that the action is completed.
Remember that you're passing <code>dispatch</code> as a parameter to this special action creator. This is what you'll use to dispatch your actions, you simply pass the action directly to dispatch and the middleware takes care of the rest.
</section>

## Instructions
<section id='instructions'>
Write both dispatches in the <code>handleAsync()</code> action creator. Dispatch <code>requestingData()</code> before the <code>setTimeout()</code> (the simulated API call). Then, after you receive the (pretend) data, dispatch the <code>receivedData()</code> action, passing in this data. Now you know how to handle asynchronous actions in Redux. Everything else continues to behave as before.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const REQUESTING_DATA = 'REQUESTING_DATA'
const RECEIVED_DATA = 'RECEIVED_DATA'

const requestingData = () => { return {type: REQUESTING_DATA} }
const receivedData = (data) => { return {type: RECEIVED_DATA, users: data.users} }

const handleAsync = () => {
  return function(dispatch) {
    // dispatch request action here

    setTimeout(function() {
      let data = {
        users: ['Jeff', 'William', 'Alice']
      }
      // dispatch received data action here

    }, 2500);
  }
};

const defaultState = {
  fetching: false,
  users: []
};

const asyncDataReducer = (state = defaultState, action) => {
  switch(action.type) {
    case REQUESTING_DATA:
      return {
        fetching: true,
        users: []
      }
    case RECEIVED_DATA:
      return {
        fetching: false,
        users: action.users
      }
    default:
      return state;
  }
};

const store = Redux.createStore(
  asyncDataReducer,
  Redux.applyMiddleware(ReduxThunk.default)
);
```

</div>



</section>

## Solution
<section id='solution'>


```js
const REQUESTING_DATA = 'REQUESTING_DATA'
const RECEIVED_DATA = 'RECEIVED_DATA'

const requestingData = () => { return {type: REQUESTING_DATA} }
const receivedData = (data) => { return {type: RECEIVED_DATA, users: data.users} }

const handleAsync = () => {
  return function(dispatch) {
    dispatch(requestingData());
    setTimeout(function() {
      let data = {
        users: ['Jeff', 'William', 'Alice']
      }
      dispatch(receivedData(data));
    }, 2500);
  }
};

const defaultState = {
  fetching: false,
  users: []
};

const asyncDataReducer = (state = defaultState, action) => {
  switch(action.type) {
    case REQUESTING_DATA:
      return {
        fetching: true,
        users: []
      }
    case RECEIVED_DATA:
      return {
        fetching: false,
        users: action.users
      }
    default:
      return state;
  }
};

const store = Redux.createStore(
  asyncDataReducer,
  Redux.applyMiddleware(ReduxThunk.default)
);
```

</section>
<hr>

# 13. Write a Counter with Redux

## Description
<section id='description'>
Now you've learned all the core principles of Redux! You've seen how to create actions and action creators, create a Redux store, dispatch your actions against the store, and design state updates with pure reducers. You've even seen how to manage complex state with reducer composition and handle asynchronous actions. These examples are simplistic, but these concepts are the core principles of Redux. If you understand them well, you're ready to start building your own Redux app. The next challenges cover some of the details regarding <code>state</code> immutability, but first, here's a review of everything you've learned so far.
</section>

## Instructions
<section id='instructions'>
In this lesson, you'll implement a simple counter with Redux from scratch. The basics are provided in the code editor, but you'll have to fill in the details! Use the names that are provided and define <code>incAction</code> and <code>decAction</code> action creators, the <code>counterReducer()</code>, <code>INCREMENT</code> and <code>DECREMENT</code> action types, and finally the Redux <code>store</code>. Once you're finished you should be able to dispatch <code>INCREMENT</code> or <code>DECREMENT</code> actions to increment or decrement the state held in the <code>store</code>. Good luck building your first Redux app!
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const INCREMENT = null; // define a constant for increment action types
const DECREMENT = null; // define a constant for decrement action types

const counterReducer = null; // define the counter reducer which will increment or decrement the state based on the action it receives

const incAction = null; // define an action creator for incrementing

const decAction = null; // define an action creator for decrementing

const store = null; // define the Redux store here, passing in your reducers
```

</div>



</section>

## Solution
<section id='solution'>


```js
const INCREMENT = 'INCREMENT';
const DECREMENT = 'DECREMENT';

const counterReducer = (state = 0, action) => {
  switch(action.type) {
    case INCREMENT:
      return state + 1;
    case DECREMENT:
      return state - 1;
    default:
      return state;
  }
};

const incAction = () => {
  return {
    type: INCREMENT
  }
};

const decAction = () => {
  return {
    type: DECREMENT
  }
};

const store = Redux.createStore(counterReducer);
```

</section>
<hr>

# 14. Never Mutate State

## Description
<section id='description'>
These final challenges describe several methods of enforcing the key principle of state immutability in Redux. Immutable state means that you never modify state directly, instead, you return a new copy of state.
If you took a snapshot of the state of a Redux app over time, you would see something like <code>state 1</code>, <code>state 2</code>, <code>state 3</code>,<code>state 4</code>, <code>...</code> and so on where each state may be similar to the last, but each is a distinct piece of data. This immutability, in fact, is what provides such features as time-travel debugging that you may have heard about.
Redux does not actively enforce state immutability in its store or reducers, that responsibility falls on the programmer. Fortunately, JavaScript (especially ES6) provides several useful tools you can use to enforce the immutability of your state, whether it is a <code>string</code>, <code>number</code>, <code>array</code>, or <code>object</code>. Note that strings and numbers are primitive values and are immutable by nature. In other words, 3 is always 3. You cannot change the value of the number 3. An <code>array</code> or <code>object</code>, however, is mutable. In practice, your state will probably consist of an <code>array</code> or <code>object</code>, as these are useful data structures for representing many types of information.
</section>

## Instructions
<section id='instructions'>
There is a <code>store</code> and <code>reducer</code> in the code editor for managing to-do items. Finish writing the <code>ADD_TO_DO</code> case in the reducer to append a new to-do to the state. There are a few ways to accomplish this with standard JavaScript or ES6. See if you can find a way to return a new array with the item from <code>action.todo</code> appended to the end.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const ADD_TO_DO = 'ADD_TO_DO';

// A list of strings representing tasks to do:
const todos = [
  'Go to the store',
  'Clean the house',
  'Cook dinner',
  'Learn to code',
];

const immutableReducer = (state = todos, action) => {
  switch(action.type) {
    case ADD_TO_DO:
      // don't mutate state here or the tests will fail
      return
    default:
      return state;
  }
};

// an example todo argument would be 'Learn React',
const addToDo = (todo) => {
  return {
    type: ADD_TO_DO,
    todo
  }
}

const store = Redux.createStore(immutableReducer);
```

</div>



</section>

## Solution
<section id='solution'>


```js
const ADD_TO_DO = 'ADD_TO_DO';

// A list of strings representing tasks to do:
const todos = [
  'Go to the store',
  'Clean the house',
  'Cook dinner',
  'Learn to code',
];

const immutableReducer = (state = todos, action) => {
  switch(action.type) {
    case ADD_TO_DO:
      return state.concat(action.todo);
    default:
      return state;
  }
};

// an example todo argument would be 'Learn React',
const addToDo = (todo) => {
  return {
    type: ADD_TO_DO,
    todo
  }
}

const store = Redux.createStore(immutableReducer);
```

</section>
<hr>

# 15. Use the Spread Operator on Arrays

## Description
<section id='description'>
One solution from ES6 to help enforce state immutability in Redux is the spread operator: <code>...</code>. The spread operator has a variety of applications, one of which is well-suited to the previous challenge of producing a new array from an existing array. This is relatively new, but commonly used syntax. For example, if you have an array <code>myArray</code> and write:
<code>let newArray = [...myArray];</code>
<code>newArray</code> is now a clone of <code>myArray</code>. Both arrays still exist separately in memory. If you perform a mutation like <code>newArray.push(5)</code>, <code>myArray</code> doesn't change. The <code>...</code> effectively <i>spreads</i> out the values in <code>myArray</code> into a new array. To clone an array but add additional values in the new array, you could write <code>[...myArray, 'new value']</code>. This would return a new array composed of the values in <code>myArray</code> and the string <code>'new value'</code> as the last value. The spread syntax can be used multiple times in array composition like this, but it's important to note that it only makes a shallow copy of the array. That is to say, it only provides immutable array operations for one-dimensional arrays.
</section>

## Instructions
<section id='instructions'>
Use the spread operator to return a new copy of state when a to-do is added.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const immutableReducer = (state = ['Do not mutate state!'], action) => {
  switch(action.type) {
    case 'ADD_TO_DO':
      // don't mutate state here or the tests will fail
      return
    default:
      return state;
  }
};

const addToDo = (todo) => {
  return {
    type: 'ADD_TO_DO',
    todo
  }
}

const store = Redux.createStore(immutableReducer);
```

</div>



</section>

## Solution
<section id='solution'>


```js
const immutableReducer = (state = ['Do not mutate state!'], action) => {
  switch(action.type) {
    case 'ADD_TO_DO':
      return [
        ...state,
        action.todo
      ];
    default:
      return state;
  }
};

const addToDo = (todo) => {
  return {
    type: 'ADD_TO_DO',
    todo
  }
}

const store = Redux.createStore(immutableReducer);
```

</section>
<hr>

# 16. Remove an Item from an Array

## Description
<section id='description'>
Time to practice removing items from an array. The spread operator can be used here as well. Other useful JavaScript methods include <code>slice()</code> and <code>concat()</code>.
</section>

## Instructions
<section id='instructions'>
The reducer and action creator were modified to remove an item from an array based on the index of the item. Finish writing the reducer so a new state array is returned with the item at the specific index removed.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const immutableReducer = (state = [0,1,2,3,4,5], action) => {
  switch(action.type) {
    case 'REMOVE_ITEM':
      // don't mutate state here or the tests will fail
      return
    default:
      return state;
  }
};

const removeItem = (index) => {
  return {
    type: 'REMOVE_ITEM',
    index
  }
}

const store = Redux.createStore(immutableReducer);
```

</div>



</section>

## Solution
<section id='solution'>


```js
const immutableReducer = (state = [0,1,2,3,4,5], action) => {
  switch(action.type) {
    case 'REMOVE_ITEM':
      return [
        ...state.slice(0, action.index),
        ...state.slice(action.index + 1)
      ];
    default:
      return state;
  }
};

const removeItem = (index) => {
  return {
    type: 'REMOVE_ITEM',
    index
  }
}

const store = Redux.createStore(immutableReducer);
```

</section>
<hr>

# 17. Copy an Object with Object.assign

## Description
<section id='description'>
The last several challenges worked with arrays, but there are ways to help enforce state immutability when state is an <code>object</code>, too. A useful tool for handling objects is the <code>Object.assign()</code> utility. <code>Object.assign()</code> takes a target object and source objects and maps properties from the source objects to the target object. Any matching properties are overwritten by properties in the source objects. This behavior is commonly used to make shallow copies of objects by passing an empty object as the first argument followed by the object(s) you want to copy. Here's an example:
<code>const newObject = Object.assign({}, obj1, obj2);</code>
This creates <code>newObject</code> as a new <code>object</code>, which contains the properties that currently exist in <code>obj1</code> and <code>obj2</code>.
</section>

## Instructions
<section id='instructions'>
The Redux state and actions were modified to handle an <code>object</code> for the <code>state</code>. Edit the code to return a new <code>state</code> object for actions with type <code>ONLINE</code>, which set the <code>status</code> property to the string <code>online</code>. Try to use <code>Object.assign()</code> to complete the challenge.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const defaultState = {
  user: 'CamperBot',
  status: 'offline',
  friends: '732,982',
  community: 'freeCodeCamp'
};

const immutableReducer = (state = defaultState, action) => {
  switch(action.type) {
    case 'ONLINE':
      // don't mutate state here or the tests will fail
      return
    default:
      return state;
  }
};

const wakeUp = () => {
  return {
    type: 'ONLINE'
  }
};

const store = Redux.createStore(immutableReducer);
```

</div>



</section>

## Solution
<section id='solution'>


```js
const defaultState = {
  user: 'CamperBot',
  status: 'offline',
  friends: '732,982',
  community: 'freeCodeCamp'
};

const immutableReducer = (state = defaultState, action) => {
  switch(action.type) {
    case 'ONLINE':
      return Object.assign({}, state, {
        status: 'online'
      });
    default:
      return state;
  }
};

const wakeUp = () => {
  return {
    type: 'ONLINE'
  }
};

const store = Redux.createStore(immutableReducer);
```

</section>
<hr>

# React and Redux
# 1. Getting Started with React Redux

## Description
<section id='description'>
This series of challenges introduces how to use Redux with React. First, here's a review of some of the key principles of each technology. React is a view library that you provide with data, then it renders the view in an efficient, predictable way. Redux is a state management framework that you can use to simplify the management of your application's state. Typically, in a React Redux app, you create a single Redux store that manages the state of your entire app. Your React components subscribe to only the pieces of data in the store that are relevant to their role. Then, you dispatch actions directly from React components, which then trigger store updates.
Although React components can manage their own state locally, when you have a complex app, it's generally better to keep the app state in a single location with Redux. There are exceptions when individual components may have local state specific only to them. Finally, because Redux is not designed to work with React out of the box, you need to use the <code>react-redux</code> package. It provides a way for you to pass Redux <code>state</code> and <code>dispatch</code> to your React components as <code>props</code>.
Over the next few challenges, first, you'll create a simple React component which allows you to input new text messages. These are added to an array that's displayed in the view. This should be a nice review of what you learned in the React lessons. Next, you'll create a Redux store and actions that manage the state of the messages array. Finally, you'll use <code>react-redux</code> to connect the Redux store with your component, thereby extracting the local state into the Redux store.
</section>

## Instructions
<section id='instructions'>
Start with a <code>DisplayMessages</code> component. Add a constructor to this component and initialize it with a state that has two properties: <code>input</code>, that's set to an empty string, and <code>messages</code>, that's set to an empty array.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class DisplayMessages extends React.Component {
  // change code below this line

  // change code above this line
  render() {
    return <div />
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<DisplayMessages />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class DisplayMessages extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: '',
      messages: []
    }
  }
  render() {
    return <div/>
  }
};
```

</section>
<hr>

# 2. Manage State Locally First

## Description
<section id='description'>
Here you'll finish creating the <code>DisplayMessages</code> component.
</section>

## Instructions
<section id='instructions'>
First, in the <code>render()</code> method, have the component render an <code>input</code> element, <code>button</code> element, and <code>ul</code> element. When the <code>input</code> element changes, it should trigger a <code>handleChange()</code> method. Also, the <code>input</code> element should render the value of <code>input</code> that's in the component's state. The <code>button</code> element should trigger a <code>submitMessage()</code> method when it's clicked.
Second, write these two methods. The <code>handleChange()</code> method should update the <code>input</code> with what the user is typing. The <code>submitMessage()</code> method should concatenate the current message (stored in <code>input</code>) to the <code>messages</code> array in local state, and clear the value of the <code>input</code>.
Finally, use the <code>ul</code> to map over the array of <code>messages</code> and render it to the screen as a list of <code>li</code> elements.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
class DisplayMessages extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: '',
      messages: []
    }
  }
  // add handleChange() and submitMessage() methods here

  render() {
    return (
      <div>
        <h2>Type in a new Message:</h2>
        { /* render an input, button, and ul here */ }

        { /* change code above this line */ }
      </div>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<DisplayMessages />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
class DisplayMessages extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: '',
      messages: []
    }
 this.handleChange = this.handleChange.bind(this);
   this.submitMessage = this.submitMessage.bind(this);
 }
  handleChange(event) {
    this.setState({
      input: event.target.value
    });
  }
  submitMessage() {
    const currentMessage = this.state.input;
    this.setState({
      input: '',
      messages: this.state.messages.concat(currentMessage)
    });
  }
  render() {
    return (
      <div>
        <h2>Type in a new Message:</h2>
        <input
          value={this.state.input}
          onChange={this.handleChange}/><br/>
        <button onClick={this.submitMessage}>Submit</button>
        <ul>
          {this.state.messages.map( (message, idx) => {
              return (
                 <li key={idx}>{message}</li>
              )
            })
          }
        </ul>
      </div>
    );
  }
};
```

</section>
<hr>

# 3. Extract State Logic to Redux

## Description
<section id='description'>
Now that you finished the React component, you need to move the logic it's performing locally in its <code>state</code> into Redux. This is the first step to connect the simple React app to Redux. The only functionality your app has is to add new messages from the user to an unordered list. The example is simple in order to demonstrate how React and Redux work together.
</section>

## Instructions
<section id='instructions'>
First, define an action type 'ADD' and set it to a const <code>ADD</code>. Next, define an action creator <code>addMessage()</code> which creates the action to add a message. You'll need to pass a <code>message</code> to this action creator and include the message in the returned <code>action</code>.
Then create a reducer called <code>messageReducer()</code> that handles the state for the messages. The initial state should equal an empty array. This reducer should add a message to the array of messages held in state, or return the current state. Finally, create your Redux store and pass it the reducer.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
// define ADD, addMessage(), messageReducer(), and store here:

```

</div>



</section>

## Solution
<section id='solution'>


```js
const ADD = 'ADD';

const addMessage = (message) => {
  return {
    type: ADD,
    message
  }
};

const messageReducer = (state = [], action) => {
  switch (action.type) {
    case ADD:
      return [
        ...state,
        action.message
      ];
    default:
      return state;
  }
};

const store = Redux.createStore(messageReducer);
```

</section>
<hr>

# 4. Use Provider to Connect Redux to React

## Description
<section id='description'>
In the last challenge, you created a Redux store to handle the messages array and created an action for adding new messages. The next step is to provide React access to the Redux store and the actions it needs to dispatch updates. React Redux provides its <code>react-redux</code> package to help accomplish these tasks.
React Redux provides a small API with two key features: <code>Provider</code> and <code>connect</code>. Another challenge covers <code>connect</code>. The <code>Provider</code> is a wrapper component from React Redux that wraps your React app. This wrapper then allows you to access the Redux <code>store</code> and <code>dispatch</code> functions throughout your component tree. <code>Provider</code> takes two props, the Redux store and the child components of your app. Defining the <code>Provider</code> for an App component might look like this:
<blockquote>&lt;Provider store={store}&gt;<br>&nbsp;&nbsp;&lt;App/&gt;<br>&lt;/Provider&gt;</blockquote>
</section>

## Instructions
<section id='instructions'>
The code editor now shows all your Redux and React code from the past several challenges. It includes the Redux store, actions, and the <code>DisplayMessages</code> component. The only new piece is the <code>AppWrapper</code> component at the bottom. Use this top level component to render the <code>Provider</code> from <code>ReactRedux</code>, and pass the Redux store as a prop. Then render the <code>DisplayMessages</code> component as a child. Once you are finished, you should see your React component rendered to the page.
<strong>Note:</strong>&nbsp;React Redux is available as a global variable here, so you can access the Provider with dot notation. The code in the editor takes advantage of this and sets it to a constant <code>Provider</code> for you to use in the <code>AppWrapper</code> render method.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
// Redux Code:
const ADD = 'ADD';

const addMessage = (message) => {
  return {
    type: ADD,
    message
  }
};

const messageReducer = (state = [], action) => {
  switch (action.type) {
    case ADD:
      return [
        ...state,
        action.message
      ];
    default:
      return state;
  }
};



const store = Redux.createStore(messageReducer);

// React Code:

class DisplayMessages extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: '',
      messages: []
    }
    this.handleChange = this.handleChange.bind(this);
    this.submitMessage = this.submitMessage.bind(this);
  }
  handleChange(event) {
    this.setState({
      input: event.target.value
    });
  }
  submitMessage() {
    const currentMessage = this.state.input;
    this.setState({
      input: '',
      messages: this.state.messages.concat(currentMessage)
    });
  }
  render() {
    return (
      <div>
        <h2>Type in a new Message:</h2>
        <input
          value={this.state.input}
          onChange={this.handleChange}/><br/>
        <button onClick={this.submitMessage}>Submit</button>
        <ul>
          {this.state.messages.map( (message, idx) => {
              return (
                 <li key={idx}>{message}</li>
              )
            })
          }
        </ul>
      </div>
    );
  }
};

const Provider = ReactRedux.Provider;

class AppWrapper extends React.Component {
  // render the Provider here

  // change code above this line
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<AppWrapper />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
// Redux Code:
const ADD = 'ADD';

const addMessage = (message) => {
  return {
    type: ADD,
    message
  }
};

const messageReducer = (state = [], action) => {
  switch (action.type) {
    case ADD:
      return [
        ...state,
        action.message
      ];
    default:
      return state;
  }
};

const store = Redux.createStore(messageReducer);

// React Code:

class DisplayMessages extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: '',
      messages: []
    }
 this.handleChange = this.handleChange.bind(this);
 this.submitMessage = this.submitMessage.bind(this);
 }
  handleChange(event) {
    this.setState({
      input: event.target.value
    });
  }
  submitMessage() {
    const currentMessage = this.state.input;
    this.setState({
      input: '',
      messages: this.state.messages.concat(currentMessage)
    });
  }
  render() {
    return (
      <div>
        <h2>Type in a new Message:</h2>
        <input
          value={this.state.input}
          onChange={this.handleChange}/><br/>
        <button onClick={this.submitMessage}>Submit</button>
        <ul>
          {this.state.messages.map( (message, idx) => {
              return (
                 <li key={idx}>{message}</li>
              )
            })
          }
        </ul>
      </div>
    );
  }
};

const Provider = ReactRedux.Provider;

class AppWrapper extends React.Component {
  // change code below this line
  render() {
    return (
      <Provider store = {store}>
        <DisplayMessages/>
      </Provider>
    );
  }
  // change code above this line
};
```

</section>
<hr>

# 5. Map State to Props

## Description
<section id='description'>
The <code>Provider</code> component allows you to provide <code>state</code> and <code>dispatch</code> to your React components, but you must specify exactly what state and actions you want. This way, you make sure that each component only has access to the state it needs. You accomplish this by creating two functions: <code>mapStateToProps()</code> and <code>mapDispatchToProps()</code>.
In these functions, you declare what pieces of state you want to have access to and which action creators you need to be able to dispatch. Once these functions are in place, you'll see how to use the React Redux <code>connect</code> method to connect them to your components in another challenge.
<strong>Note:</strong>&nbsp;Behind the scenes, React Redux uses the <code>store.subscribe()</code> method to implement <code>mapStateToProps()</code>.
</section>

## Instructions
<section id='instructions'>
Create a function <code>mapStateToProps()</code>. This function should take <code>state</code> as an argument, then return an object which maps that state to specific property names. These properties will become accessible to your component via <code>props</code>. Since this example keeps the entire state of the app in a single array, you can pass that entire state to your component. Create a property <code>messages</code> in the object that's being returned, and set it to <code>state</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const state = [];

// change code below this line

```

</div>



</section>

## Solution
<section id='solution'>


```js
const state = [];

// change code below this line

const mapStateToProps = (state) => {
  return {
    messages: state
  }
};
```

</section>
<hr>

# 6. Map Dispatch to Props

## Description
<section id='description'>
The <code>mapDispatchToProps()</code> function is used to provide specific action creators to your React components so they can dispatch actions against the Redux store. It's similar in structure to the <code>mapStateToProps()</code> function you wrote in the last challenge. It returns an object that maps dispatch actions to property names, which become component <code>props</code>. However, instead of returning a piece of <code>state</code>, each property returns a function that calls <code>dispatch</code> with an action creator and any relevant action data. You have access to this <code>dispatch</code> because it's passed in to <code>mapDispatchToProps()</code> as a parameter when you define the function, just like you passed <code>state</code> to <code>mapStateToProps()</code>. Behind the scenes, React Redux is using Redux's <code>store.dispatch()</code> to conduct these dispatches with <code>mapDispatchToProps()</code>. This is similar to how it uses <code>store.subscribe()</code> for components that are mapped to <code>state</code>.
For example, you have a <code>loginUser()</code> action creator that takes a <code>username</code> as an action payload. The object returned from <code>mapDispatchToProps()</code> for this action creator would look something like:
<blockquote>{<br>&nbsp;&nbsp;submitLoginUser: function(username) {<br>&nbsp;&nbsp;&nbsp;&nbsp;dispatch(loginUser(username));<br>&nbsp;&nbsp;}<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
The code editor provides an action creator called <code>addMessage()</code>. Write the function <code>mapDispatchToProps()</code> that takes <code>dispatch</code> as an argument, then returns an object. The object should have a property <code>submitNewMessage</code> set to the dispatch function, which takes a parameter for the new message to add when it dispatches <code>addMessage()</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const addMessage = (message) => {
  return {
    type: 'ADD',
    message: message
  }
};

// change code below this line

```

</div>



</section>

## Solution
<section id='solution'>


```js
const addMessage = (message) => {
  return {
    type: 'ADD',
    message: message
  }
};

// change code below this line

const mapDispatchToProps = (dispatch) => {
  return {
    submitNewMessage: function(message) {
      dispatch(addMessage(message));
    }
  }
};
```

</section>
<hr>

# 7. Connect Redux to React

## Description
<section id='description'>
Now that you've written both the <code>mapStateToProps()</code> and the <code>mapDispatchToProps()</code> functions, you can use them to map <code>state</code> and <code>dispatch</code> to the <code>props</code> of one of your React components. The <code>connect</code> method from React Redux can handle this task. This method takes two optional arguments, <code>mapStateToProps()</code> and <code>mapDispatchToProps()</code>. They are optional because you may have a component that only needs access to <code>state</code> but doesn't need to dispatch any actions, or vice versa.
To use this method, pass in the functions as arguments, and immediately call the result with your component. This syntax is a little unusual and looks like:
<code>connect(mapStateToProps, mapDispatchToProps)(MyComponent)</code>
<strong>Note:</strong>&nbsp;If you want to omit one of the arguments to the <code>connect</code> method, you pass <code>null</code> in its place.
</section>

## Instructions
<section id='instructions'>
The code editor has the <code>mapStateToProps()</code> and <code>mapDispatchToProps()</code> functions and a new React component called <code>Presentational</code>. Connect this component to Redux with the <code>connect</code> method from the <code>ReactRedux</code> global object, and call it immediately on the <code>Presentational</code> component. Assign the result to a new <code>const</code> called <code>ConnectedComponent</code> that represents the connected component. That's it, now you're connected to Redux! Try changing either of <code>connect</code>'s arguments to <code>null</code> and observe the test results.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
const addMessage = (message) => {
  return {
    type: 'ADD',
    message: message
  }
};

const mapStateToProps = (state) => {
  return {
    messages: state
  }
};

const mapDispatchToProps = (dispatch) => {
  return {
    submitNewMessage: (message) => {
      dispatch(addMessage(message));
    }
  }
};

class Presentational extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return <h3>This is a Presentational Component</h3>
  }
};

const connect = ReactRedux.connect;
// change code below this line

```

</div>


### After Test
<div id='jsx-teardown'>

```js

const store = Redux.createStore(
  (state = '__INITIAL__STATE__', action) => state
);
class AppWrapper extends React.Component {
  render() {
    return (
      <ReactRedux.Provider store = {store}>
        <ConnectedComponent/>
      </ReactRedux.Provider>
    );
  }
};
ReactDOM.render(<AppWrapper />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
const addMessage = (message) => {
  return {
    type: 'ADD',
    message: message
  }
};

const mapStateToProps = (state) => {
  return {
    messages: state
  }
};

const mapDispatchToProps = (dispatch) => {
  return {
    submitNewMessage: (message) => {
      dispatch(addMessage(message));
    }
  }
};

class Presentational extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    return <h3>This is a Presentational Component</h3>
  }
};

const connect = ReactRedux.connect;
// change code below this line

const ConnectedComponent = connect(mapStateToProps, mapDispatchToProps)(Presentational);

```

</section>
<hr>

# 8. Connect Redux to the Messages App

## Description
<section id='description'>
Now that you understand how to use <code>connect</code> to connect React to Redux, you can apply what you've learned to your React component that handles messages.
In the last lesson, the component you connected to Redux was named <code>Presentational</code>, and this wasn't arbitrary. This term <i>generally</i> refers to React components that are not directly connected to Redux. They are simply responsible for the presentation of UI and do this as a function of the props they receive. By contrast, container components are connected to Redux. These are typically responsible for dispatching actions to the store and often pass store state to child components as props.
</section>

## Instructions
<section id='instructions'>
The code editor has all the code you've written in this section so far. The only change is that the React component is renamed to <code>Presentational</code>. Create a new component held in a constant called <code>Container</code> that uses <code>connect</code> to connect the <code>Presentational</code> component to Redux. Then, in the <code>AppWrapper</code>, render the React Redux <code>Provider</code> component. Pass <code>Provider</code> the Redux <code>store</code> as a prop and render <code>Container</code> as a child. Once everything is setup, you will see the messages app rendered to the page again.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
// Redux:
const ADD = 'ADD';

const addMessage = (message) => {
  return {
    type: ADD,
    message: message
  }
};

const messageReducer = (state = [], action) => {
  switch (action.type) {
    case ADD:
      return [
        ...state,
        action.message
      ];
    default:
      return state;
  }
};

const store = Redux.createStore(messageReducer);

// React:
class Presentational extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: '',
      messages: []
    }
    this.handleChange = this.handleChange.bind(this);
    this.submitMessage = this.submitMessage.bind(this);
  }
  handleChange(event) {
    this.setState({
      input: event.target.value
    });
  }
  submitMessage() {
    const currentMessage = this.state.input;
    this.setState({
      input: '',
      messages: this.state.messages.concat(currentMessage)
    });
  }
  render() {
    return (
      <div>
        <h2>Type in a new Message:</h2>
        <input
          value={this.state.input}
          onChange={this.handleChange}/><br/>
        <button onClick={this.submitMessage}>Submit</button>
        <ul>
          {this.state.messages.map( (message, idx) => {
              return (
                 <li key={idx}>{message}</li>
              )
            })
          }
        </ul>
      </div>
    );
  }
};

// React-Redux:
const mapStateToProps = (state) => {
  return { messages: state }
};

const mapDispatchToProps = (dispatch) => {
  return {
    submitNewMessage: (newMessage) => {
       dispatch(addMessage(newMessage))
    }
  }
};

const Provider = ReactRedux.Provider;
const connect = ReactRedux.connect;

// define the Container component here:


class AppWrapper extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    // complete the return statement:
    return (null);
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<AppWrapper />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
// Redux:
const ADD = 'ADD';

const addMessage = (message) => {
  return {
    type: ADD,
    message: message
  }
};

const messageReducer = (state = [], action) => {
  switch (action.type) {
    case ADD:
      return [
        ...state,
        action.message
      ];
    default:
      return state;
  }
};

const store = Redux.createStore(messageReducer);

// React:
class Presentational extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: '',
      messages: []
    }
 this.handleChange = this.handleChange.bind(this);
 this.submitMessage = this.submitMessage.bind(this);
  }
  handleChange(event) {
    this.setState({
      input: event.target.value
    });
  }
  submitMessage() {
    const currentMessage = this.state.input;
    this.setState({
      input: '',
      messages: this.state.messages.concat(currentMessage)
    });
  }
  render() {
    return (
      <div>
        <h2>Type in a new Message:</h2>
        <input
          value={this.state.input}
          onChange={this.handleChange}/><br/>
        <button onClick={this.submitMessage}>Submit</button>
        <ul>
          {this.state.messages.map( (message, idx) => {
              return (
                 <li key={idx}>{message}</li>
              )
            })
          }
        </ul>
      </div>
    );
  }
};

// React-Redux:
const mapStateToProps = (state) => {
  return { messages: state }
};

const mapDispatchToProps = (dispatch) => {
  return {
    submitNewMessage: (newMessage) => {
       dispatch(addMessage(newMessage))
    }
  }
};

const Provider = ReactRedux.Provider;
const connect = ReactRedux.connect;

// define the Container component here:
const Container = connect(mapStateToProps, mapDispatchToProps)(Presentational);

class AppWrapper extends React.Component {
  constructor(props) {
    super(props);
  }
  render() {
    // complete the return statement:
    return (
      <Provider store={store}>
        <Container/>
      </Provider>
    );
  }
};
```

</section>
<hr>

# 9. Extract Local State into Redux

## Description
<section id='description'>
You're almost done! Recall that you wrote all the Redux code so that Redux could control the state management of your React messages app. Now that Redux is connected, you need to extract the state management out of the <code>Presentational</code> component and into Redux. Currently, you have Redux connected, but you are handling the state locally within the <code>Presentational</code> component.
</section>

## Instructions
<section id='instructions'>
In the <code>Presentational</code> component, first, remove the <code>messages</code> property in the local <code>state</code>. These messages will be managed by Redux. Next, modify the <code>submitMessage()</code> method so that it dispatches <code>submitNewMessage()</code> from <code>this.props</code>, and pass in the current message input from local <code>state</code> as an argument. Because you removed <code>messages</code> from local state, remove the <code>messages</code> property from the call to <code>this.setState()</code> here as well. Finally, modify the <code>render()</code> method so that it maps over the messages received from <code>props</code> rather than <code>state</code>.
Once these changes are made, the app will continue to function the same, except Redux manages the state. This example also illustrates how a component may have local <code>state</code>: your component still tracks user input locally in its own <code>state</code>. You can see how Redux provides a useful state management framework on top of React. You achieved the same result using only React's local state at first, and this is usually possible with simple apps. However, as your apps become larger and more complex, so does your state management, and this is the problem Redux solves.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
// Redux:
const ADD = 'ADD';

const addMessage = (message) => {
  return {
    type: ADD,
    message: message
  }
};

const messageReducer = (state = [], action) => {
  switch (action.type) {
    case ADD:
      return [
        ...state,
        action.message
      ];
    default:
      return state;
  }
};

const store = Redux.createStore(messageReducer);

// React:
const Provider = ReactRedux.Provider;
const connect = ReactRedux.connect;

// Change code below this line
class Presentational extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: '',
      messages: []
    }
    this.handleChange = this.handleChange.bind(this);
    this.submitMessage = this.submitMessage.bind(this);
  }
  handleChange(event) {
    this.setState({
      input: event.target.value
    });
  }
  submitMessage() {
    this.setState({
      input: '',
      messages: this.state.messages.concat(this.state.input)
    });
  }
  render() {
    return (
      <div>
        <h2>Type in a new Message:</h2>
        <input
          value={this.state.input}
          onChange={this.handleChange}/><br/>
        <button onClick={this.submitMessage}>Submit</button>
        <ul>
          {this.state.messages.map( (message, idx) => {
              return (
                 <li key={idx}>{message}</li>
              )
            })
          }
        </ul>
      </div>
    );
  }
};
// Change code above this line

const mapStateToProps = (state) => {
  return {messages: state}
};

const mapDispatchToProps = (dispatch) => {
  return {
    submitNewMessage: (message) => {
      dispatch(addMessage(message))
    }
  }
};

const Container = connect(mapStateToProps, mapDispatchToProps)(Presentational);

class AppWrapper extends React.Component {
  render() {
    return (
      <Provider store={store}>
        <Container/>
      </Provider>
    );
  }
};
```

</div>


### After Test
<div id='jsx-teardown'>

```js
ReactDOM.render(<AppWrapper />, document.getElementById('root'))
```

</div>

</section>

## Solution
<section id='solution'>


```js
// Redux:
const ADD = 'ADD';

const addMessage = (message) => {
  return {
    type: ADD,
    message: message
  }
};

const messageReducer = (state = [], action) => {
  switch (action.type) {
    case ADD:
      return [
        ...state,
        action.message
      ];
    default:
      return state;
  }
};

const store = Redux.createStore(messageReducer);

// React:
const Provider = ReactRedux.Provider;
const connect = ReactRedux.connect;

// Change code below this line
class Presentational extends React.Component {
  constructor(props) {
    super(props);
    this.state = {
      input: ''
    }
 this.handleChange = this.handleChange.bind(this);
 this.submitMessage = this.submitMessage.bind(this);
  }
  handleChange(event) {
    this.setState({
      input: event.target.value
    });
  }
  submitMessage() {
    this.props.submitNewMessage(this.state.input);
    this.setState({
      input: ''
    });
  }
  render() {
    return (
      <div>
        <h2>Type in a new Message:</h2>
        <input
          value={this.state.input}
          onChange={this.handleChange}/><br/>
        <button onClick={this.submitMessage}>Submit</button>
        <ul>
          {this.props.messages.map( (message, idx) => {
              return (
                 <li key={idx}>{message}</li>
              )
            })
          }
        </ul>
      </div>
    );
  }
};
// Change code above this line

const mapStateToProps = (state) => {
  return {messages: state}
};

const mapDispatchToProps = (dispatch) => {
  return {
    submitNewMessage: (message) => {
      dispatch(addMessage(message))
    }
  }
};

const Container = connect(mapStateToProps, mapDispatchToProps)(Presentational);

class AppWrapper extends React.Component {
  render() {
    return (
      <Provider store={store}>
        <Container/>
      </Provider>
    );
  }
};
```

</section>
<hr>

# 10. Moving Forward From Here

## Description
<section id='description'>
Congratulations! You finished the lessons on React and Redux. There's one last item worth pointing out before you move on. Typically, you won't write React apps in a code editor like this. This challenge gives you a glimpse of what the syntax looks like if you're working with npm and a file system on your own machine. The code should look similar, except for the use of <code>import</code> statements (these pull in all of the dependencies that have been provided for you in the challenges). The "Managing Packages with npm" section covers npm in more detail.
Finally, writing React and Redux code generally requires some configuration. This can get complicated quickly. If you are interested in experimenting on your own machine, the
<a id='CRA' target ='_blank' href='https://github.com/facebookincubator/create-react-app'>Create React App</a> comes configured and ready to go.
Alternatively, you can enable Babel as a JavaScript Preprocessor in CodePen, add React and ReactDOM as external JavaScript resources, and work there as well.
</section>

## Instructions
<section id='instructions'>
Log the message <code>'Now I know React and Redux!'</code> to the console.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='jsx-seed'>

```jsx
// import React from 'react'
// import ReactDOM from 'react-dom'
// import { Provider, connect } from 'react-redux'
// import { createStore, combineReducers, applyMiddleware } from 'redux'
// import thunk from 'redux-thunk'

// import rootReducer from './redux/reducers'
// import App from './components/App'

// const store = createStore(
//   rootReducer,
//   applyMiddleware(thunk)
// );

// ReactDOM.render(
//   <Provider store={store}>
//     <App/>
//   </Provider>,
//   document.getElementById('root')
// );

// change code below this line

```

</div>



</section>

## Solution
<section id='solution'>


```js
console.log('Now I know React and Redux!');
```

</section>
<hr>

# Front End Libraries Projects
# 1. Build a Random Quote Machine

## Description
<section id='description'>
<strong>Objective:</strong> Build a <a href='https://codepen.io' target='_blank'>CodePen.io</a> app that is functionally similar to this: <a href='https://codepen.io/freeCodeCamp/full/qRZeGZ' target='_blank'>https://codepen.io/freeCodeCamp/full/qRZeGZ</a>.
Fulfill the below <a href='https://en.wikipedia.org/wiki/User_story' target='_blank'>user stories</a> and get all of the tests to pass. Give it your own personal style.
You can use any mix of HTML, JavaScript, CSS, Bootstrap, SASS, React, Redux, and jQuery to complete this project. You should use a frontend framework (like React for example) because this section is about learning frontend frameworks. Additional technologies not listed above are not recommended and using them is at your own risk. We are looking at supporting other frontend frameworks like Angular and Vue, but they are not currently supported. We will accept and try to fix all issue reports that use the suggested technology stack for this project. Happy coding!
<strong>User Story #1:</strong> I can see a wrapper element with a corresponding <code>id="quote-box"</code>.
<strong>User Story #2:</strong> Within <code>#quote-box</code>, I can see an element with a corresponding <code>id="text"</code>.
<strong>User Story #3:</strong> Within <code>#quote-box</code>, I can see an element with a corresponding <code>id="author"</code>.
<strong>User Story #4:</strong> Within <code>#quote-box</code>, I can see a clickable element with a corresponding <code>id="new-quote"</code>.
<strong>User Story #5:</strong> Within <code>#quote-box</code>, I can see a clickable <codea</code> element with a corresponding <code>id="tweet-quote"</code>.
<strong>User Story #6:</strong> On first load, my quote machine displays a random quote in the element with <code>id="text"</code>.
<strong>User Story #7:</strong> On first load, my quote machine displays the random quote's author in the element with <code>id="author"</code>.
<strong>User Story #8:</strong> When the <code>#new-quote</code> button is clicked, my quote machine should fetch a new quote and display it in the <code>#text</code> element.
<strong>User Story #9:</strong> My quote machine should fetch the new quote's author when the <code>#new-quote</code> button is clicked and display it in the <code>#author</code> element.
<strong>User Story #10:</strong> I can tweet the current quote by clicking on the <code>#tweet-quote</code> <code>a</code> element. This <code>a</code> element should include the <code>"twitter.com/intent/tweet"</code> path in its <code>href</code> attribute to tweet the current quote.
<strong>User Story #11:</strong> The <code>#quote-box</code> wrapper element should be horizontally centered. Please run tests with browser's zoom level at 100% and page maximized.
You can build your project by forking <a href='http://codepen.io/freeCodeCamp/pen/MJjpwO' target='_blank'>this CodePen pen</a>. Or you can use this CDN link to run the tests in any environment you like: <code>https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js</code>
Once you're done, submit the URL to your working project with all its tests passing.
Remember to use the <a href='https://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> method if you get stuck.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 2. Build a Markdown Previewer

## Description
<section id='description'>
<strong>Objective:</strong> Build a <a href='https://codepen.io' target='_blank'>CodePen.io</a> app that is functionally similar to this: <a href='https://codepen.io/freeCodeCamp/full/GrZVVO' target='_blank'>https://codepen.io/freeCodeCamp/full/GrZVVO</a>.
Fulfill the below <a href='https://en.wikipedia.org/wiki/User_story' target='_blank'>user stories</a> and get all of the tests to pass. Give it your own personal style.
You can use any mix of HTML, JavaScript, CSS, Bootstrap, SASS, React, Redux, and jQuery to complete this project. You should use a frontend framework (like React for example) because this section is about learning frontend frameworks. Additional technologies not listed above are not recommended and using them is at your own risk. We are looking at supporting other frontend frameworks like Angular and Vue, but they are not currently supported. We will accept and try to fix all issue reports that use the suggested technology stack for this project. Happy coding!
<strong>User Story #1:</strong> I can see a <code>textarea</code> element with a corresponding <code>id="editor"</code>.
<strong>User Story #2:</strong> I can see an element with a corresponding <code>id="preview"</code>.
<strong>User Story #3:</strong> When I enter text into the <code>#editor</code> element, the <code>#preview</code> element is updated as I type to display the content of the textarea.
<strong>User Story #4:</strong> When I enter GitHub flavored markdown into the <code>#editor</code> element, the text is rendered as HTML in the <code>#preview</code> element as I type (HINT: You don't need to parse Markdown yourself - you can import the Marked library for this: <a href='https://cdnjs.com/libraries/marked' target='_blank'>https://cdnjs.com/libraries/marked</a>).
<strong>User Story #5:</strong> When my markdown previewer first loads, the default text in the <code>#editor</code> field should contain valid markdown that represents at least one of each of the following elements: a header (H1 size), a sub header (H2 size), a link, inline code, a code block, a list item, a blockquote, an image, and bolded text.
<strong>User Story #6:</strong> When my markdown previewer first loads, the default markdown in the <code>#editor</code> field should be rendered as HTML in the <code>#preview</code> element.
<strong>Optional Bonus (you do not need to make this test pass):</strong> My markdown previewer interprets carriage returns and renders them as <code>br</code> (line break) elements.
You can build your project by forking <a href='http://codepen.io/freeCodeCamp/pen/MJjpwO' target='_blank'>this CodePen pen</a>. Or you can use this CDN link to run the tests in any environment you like: <code>https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js</code>
Once you're done, submit the URL to your working project with all its tests passing.
Remember to use the <a href='https://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> method if you get stuck.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 3. Build a Drum Machine

## Description
<section id='description'>
<strong>Objective:</strong> Build a <a href='https://codepen.io' target='_blank'>CodePen.io</a> app that is functionally similar to this: <a href='https://codepen.io/freeCodeCamp/full/MJyNMd' target='_blank'>https://codepen.io/freeCodeCamp/full/MJyNMd</a>.
Fulfill the below <a href='https://en.wikipedia.org/wiki/User_story' target='_blank'>user stories</a> and get all of the tests to pass. Give it your own personal style.
You can use any mix of HTML, JavaScript, CSS, Bootstrap, SASS, React, Redux, and jQuery to complete this project. You should use a frontend framework (like React for example) because this section is about learning frontend frameworks. Additional technologies not listed above are not recommended and using them is at your own risk. We are looking at supporting other frontend frameworks like Angular and Vue, but they are not currently supported. We will accept and try to fix all issue reports that use the suggested technology stack for this project. Happy coding!
<strong>User Story #1:</strong> I should be able to see an outer container with a corresponding <code>id="drum-machine"</code> that contains all other elements.
<strong>User Story #2:</strong> Within <code>#drum-machine</code> I can see an element with a corresponding <code>id="display"</code>.
<strong>User Story #3:</strong> Within <code>#drum-machine</code> I can see 9 clickable drum pad elements, each with a class name of <code>drum-pad</code>, a unique id that describes the audio clip the drum pad will be set up to trigger, and an inner text that corresponds to one of the following keys on the keyboard: Q, W, E, A, S, D, Z, X, C. The drum pads MUST be in this order.
<strong>User Story #4:</strong> Within each <code>.drum-pad</code>, there should be an HTML5 <code>audio</code> element which has a <code>src</code> attribute pointing to an audio clip, a class name of <code>clip</code>, and an id corresponding to the inner text of its parent <code>.drum-pad</code> (e.g. <code>id="Q"</code>, <code>id="W"</code>, <code>id="E"</code> etc.).
<strong>User Story #5:</strong> When I click on a <code>.drum-pad</code> element, the audio clip contained in its child <code>audio</code> element should be triggered.
<strong>User Story #6:</strong> When I press the trigger key associated with each <code>.drum-pad</code>, the audio clip contained in its child <code>audio</code> element should be triggered (e.g. pressing the Q key should trigger the drum pad which contains the string "Q", pressing the W key should trigger the drum pad which contains the string "W", etc.).
<strong>User Story #7:</strong> When a <code>.drum-pad</code> is triggered, a string describing the associated audio clip is displayed as the inner text of the <code>#display</code> element (each string must be unique).
You can build your project by forking <a href='http://codepen.io/freeCodeCamp/pen/MJjpwO' target='_blank'>this CodePen pen</a>. Or you can use this CDN link to run the tests in any environment you like: <code>https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js</code>
Once you're done, submit the URL to your working project with all its tests passing.
Remember to use the <a href='https://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> method if you get stuck.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 4. Build a JavaScript Calculator

## Description
<section id='description'>
<strong>Objective:</strong> Build a <a href='https://codepen.io' target='_blank'>CodePen.io</a> app that is functionally similar to this: <a href='https://codepen.io/freeCodeCamp/full/wgGVVX' target='_blank'>https://codepen.io/freeCodeCamp/full/wgGVVX</a>.
Fulfill the below <a href='https://en.wikipedia.org/wiki/User_story' target='_blank'>user stories</a> and get all of the tests to pass. Give it your own personal style.
You can use any mix of HTML, JavaScript, CSS, Bootstrap, SASS, React, Redux, and jQuery to complete this project. You should use a frontend framework (like React for example) because this section is about learning frontend frameworks. Additional technologies not listed above are not recommended and using them is at your own risk. We are looking at supporting other frontend frameworks like Angular and Vue, but they are not currently supported. We will accept and try to fix all issue reports that use the suggested technology stack for this project. Happy coding!
<strong>User Story #1:</strong> My calculator should contain a clickable element containing an <code>=</code> (equal sign) with a corresponding <code>id="equals"</code>.
<strong>User Story #2:</strong> My calculator should contain 10 clickable elements containing one number each from 0-9, with the following corresponding IDs: <code>id="zero"</code>, <code>id="one"</code>, <code>id="two"</code>, <code>id="three"</code>, <code>id="four"</code>, <code>id="five"</code>, <code>id="six"</code>, <code>id="seven"</code>, <code>id="eight"</code>, and <code>id="nine"</code>.
<strong>User Story #3:</strong> My calculator should contain 4 clickable elements each containing one of the 4 primary mathematical operators with the following corresponding IDs: <code>id="add"</code>, <code>id="subtract"</code>, <code>id="multiply"</code>, <code>id="divide"</code>.
<strong>User Story #4:</strong> My calculator should contain a clickable element containing a <code>.</code> (decimal point) symbol with a corresponding <code>id="decimal"</code>.
<strong>User Story #5:</strong> My calculator should contain a clickable element with an <code>id="clear"</code>.
<strong>User Story #6:</strong> My calculator should contain an element to display values with a corresponding <code>id="display"</code>.
<strong>User Story #7:</strong> At any time, pressing the clear button clears the input and output values, and returns the calculator to its initialized state; 0 should be shown in the element with the id of <code>display</code>.
<strong>User Story #8:</strong> As I input numbers, I should be able to see my input in the element with the id of <code>display</code>.
<strong>User Story #9:</strong> In any order, I should be able to add, subtract, multiply and divide a chain of numbers of any length, and when I hit <code>=</code>, the correct result should be shown in the element with the id of <code>display</code>.
<strong>User Story #10:</strong> When inputting numbers, my calculator should not allow a number to begin with multiple zeros.
<strong>User Story #11:</strong> When the decimal element is clicked, a <code>.</code> should append to the currently displayed value; two <code>.</code> in one number should not be accepted.
<strong>User Story #12:</strong> I should be able to perform any operation (+, -, *, /) on numbers containing decimal points.
<strong>User Story #13:</strong> If 2 or more operators are entered consecutively, the operation performed should be the last operator entered.
<strong>User Story #14:</strong> Pressing an operator immediately following <code>=</code> should start a new calculation that operates on the result of the previous evaluation.
<strong>User Story #15:</strong> My calculator should have several decimal places of precision when it comes to rounding (note that there is no exact standard, but you should be able to handle calculations like <code>2 / 7</code> with reasonable precision to at least 4 decimal places).
<strong>Note On Calculator Logic:</strong> It should be noted that there are two main schools of thought on calculator input logic: <dfn>immediate execution logic</dfn> and <dfn>formula logic</dfn>. Our example utilizes formula logic and observes order of operation precedence, immediate execution does not. Either is acceptable, but please note that depending on which you choose, your calculator may yield different results than ours for certain equations (see below example). As long as your math can be verified by another production calculator, please do not consider this a bug.
<strong>EXAMPLE:</strong> <code>3 + 5 x 6 - 2 / 4 =</code><br><ul><li><strong>Immediate Execution Logic:</strong> <code>11.5</code></li><li><strong>Formula/Expression Logic:</strong> <code>32.5</code></li></ul>
You can build your project by forking <a href='http://codepen.io/freeCodeCamp/pen/MJjpwO' target='_blank'>this CodePen pen</a>. Or you can use this CDN link to run the tests in any environment you like: <code>https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js</code>
Once you're done, submit the URL to your working project with all its tests passing.
Remember to use the <a href='https://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> method if you get stuck.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

# 5. Build a Pomodoro Clock

## Description
<section id='description'>
<strong>Objective:</strong> Build a <a href='https://codepen.io' target='_blank'>CodePen.io</a> app that is functionally similar to this: <a href='https://codepen.io/freeCodeCamp/full/XpKrrW' target='_blank'>https://codepen.io/freeCodeCamp/full/XpKrrW</a>.
Fulfill the below <a href='https://en.wikipedia.org/wiki/User_story' target='_blank'>user stories</a> and get all of the tests to pass. Give it your own personal style.
You can use any mix of HTML, JavaScript, CSS, Bootstrap, SASS, React, Redux, and jQuery to complete this project. You should use a frontend framework (like React for example) because this section is about learning frontend frameworks. Additional technologies not listed above are not recommended and using them is at your own risk. We are looking at supporting other frontend frameworks like Angular and Vue, but they are not currently supported. We will accept and try to fix all issue reports that use the suggested technology stack for this project. Happy coding!
<strong>User Story #1:</strong> I can see an element with <code>id="break-label"</code> that contains a string (e.g. "Break Length").
<strong>User Story #2:</strong> I can see an element with <code>id="session-label"</code> that contains a string (e.g. "Session Length").
<strong>User Story #3:</strong> I can see two clickable elements with corresponding IDs: <code>id="break-decrement"</code> and <code>id="session-decrement"</code>.
<strong>User Story #4:</strong> I can see two clickable elements with corresponding IDs: <code>id="break-increment"</code> and <code>id="session-increment"</code>.
<strong>User Story #5:</strong> I can see an element with a corresponding <code>id="break-length"</code>, which by default (on load) displays a value of 5.
<strong>User Story #6:</strong> I can see an element with a corresponding <code>id="session-length"</code>, which by default displays a value of 25.
<strong>User Story #7:</strong> I can see an element with a corresponding <code>id="timer-label"</code>, that contains a string indicating a session is initialized (e.g. "Session").
<strong>User Story #8:</strong> I can see an element with corresponding <code>id="time-left"</code>. NOTE: Paused or running, the value in this field should always be displayed in <code>mm:ss</code> format (i.e. 25:00).
<strong>User Story #9:</strong> I can see a clickable element with a corresponding <code>id="start_stop"</code>.
<strong>User Story #10:</strong> I can see a clickable element with a corresponding <code>id="reset"</code>.
<strong>User Story #11:</strong> When I click the element with the id of <code>reset</code>, any running timer should be stopped, the value within <code>id="break-length"</code> should return to <code>5</code>, the value within <code>id="session-length"</code> should return to 25, and the element with <code>id="time-left"</code> should reset to it's default state.
<strong>User Story #12:</strong> When I click the element with the id of <code>break-decrement</code>, the value within <code>id="break-length"</code> decrements by a value of 1, and I can see the updated value.
<strong>User Story #13:</strong> When I click the element with the id of <code>break-increment</code>, the value within <code>id="break-length"</code> increments by a value of 1, and I can see the updated value.
<strong>User Story #14:</strong> When I click the element with the id of <code>session-decrement</code>, the value within <code>id="session-length"</code> decrements by a value of 1, and I can see the updated value.
<strong>User Story #15:</strong> When I click the element with the id of <code>session-increment</code>, the value within <code>id="session-length"</code> increments by a value of 1, and I can see the updated value.
<strong>User Story #16:</strong> I should not be able to set a session or break length to <= 0.
<strong>User Story #17:</strong> I should not be able to set a session or break length to > 60.
<strong>User Story #18:</strong> When I first click the element with <code>id="start_stop"</code>, the timer should begin running from the value currently displayed in <code>id="session-length"</code>, even if the value has been incremented or decremented from the original value of 25.
<strong>User Story #19:</strong> If the timer is running, the element with the id of <code>time-left</code> should display the remaining time in <code>mm:ss</code> format (decrementing by a value of 1 and updating the display every 1000ms).
<strong>User Story #20:</strong> If the timer is running and I click the element with <code>id="start_stop"</code>, the countdown should pause.
<strong>User Story #21:</strong> If the timer is paused and I click the element with <code>id="start_stop"</code>, the countdown should resume running from the point at which it was paused.
<strong>User Story #22:</strong> When a session countdown reaches zero (NOTE: timer MUST reach 00:00), and a new countdown begins, the element with the id of <code>timer-label</code> should display a string indicating a break has begun.
<strong>User Story #23:</strong> When a session countdown reaches zero (NOTE: timer MUST reach 00:00), a new break countdown should begin, counting down from the value currently displayed in the <code>id="break-length"</code> element.
<strong>User Story #24:</strong> When a break countdown reaches zero (NOTE: timer MUST reach 00:00), and a new countdown begins, the element with the id of <code>timer-label</code> should display a string indicating a session has begun.
<strong>User Story #25:</strong> When a break countdown reaches zero (NOTE: timer MUST reach 00:00), a new session countdown should begin, counting down from the value currently displayed in the <code>id="session-length"</code> element.
<strong>User Story #26:</strong> When a countdown reaches zero (NOTE: timer MUST reach 00:00), a sound indicating that time is up should play. This should utilize an HTML5 <code>audio</code> tag and have a corresponding <code>id="beep"</code>.
<strong>User Story #27:</strong> The audio element with <code>id="beep"</code> must be 1 second or longer.
<strong>User Story #28:</strong> The audio element with id of <code>beep</code> must stop playing and be rewound to the beginning when the element with the id of <code>reset</code> is clicked.
You can build your project by forking <a href='http://codepen.io/freeCodeCamp/pen/MJjpwO' target='_blank'>this CodePen pen</a>. Or you can use this CDN link to run the tests in any environment you like: <code>https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js</code>
Once you're done, submit the URL to your working project with all its tests passing.
Remember to use the <a href='https://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> method if you get stuck.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
<hr>

