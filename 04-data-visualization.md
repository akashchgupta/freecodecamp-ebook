# Data Visualization with D3
# 1. Add Document Elements with D3

## Description
<section id='description'>
D3 has several methods that let you add and change elements in your document.
The <code>select()</code> method selects one element from the document. It takes an argument for the name of the element you want and returns an HTML node for the first element in the document that matches the name. Here's an example:
<code>const anchor = d3.select("a");</code>
The above example finds the first anchor tag on the page and saves an HTML node for it in the variable <code>anchor</code>. You can use the selection with other methods. The "d3" part of the example is a reference to the D3 object, which is how you access D3 methods.
Two other useful methods are <code>append()</code> and <code>text()</code>.
The <code>append()</code> method takes an argument for the element you want to add to the document. It appends an HTML node to a selected item, and returns a handle to that node.
The <code>text()</code> method either sets the text of the selected node, or gets the current text. To set the value, you pass a string as an argument inside the parentheses of the method.
Here's an example that selects an unordered list, appends a list item, and adds text:
<blockquote>d3.select("ul")<br>&nbsp;&nbsp;.append("li")<br>&nbsp;&nbsp;.text("Very important item");</blockquote>
D3 allows you to chain several methods together with periods to perform a number of actions in a row.
</section>

## Instructions
<section id='instructions'>
Use the <code>select</code> method to select the <code>body</code> tag in the document. Then <code>append</code> an <code>h1</code> tag to it, and add the text "Learning D3" into the <code>h1</code> element.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    // Add your code below this line



    // Add your code above this line
  </script>
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

# 2. Select a Group of Elements with D3

## Description
<section id='description'>
D3 also has the <code>selectAll()</code> method to select a group of elements. It returns an array of HTML nodes for all the items in the document that match the input string. Here's an example to select all the anchor tags in a document:
<code>const anchors = d3.selectAll("a");</code>
Like the <code>select()</code> method, <code>selectAll()</code> supports method chaining, and you can use it with other methods.
</section>

## Instructions
<section id='instructions'>
Select all of the <code>li</code> tags in the document, and change their text to "list item" by chaining the <code>.text()</code> method.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <ul>
    <li>Example</li>
    <li>Example</li>
    <li>Example</li>
  </ul>
  <script>
    // Add your code below this line



    // Add your code above this line
  </script>
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

# 3. Work with Data in D3

## Description
<section id='description'>
The D3 library focuses on a data-driven approach. When you have a set of data, you can apply D3 methods to display it on the page. Data comes in many formats, but this challenge uses a simple array of numbers.
The first step is to make D3 aware of the data. The <code>data()</code> method is used on a selection of DOM elements to attach the data to those elements. The data set is passed as an argument to the method.
A common workflow pattern is to create a new element in the document for each piece of data in the set. D3 has the <code>enter()</code> method for this purpose.
When <code>enter()</code> is combined with the <code>data()</code> method, it looks at the selected elements from the page and compares them to the number of data items in the set. If there are fewer elements than data items, it creates the missing elements.
Here is an example that selects a <code>ul</code> element and creates a new list item based on the number of entries in the array:
<blockquote>&lt;body&gt;<br>&nbsp;&nbsp;&lt;ul&gt;&lt;/ul&gt;<br>&nbsp;&nbsp;&lt;script&gt;<br>&nbsp;&nbsp;&nbsp;&nbsp;const dataset = ["a", "b", "c"];<br>&nbsp;&nbsp;&nbsp;&nbsp;d3.select("ul").selectAll("li")<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;.data(dataset)<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;.enter()<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;.append("li")<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;.text("New item");<br>&nbsp;&nbsp;&lt;/script&gt;<br>&lt;/body&gt;</blockquote>
It may seem confusing to select elements that don't exist yet. This code is telling D3 to first select the <code>ul</code> on the page. Next, select all list items, which returns an empty selection. Then the <code>data()</code> method reviews the dataset and runs the following code three times, once for each item in the array. The <code>enter()</code> method sees there are no <code>li</code> elements on the page, but it needs 3 (one for each piece of data in <code>dataset</code>). New <code>li</code> elements are appended to the <code>ul</code> and have the text "New item".
</section>

## Instructions
<section id='instructions'>
Select the <code>body</code> node, then select all <code>h2</code> elements. Have D3 create and append an <code>h2</code> tag for each item in the <code>dataset</code> array. The text in the <code>h2</code> should say "New Title". Your code should use the <code>data()</code> and <code>enter()</code> methods.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    // Add your code below this line



    // Add your code above this line
  </script>
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

# 4. Work with Dynamic Data in D3

## Description
<section id='description'>
The last two challenges cover the basics of displaying data dynamically with D3 using the <code>data()</code> and <code>enter()</code> methods. These methods take a data set and, together with the <code>append()</code> method, create a new DOM element for each entry in the data set.
In the previous challenge, you created a new <code>h2</code> element for each item in the <code>dataset</code> array, but they all contained the same text, "New Title". This is because you have not made use of the data that is bound to each of the <code>h2</code> elements.
The D3 <code>text()</code> method can take a string or a callback function as an argument:
<code>selection.text((d) => d)</code>
In the example above, the parameter <code>d</code> refers to a single entry in the dataset that a selection is bound to.
Using the current example as context, the first <code>h2</code> element is bound to 12, the second <code>h2</code> element is bound to 31, the third <code>h2</code> element is bound to 22, and so on.
</section>

## Instructions
<section id='instructions'>
Change the <code>text()</code> method so that each <code>h2</code> element displays the corresponding value from the <code>dataset</code> array with a single space and "USD". For example, the first heading should be "12 USD".
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    d3.select("body").selectAll("h2")
      .data(dataset)
      .enter()
      .append("h2")
      // Add your code below this line

      .text("New Title");

      // Add your code above this line
  </script>
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

# 5. Add Inline Styling to Elements

## Description
<section id='description'>
D3 lets you add inline CSS styles on dynamic elements with the <code>style()</code> method.
The <code>style()</code> method takes a comma-separated key-value pair as an argument. Here's an example to set the selection's text color to blue:
<code>selection.style("color","blue");</code>
</section>

## Instructions
<section id='instructions'>
Add the <code>style()</code> method to the code in the editor to make all the displayed text have a <code>font-family</code> of <code>verdana</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    d3.select("body").selectAll("h2")
      .data(dataset)
      .enter()
      .append("h2")
      .text((d) => (d + " USD"))
      // Add your code below this line



      // Add your code above this line
  </script>
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

# 6. Change Styles Based on Data

## Description
<section id='description'>
D3 is about visualization and presentation of data. It's likely you'll want to change the styling of elements based on the data. You can use a callback function in the <code>style()</code> method to change the styling for different elements.
For example, you may want to color a data point blue if has a value less than 20, and red otherwise. You can use a callback function in the <code>style()</code> method and include the conditional logic. The callback function uses the <code>d</code> parameter to represent the data point:
<blockquote>selection.style("color", (d) => {<br>&nbsp;&nbsp;/* Logic that returns the color based on a condition */<br>});</blockquote>
The <code>style()</code> method is not limited to setting the <code>color</code> - it can be used with other CSS properties as well.
</section>

## Instructions
<section id='instructions'>
Add the <code>style()</code> method to the code in the editor to set the <code>color</code> of the <code>h2</code> elements conditionally. Write the callback function so if the data value is less than 20, it returns "red", otherwise it returns "green".
<strong>Note</strong><br>You can use if-else logic, or the ternary operator.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    d3.select("body").selectAll("h2")
      .data(dataset)
      .enter()
      .append("h2")
      .text((d) => (d + " USD"))
      // Add your code below this line



      // Add your code above this line
  </script>
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

# 7. Add Classes with D3

## Description
<section id='description'>
Using a lot of inline styles on HTML elements gets hard to manage, even for smaller apps. It's easier to add a class to elements and style that class one time using CSS rules. D3 has the <code>attr()</code> method to add any HTML attribute to an element, including a class name.
The <code>attr()</code> method works the same way that <code>style()</code> does. It takes comma-separated values, and can use a callback function. Here's an example to add a class of "container" to a selection:
<code>selection.attr("class", "container");</code>

Note that the "class" parameter will remain the same whenever you need to add a class and only the "container" parameter will change.
</section>

## Instructions
<section id='instructions'>
Add the <code>attr()</code> method to the code in the editor and put a class of <code>bar</code> on the <code>div</code> elements.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style>
  .bar {
    width: 25px;
    height: 100px;
    display: inline-block;
    background-color: blue;
  }
</style>
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    d3.select("body").selectAll("div")
      .data(dataset)
      .enter()
      .append("div")
      // Add your code below this line



      // Add your code above this line
  </script>
</body>
```

</div>



</section>

## Solution
<section id='solution'>

```html
<style>
  .bar {
    width: 25px;
    height: 100px;
    display: inline-block;
    background-color: blue;
  }
</style>
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    d3.select("body").selectAll("div")
      .data(dataset)
      .enter()
      .append("div")
      // Add your code below this line
      .attr("class","bar");
      // Add your code above this line
  </script>
</body>
```
</section>
<hr>

# 8. Update the Height of an Element Dynamically

## Description
<section id='description'>
The previous challenges covered how to display data from an array and how to add CSS classes. You can combine these lessons to create a simple bar chart. There are two steps to this:
1) Create a <code>div</code> for each data point in the array
2) Give each <code>div</code> a dynamic height, using a callback function in the <code>style()</code> method that sets height equal to the data value
Recall the format to set a style using a callback function:
<code>selection.style("cssProperty", (d) => d)</code>
</section>

## Instructions
<section id='instructions'>
Add the <code>style()</code> method to the code in the editor to set the <code>height</code> property for each element. Use a callback function to return the value of the data point with the string "px" added to it.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style>
  .bar {
    width: 25px;
    height: 100px;
    display: inline-block;
    background-color: blue;
  }
</style>
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    d3.select("body").selectAll("div")
      .data(dataset)
      .enter()
      .append("div")
      .attr("class", "bar")
      // Add your code below this line



      // Add your code above this line
  </script>
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

# 9. Change the Presentation of a Bar Chart

## Description
<section id='description'>
The last challenge created a bar chart, but there are a couple of formatting changes that could improve it:
1) Add space between each bar to visually separate them, which is done by adding a margin to the CSS for the <code>bar</code> class
2) Increase the height of the bars to better show the difference in values, which is done by multiplying the value by a number to scale the height
</section>

## Instructions
<section id='instructions'>
First, add a <code>margin</code> of 2px to the <code>bar</code> class in the <code>style</code> tag. Next, change the callback function in the <code>style()</code> method so it returns a value 10 times the original data value (plus the "px").
<strong>Note</strong><br>Multiplying each data point by the <em>same</em> constant only alters the scale. It's like zooming in, and it doesn't change the meaning of the underlying data.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style>
  .bar {
    width: 25px;
    height: 100px;
    /* Add your code below this line */

    /* Add your code above this line */
    display: inline-block;
    background-color: blue;
  }
</style>
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    d3.select("body").selectAll("div")
      .data(dataset)
      .enter()
      .append("div")
      .attr("class", "bar")
      // Add your code below this line
      .style("height", (d) => (d + "px"))

      // Add your code above this line
  </script>
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

# 10. Learn About SVG in D3

## Description
<section id='description'>
SVG stands for <code>Scalable Vector Graphics</code>.
Here "scalable" means that, if you zoom in or out on an object, it would not appear pixelated. It scales with the display system, whether it's on a small mobile screen or a large TV monitor.
SVG is used to make common geometric shapes. Since D3 maps data into a visual representation, it uses SVG to create the shapes for the visualization. SVG shapes for a web page must go within an HTML <code>svg</code> tag.
CSS can be scalable when styles use relative units (such as <code>vh</code>, <code>vw</code>, or percentages), but using SVG is more flexible to build data visualizations.
</section>

## Instructions
<section id='instructions'>
Add an <code>svg</code> node to the <code>body</code> using <code>append()</code>. Give it a <code>width</code> attribute set to the provided <code>w</code> constant and a <code>height</code> attribute set to the provided <code>h</code> constant using the <code>attr()</code> or <code>style()</code> methods for each. You'll see it in the output because there's a <code>background-color</code> of pink applied to it in the <code>style</code> tag.
  <strong>Note</strong><br>When using <code>attr()</code> width and height attributes do not have units. This is the building block of scaling - the element will always have a 5:1 width to height ratio, no matter what the zoom level is.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style>
  svg {
    background-color: pink;
  }
</style>
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  // Add your code below this line



                  // Add your code above this line
  </script>
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

# 11. Display Shapes with SVG

## Description
<section id='description'>
The last challenge created an <code>svg</code> element with a given width and height, which was visible because it had a <code>background-color</code> applied to it in the <code>style</code> tag. The code made space for the given width and height.
The next step is to create a shape to put in the <code>svg</code> area. There are a number of supported shapes in SVG, such as rectangles and circles. They are used to display data. For example, a rectangle (<code>&lt;rect&gt;</code>) SVG shape could create a bar in a bar chart.
When you place a shape into the <code>svg</code> area, you can specify where it goes with <code>x</code> and <code>y</code> coordinates. The origin point of (0, 0) is in the upper-left corner. Positive values for <code>x</code> push the shape to the right, and positive values for <code>y</code> push the shape down from the origin point.
To place a shape in the middle of the 500 (width) x 100 (height) <code>svg</code> from last challenge, the <code>x</code> coordinate would be 250 and the <code>y</code> coordinate would be 50.
An SVG <code>rect</code> has four attributes. There are the <code>x</code> and <code>y</code> coordinates for where it is placed in the <code>svg</code> area. It also has a <code>height</code> and <code>width</code> to specify the size.
</section>

## Instructions
<section id='instructions'>
Add a <code>rect</code> shape to the <code>svg</code> using <code>append()</code>, and give it a <code>width</code> attribute of 25 and <code>height</code> attribute of 100. Also, give the <code>rect</code> <code>x</code> and <code>y</code> attributes each set to 0.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h)
                  // Add your code below this line



                  // Add your code above this line
  </script>
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

# 12. Create a Bar for Each Data Point in the Set

## Description
<section id='description'>
The last challenge added only one rectangle to the <code>svg</code> element to represent a bar. Here, you'll combine what you've learned so far about <code>data()</code>, <code>enter()</code>, and SVG shapes to create and append a rectangle for each data point in <code>dataset</code>.
A previous challenge showed the format for how to create and append a <code>div</code> for each item in <code>dataset</code>:
<blockquote>d3.select("body").selectAll("div")<br>&nbsp;&nbsp;.data(dataset)<br>&nbsp;&nbsp;.enter()<br>&nbsp;&nbsp;.append("div")</blockquote>
There are a few differences working with <code>rect</code> elements instead of <code>divs</code>. The <code>rects</code> must be appended to an <code>svg</code> element, not directly to the <code>body</code>. Also, you need to tell D3 where to place each <code>rect</code> within the <code>svg</code> area. The bar placement will be covered in the next challenge.
</section>

## Instructions
<section id='instructions'>
Use the <code>data()</code>, <code>enter()</code>, and <code>append()</code> methods to create and append a <code>rect</code> for each item in <code>dataset</code>. The bars should display all on top of each other, this will be fixed in the next challenge.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("rect")
       // Add your code below this line



       // Add your code above this line
       .attr("x", 0)
       .attr("y", 0)
       .attr("width", 25)
       .attr("height", 100);
  </script>
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

# 13. Dynamically Set the Coordinates for Each Bar

## Description
<section id='description'>
The last challenge created and appended a rectangle to the <code>svg</code> element for each point in <code>dataset</code> to represent a bar. Unfortunately, they were all stacked on top of each other.
The placement of a rectangle is handled by the <code>x</code> and <code>y</code> attributes. They tell D3 where to start drawing the shape in the <code>svg</code> area. The last challenge set them each to 0, so every bar was placed in the upper-left corner.
For a bar chart, all of the bars should sit on the same vertical level, which means the <code>y</code> value stays the same (at 0) for all bars. The <code>x</code> value, however, needs to change as you add new bars. Remember that larger <code>x</code> values push items farther to the right. As you go through the array elements in <code>dataset</code>, the x value should increase.
The <code>attr()</code> method in D3 accepts a callback function to dynamically set that attribute. The callback function takes two arguments, one for the data point itself (usually <code>d</code>) and one for the index of the data point in the array. The second argument for the index is optional. Here's the format:
<blockquote>selection.attr("property", (d, i) => {<br>&nbsp;&nbsp;/* <br>&nbsp;&nbsp;* d is the data point value<br>&nbsp;&nbsp;* i is the index of the data point in the array<br>&nbsp;&nbsp;*/<br>})</blockquote>
It's important to note that you do NOT need to write a <code>for</code> loop or use <code>forEach()</code> to iterate over the items in the data set. Recall that the <code>data()</code> method parses the data set, and any method that's chained after <code>data()</code> is run once for each item in the data set.
</section>

## Instructions
<section id='instructions'>
Change the <code>x</code> attribute callback function so it returns the index times 30.
<strong>Note</strong><br>Each bar has a width of 25, so increasing each <code>x</code> value by 30 adds some space between the bars. Any value greater than 25 would work in this example.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("rect")
       .data(dataset)
       .enter()
       .append("rect")
       .attr("x", (d, i) => {
         // Add your code below this line



         // Add your code above this line
       })
       .attr("y", 0)
       .attr("width", 25)
       .attr("height", 100);
  </script>
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

# 14. Dynamically Change the Height of Each Bar

## Description
<section id='description'>
The height of each bar can be set to the value of the data point in the array, similar to how the <code>x</code> value was set dynamically.
<blockquote>selection.attr("property", (d, i) => {<br>&nbsp;&nbsp;/* <br>&nbsp;&nbsp;* d is the data point value<br>&nbsp;&nbsp;* i is the index of the data point in the array<br>&nbsp;&nbsp;*/<br>})</blockquote>
</section>

## Instructions
<section id='instructions'>
Change the callback function for the <code>height</code> attribute to return the data value times 3.
<strong>Note</strong><br>Remember that multiplying all data points by the same constant scales the data (like zooming in). It helps to see the differences between bar values in this example.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("rect")
       .data(dataset)
       .enter()
       .append("rect")
       .attr("x", (d, i) => i * 30)
       .attr("y", 0)
       .attr("width", 25)
       .attr("height", (d, i) => {
         // Add your code below this line



         // Add your code above this line
       });
  </script>
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

# 15. Invert SVG Elements

## Description
<section id='description'>
You may have noticed the bar chart looked like it's upside-down, or inverted. This is because of how SVG uses (x, y) coordinates.
In SVG, the origin point for the coordinates is in the upper-left corner. An <code>x</code> coordinate of 0 places a shape on the left edge of the SVG area. A <code>y</code> coordinate of 0 places a shape on the top edge of the SVG area. Higher <code>x</code> values push the rectangle to the right. Higher <code>y</code> values push the rectangle down.
To make the bars right-side-up, you need to change the way the <code>y</code> coordinate is calculated. It needs to account for both the height of the bar and the total height of the SVG area.
The height of the SVG area is 100. If you have a data point of 0 in the set, you would want the bar to start at the bottom of the SVG area (not the top). To do this, the <code>y</code> coordinate needs a value of 100. If the data point value were 1, you would start with a <code>y</code> coordinate of 100 to set the bar at the bottom. Then you need to account for the height of the bar of 1, so the final <code>y</code> coordinate would be 99.
The <code>y</code> coordinate that is <code>y = heightOfSVG - heightOfBar</code> would place the bars right-side-up.
</section>

## Instructions
<section id='instructions'>
Change the callback function for the <code>y</code> attribute to set the bars right-side-up. Remember that the <code>height</code> of the bar is 3 times the data value <code>d</code>.
<strong>Note</strong><br>In general, the relationship is <code>y = h - m * d</code>, where <code>m</code> is the constant that scales the data points.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("rect")
       .data(dataset)
       .enter()
       .append("rect")
       .attr("x", (d, i) => i * 30)
       .attr("y", (d, i) => {
         // Add your code below this line



         // Add your code above this line
       })
       .attr("width", 25)
       .attr("height", (d, i) => 3 * d);
  </script>
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

# 16. Change the Color of an SVG Element

## Description
<section id='description'>
The bars are in the right position, but they are all the same black color. SVG has a way to change the color of the bars.
In SVG, a <code>rect</code> shape is colored with the <code>fill</code> attribute. It supports hex codes, color names, and rgb values, as well as more complex options like gradients and transparency.
</section>

## Instructions
<section id='instructions'>
Add an <code>attr()</code> method to set the "fill" of all the bars to the color "navy".
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("rect")
       .data(dataset)
       .enter()
       .append("rect")
       .attr("x", (d, i) => i * 30)
       .attr("y", (d, i) => h - 3 * d)
       .attr("width", 25)
       .attr("height", (d, i) => 3 * d)
       // Add your code below this line



       // Add your code above this line
  </script>
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

# 17. Add Labels to D3 Elements

## Description
<section id='description'>
D3 lets you label a graph element, such as a bar, using the SVG <code>text</code> element.
Like the <code>rect</code> element, a <code>text</code> element needs to have <code>x</code> and <code>y</code> attributes, to place it on the SVG canvas. It also needs to access the data to display those values.
D3 gives you a high level of control over how you label your bars.
</section>

## Instructions
<section id='instructions'>
The code in the editor already binds the data to each new <code>text</code> element. First, append <code>text</code> nodes to the <code>svg</code>. Next, add attributes for the <code>x</code> and <code>y</code> coordinates. They should be calculated the same way as the <code>rect</code> ones, except the <code>y</code> value for the <code>text</code> should make the label sit 3 units higher than the bar. Finally, use the D3 <code>text()</code> method to set the label equal to the data point value.
<strong>Note</strong><br>For the label to sit higher than the bar, decide if the <code>y</code> value for the <code>text</code> should be 3 greater or 3 less than the <code>y</code> value for the bar.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("rect")
       .data(dataset)
       .enter()
       .append("rect")
       .attr("x", (d, i) => i * 30)
       .attr("y", (d, i) => h - 3 * d)
       .attr("width", 25)
       .attr("height", (d, i) => 3 * d)
       .attr("fill", "navy");

    svg.selectAll("text")
       .data(dataset)
       .enter()
       // Add your code below this line




       // Add your code above this line
  </script>
<body>
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

# 18. Style D3 Labels

## Description
<section id='description'>
D3 methods can add styles to the bar labels. The <code>fill</code> attribute sets the color of the text for a <code>text</code> node. The <code>style()</code> method sets CSS rules for other styles, such as "font-family" or "font-size".
</section>

## Instructions
<section id='instructions'>
Set the <code>font-size</code> of the <code>text</code> elements to 25px, and the color of the text to red.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("rect")
       .data(dataset)
       .enter()
       .append("rect")
       .attr("x", (d, i) => i * 30)
       .attr("y", (d, i) => h - 3 * d)
       .attr("width", 25)
       .attr("height", (d, i) => d * 3)
       .attr("fill", "navy");

    svg.selectAll("text")
       .data(dataset)
       .enter()
       .append("text")
       .text((d) => d)
       .attr("x", (d, i) => i * 30)
       .attr("y", (d, i) => h - (3 * d) - 3)
       // Add your code below this line



       // Add your code above this line
  </script>
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

# 19. Add a Hover Effect to a D3 Element

## Description
<section id='description'>
It's possible to add effects that highlight a bar when the user hovers over it with the mouse. So far, the styling for the rectangles is applied with the built-in D3 and SVG methods, but you can use CSS as well.
You set the CSS class on the SVG elements with the <code>attr()</code> method. Then the <code>:hover</code> pseudo-class for your new class holds the style rules for any hover effects.
</section>

## Instructions
<section id='instructions'>
Use the <code>attr()</code> method to add a class of <code>bar</code> to all the <code>rect</code> elements. This changes the <code>fill</code> color of the bar to brown when you mouse over it.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style>
  .bar:hover {
    fill: brown;
  }
</style>
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("rect")
       .data(dataset)
       .enter()
       .append("rect")
       .attr("x", (d, i) => i * 30)
       .attr("y", (d, i) => h - 3 * d)
       .attr("width", 25)
       .attr("height", (d, i) => 3 * d)
       .attr("fill", "navy")
       // Add your code below this line



       // Add your code above this line

    svg.selectAll("text")
       .data(dataset)
       .enter()
       .append("text")
       .text((d) => d)
       .attr("x", (d, i) => i * 30)
       .attr("y", (d, i) => h - (3 * d) - 3);

  </script>
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

# 20. Add a Tooltip to a D3 Element

## Description
<section id='description'>
A tooltip shows more information about an item on a page when the user hovers over that item. There are several ways to add a tooltip to a visualization, this challenge uses the SVG <code>title</code> element.
<code>title</code> pairs with the <code>text()</code> method to dynamically add data to the bars.
</section>

## Instructions
<section id='instructions'>
Append a <code>title</code> element under each <code>rect</code> node. Then call the <code>text()</code> method with a callback function so the text displays the data value.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<style>
  .bar:hover {
    fill: brown;
  }
</style>
<body>
  <script>
    const dataset = [12, 31, 22, 17, 25, 18, 29, 14, 9];

    const w = 500;
    const h = 100;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("rect")
       .data(dataset)
       .enter()
       .append("rect")
       .attr("x", (d, i) => i * 30)
       .attr("y", (d, i) => h - 3 * d)
       .attr("width", 25)
       .attr("height", (d, i) => d * 3)
       .attr("fill", "navy")
       .attr("class", "bar")
       // Add your code below this line



       // Add your code above this line

    svg.selectAll("text")
       .data(dataset)
       .enter()
       .append("text")
       .text((d) => d)
       .attr("x", (d, i) => i * 30)
       .attr("y", (d, i) => h - (d * 3 + 3))

  </script>
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

# 21. Create a Scatterplot with SVG Circles

## Description
<section id='description'>
A scatter plot is another type of visualization. It usually uses circles to map data points, which have two values each. These values tie to the <code>x</code> and <code>y</code> axes, and are used to position the circle in the visualization.
SVG has a <code>circle</code> tag to create the circle shape. It works a lot like the <code>rect</code> elements you used for the bar chart.
</section>

## Instructions
<section id='instructions'>
Use the <code>data()</code>, <code>enter()</code>, and <code>append()</code> methods to bind <code>dataset</code> to new <code>circle</code> elements that are appended to the SVG canvas.
<strong>Note</strong><br>The circles won't be visible because we haven't set their attributes yet. We'll do that in the next challenge.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [
                  [ 34,    78 ],
                  [ 109,   280 ],
                  [ 310,   120 ],
                  [ 79,    411 ],
                  [ 420,   220 ],
                  [ 233,   145 ],
                  [ 333,   96 ],
                  [ 222,   333 ],
                  [ 78,    320 ],
                  [ 21,    123 ]
                ];


    const w = 500;
    const h = 500;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("circle")
       // Add your code below this line



       // Add your code above this line

  </script>
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

# 22. Add Attributes to the Circle Elements

## Description
<section id='description'>
The last challenge created the <code>circle</code> elements for each point in the <code>dataset</code>, and appended them to the SVG canvas. But D3 needs more information about the position and size of each <code>circle</code> to display them correctly.
A <code>circle</code> in SVG has three main attributes. The <code>cx</code> and <code>cy</code> attributes are the coordinates. They tell D3 where to position the <em>center</em> of the shape on the SVG canvas. The radius (<code>r</code> attribute) gives the size of the <code>circle</code>.
Just like the <code>rect</code> <code>y</code> coordinate, the <code>cy</code> attribute for a <code>circle</code> is measured from the top of the SVG canvas, not from the bottom.
All three attributes can use a callback function to set their values dynamically. Remember that all methods chained after <code>data(dataset)</code> run once per item in <code>dataset</code>. The <code>d</code> parameter in the callback function refers to the current item in <code>dataset</code>, which is an array for each point. You use bracket notation, like <code>d[0]</code>, to access the values in that array.
</section>

## Instructions
<section id='instructions'>
Add <code>cx</code>, <code>cy</code>, and <code>r</code> attributes to the <code>circle</code> elements. The <code>cx</code> value should be the first number in the array for each item in <code>dataset</code>. The <code>cy</code> value should be based off the second number in the array, but make sure to show the chart right-side-up and not inverted. The <code>r</code> value should be 5 for all circles.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [
                  [ 34,    78 ],
                  [ 109,   280 ],
                  [ 310,   120 ],
                  [ 79,    411 ],
                  [ 420,   220 ],
                  [ 233,   145 ],
                  [ 333,   96 ],
                  [ 222,   333 ],
                  [ 78,    320 ],
                  [ 21,    123 ]
                ];


    const w = 500;
    const h = 500;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("circle")
       .data(dataset)
       .enter()
       .append("circle")
       // Add your code below this line



       // Add your code above this line

  </script>
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

# 23. Add Labels to Scatter Plot Circles

## Description
<section id='description'>
You can add text to create labels for the points in a scatter plot.
The goal is to display the comma-separated values for the first (<code>x</code>) and second (<code>y</code>) fields of each item in <code>dataset</code>.
The <code>text</code> nodes need <code>x</code> and <code>y</code> attributes to position it on the SVG canvas. In this challenge, the <code>y</code> value (which determines height) can use the same value that the <code>circle</code> uses for its <code>cy</code> attribute. The <code>x</code> value can be slightly larger than the <code>cx</code> value of the <code>circle</code>, so the label is visible. This will push the label to the right of the plotted point.
</section>

## Instructions
<section id='instructions'>
Label each point on the scatter plot using the <code>text</code> elements. The text of the label should be the two values separated by a comma and a space. For example, the label for the first point is "34, 78". Set the <code>x</code> attribute so it's 5 units more than the value you used for the <code>cx</code> attribute on the <code>circle</code>. Set the <code>y</code> attribute the same way that's used for the <code>cy</code> value on the <code>circle</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [
                  [ 34,    78 ],
                  [ 109,   280 ],
                  [ 310,   120 ],
                  [ 79,    411 ],
                  [ 420,   220 ],
                  [ 233,   145 ],
                  [ 333,   96 ],
                  [ 222,   333 ],
                  [ 78,    320 ],
                  [ 21,    123 ]
                ];


    const w = 500;
    const h = 500;

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("circle")
       .data(dataset)
       .enter()
       .append("circle")
       .attr("cx", (d, i) => d[0])
       .attr("cy", (d, i) => h - d[1])
       .attr("r", 5);

    svg.selectAll("text")
       .data(dataset)
       .enter()
       .append("text")
       // Add your code below this line



       // Add your code above this line
  </script>
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

# 24. Create a Linear Scale with D3

## Description
<section id='description'>
The bar and scatter plot charts both plotted data directly onto the SVG canvas. However, if the height of a bar or one of the data points were larger than the SVG height or width values, it would go outside the SVG area.
In D3, there are scales to help plot data. <code>Scales</code> are functions that tell the program how to map a set of raw data points onto the pixels of the SVG canvas.
For example, say you have a 100x500-sized SVG canvas and you want to plot Gross Domestic Product (GDP) for a number of countries. The set of numbers would be in the billion or trillion-dollar range. You provide D3 a type of scale to tell it how to place the large GDP values into that 100x500-sized area.
It's unlikely you would plot raw data as-is. Before plotting it, you set the scale for your entire data set, so that the <code>x</code> and <code>y</code> values fit your canvas width and height.
D3 has several scale types. For a linear scale (usually used with quantitative data), there is the D3 method <code>scaleLinear()</code>:
<code> const scale = d3.scaleLinear()</code>
By default, a scale uses the identity relationship. The value of the input is the same as the value of the output. A separate challenge covers how to change this.
</section>

## Instructions
<section id='instructions'>
Change the <code>scale</code> variable to create a linear scale. Then set the <code>output</code> variable to the scale called with an input argument of 50.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    // Add your code below this line

    const scale = undefined; // Create the scale here
    const output = scale(); // Call the scale with an argument here

    // Add your code above this line

    d3.select("body")
      .append("h2")
      .text(output);

  </script>
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

# 25. Set a Domain and a Range on a Scale

## Description
<section id='description'>
By default, scales use the identity relationship - the input value maps to the output value. But scales can be much more flexible and interesting.
Say a data set has values ranging from 50 to 480. This is the input information for a scale, and is also known as the domain.
You want to map those points along the <code>x</code> axis on the SVG canvas, between 10 units and 500 units. This is the output information, which is also known as the range.
The <code>domain()</code> and <code>range()</code> methods set these values for the scale. Both methods take an array of at least two elements as an argument. Here's an example:
<blockquote>// Set a domain<br>// The domain covers the set of input values<br>scale.domain([50, 480]);<br>// Set a range<br>// The range covers the set of output values<br>scale.range([10, 500]);<br>scale(50) // Returns 10<br>scale(480) // Returns 500<br>scale(325) // Returns 323.37<br>scale(750) // Returns 807.67<br>d3.scaleLinear()</blockquote>
Notice that the scale uses the linear relationship between the domain and range values to figure out what the output should be for a given number. The minimum value in the domain (50) maps to the minimum value (10) in the range.
</section>

## Instructions
<section id='instructions'>
Create a scale and set its domain to <code>[250, 500]</code> and range to <code>[10, 150]</code>.
<strong>Note</strong><br>You can chain the <code>domain()</code> and <code>range()</code> methods onto the <code>scale</code> variable.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    // Add your code below this line
    const scale = d3.scaleLinear();



    // Add your code above this line
    const output = scale(50);
    d3.select("body")
      .append("h2")
      .text(output);
  </script>
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

# 26. Use the d3.max and d3.min Functions to Find Minimum and Maximum Values in a Dataset

## Description
<section id='description'>
The D3 methods <code>domain()</code> and <code>range()</code> set that information for your scale based on the data. There are a couple methods to make that easier.
Often when you set the domain, you'll want to use the minimum and maximum values within the data set. Trying to find these values manually, especially in a large data set, may cause errors.
D3 has two methods - <code>min()</code> and <code>max()</code> to return this information. Here's an example:
<blockquote>const exampleData = [34, 234, 73, 90, 6, 52];<br>d3.min(exampleData) // Returns 6<br>d3.max(exampleData) // Returns 234</blockquote>
A dataset may have nested arrays, like the [x, y] coordinate pairs that were in the scatter plot example. In that case, you need to tell D3 how to calculate the maximum and minimum.
Fortunately, both the <code>min()</code> and <code>max()</code> methods take a callback function.
In this example, the callback function's argument <code>d</code> is for the current inner array. The callback needs to return the element from the inner array (the x or y value) over which you want to compute the maximum or minimum. Here's an example for how to find the min and max values with an array of arrays:
<blockquote>const locationData = [[1, 7],[6, 3],[8, 3]];<br>// Returns the smallest number out of the first elements<br>const minX = d3.min(locationData, (d) => d[0]);<br>// minX compared 1, 6, and 8 and is set to 1</blockquote>
</section>

## Instructions
<section id='instructions'>
The <code>positionData</code> variable holds a 3-dimensional (3D) array. Use a D3 method to find the maximum value of the z coordinate (the third value) from the arrays and save it in the <code>output</code> variable.
<strong>Note</strong><br>Fun fact - D3 can plot 3D arrays.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const positionData = [[1, 7, -4],[6, 3, 8],[2, 9, 3]]
    // Add your code below this line

    const output = undefined; // Change this line

    // Add your code above this line

    d3.select("body")
      .append("h2")
      .text(output)
  </script>
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

# 27. Use Dynamic Scales

## Description
<section id='description'>
The D3 <code>min()</code> and <code>max()</code> methods are useful to help set the scale.
Given a complex data set, one priority is to set the scale so the visualization fits the SVG container's width and height. You want all the data plotted inside the SVG canvas so it's visible on the web page.
The example below sets the x-axis scale for scatter plot data. The <code>domain()</code> method passes information to the scale about the raw data values for the plot. The <code>range()</code> method gives it information about the actual space on the web page for the visualization.
In the example, the domain goes from 0 to the maximum in the set. It uses the <code>max()</code> method with a callback function based on the x values in the arrays. The range uses the SVG canvas' width (<code>w</code>), but it includes some padding, too. This puts space between the scatter plot dots and the edge of the SVG canvas.
<blockquote>const dataset = [<br>&nbsp;&nbsp;[ 34,    78 ],<br>&nbsp;&nbsp;[ 109,   280 ],<br>&nbsp;&nbsp;[ 310,   120 ],<br>&nbsp;&nbsp;[ 79,    411 ],<br>&nbsp;&nbsp;[ 420,   220 ],<br>&nbsp;&nbsp;[ 233,   145 ],<br>&nbsp;&nbsp;[ 333,   96 ],<br>&nbsp;&nbsp;[ 222,   333 ],<br>&nbsp;&nbsp;[ 78,    320 ],<br>&nbsp;&nbsp;[ 21,    123 ]<br>];<br>const w = 500;<br>const h = 500;<br><br>// Padding between the SVG canvas boundary and the plot<br>const padding = 30;<br>const xScale = d3.scaleLinear()<br>&nbsp;&nbsp;.domain([0, d3.max(dataset, (d) => d[0])])<br>&nbsp;&nbsp;.range([padding, w - padding]);</blockquote>
The padding may be confusing at first. Picture the x-axis as a horizontal line from 0 to 500 (the width value for the SVG canvas). Including the padding in the <code>range()</code> method forces the plot to start at 30 along that line (instead of 0), and end at 470 (instead of 500).
</section>

## Instructions
<section id='instructions'>
Use the <code>yScale</code> variable to create a linear y-axis scale. The domain should start at zero and go to the maximum y value in the set. The range should use the SVG height (<code>h</code>) and include padding.
<strong>Note</strong><br>Remember to keep the plot right-side-up. When you set the range for the y coordinates, the higher value (height minus padding) is the first argument, and the lower value is the second argument.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [
                  [ 34,    78 ],
                  [ 109,   280 ],
                  [ 310,   120 ],
                  [ 79,    411 ],
                  [ 420,   220 ],
                  [ 233,   145 ],
                  [ 333,   96 ],
                  [ 222,   333 ],
                  [ 78,    320 ],
                  [ 21,    123 ]
                ];

    const w = 500;
    const h = 500;

    // Padding between the SVG canvas boundary and the plot
    const padding = 30;

    // Create an x and y scale

    const xScale = d3.scaleLinear()
                    .domain([0, d3.max(dataset, (d) => d[0])])
                    .range([padding, w - padding]);

    // Add your code below this line

    const yScale = undefined;


    // Add your code above this line

    const output = yScale(411); // Returns 30
    d3.select("body")
      .append("h2")
      .text(output)
  </script>
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

# 28. Use a Pre-Defined Scale to Place Elements

## Description
<section id='description'>
With the scales set up, it's time to map the scatter plot again. The scales are like processing functions that turn the x and y raw data into values that fit and render correctly on the SVG canvas. They keep the data within the screen's plotting area.
You set the coordinate attribute values for an SVG shape with the scaling function. This includes <code>x</code> and <code>y</code> attributes for <code>rect</code> or <code>text</code> elements, or <code>cx</code> and <code>cy</code> for <code>circles</code>. Here's an example:
<blockquote>shape<br>&nbsp;&nbsp;.attr("x", (d) => xScale(d[0]))</blockquote>
Scales set shape coordinate attributes to place the data points onto the SVG canvas. You don't need to apply scales when you display the actual data value, for example, in the <code>text()</code> method for a tooltip or label.
</section>

## Instructions
<section id='instructions'>
Use <code>xScale</code> and <code>yScale</code> to position both the <code>circle</code> and <code>text</code> shapes onto the SVG canvas. For the <code>circles</code>, apply the scales to set the <code>cx</code> and <code>cy</code> attributes. Give them a radius of 5 units, too.
For the <code>text</code> elements, apply the scales to set the <code>x</code> and <code>y</code> attributes. The labels should be offset to the right of the dots. To do this, add 10 units to the x data value before passing it to the <code>xScale</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [
                  [ 34,     78 ],
                  [ 109,   280 ],
                  [ 310,   120 ],
                  [ 79,   411 ],
                  [ 420,   220 ],
                  [ 233,   145 ],
                  [ 333,   96 ],
                  [ 222,    333 ],
                  [ 78,    320 ],
                  [ 21,   123 ]
                ];

    const w = 500;
    const h = 500;
    const padding = 60;

    const xScale = d3.scaleLinear()
                     .domain([0, d3.max(dataset, (d) => d[0])])
                     .range([padding, w - padding]);

    const yScale = d3.scaleLinear()
                     .domain([0, d3.max(dataset, (d) => d[1])])
                     .range([h - padding, padding]);

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("circle")
       .data(dataset)
       .enter()
       .append("circle")
       // Add your code below this line



       // Add your code above this line

    svg.selectAll("text")
       .data(dataset)
       .enter()
       .append("text")
       .text((d) =>  (d[0] + ", "
 + d[1]))
       // Add your code below this line



       // Add your code above this line
  </script>
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

# 29. Add Axes to a Visualization

## Description
<section id='description'>
Another way to improve the scatter plot is to add an x-axis and a y-axis.
D3 has two methods <code>axisLeft()</code> and <code>axisBottom()</code> to render the y and x axes, respectively. (Axes is the plural form of axis). Here's an example to create the x-axis based on the <code>xScale</code> in the previous challenges:
<code>const xAxis = d3.axisBottom(xScale);</code>
The next step is to render the axis on the SVG canvas. To do so, you can use a general SVG component, the <code>g</code> element. The <code>g</code> stands for group.
Unlike <code>rect</code>, <code>circle</code>, and <code>text</code>, an axis is just a straight line when it's rendered. Because it is a simple shape, using <code>g</code> works.
The last step is to apply a <code>transform</code> attribute to position the axis on the SVG canvas in the right place. Otherwise, the line would render along the border of SVG canvas and wouldn't be visible.
SVG supports different types of <code>transforms</code>, but positioning an axis needs <code>translate</code>. When it's applied to the <code>g</code> element, it moves the whole group over and down by the given amounts. Here's an example:
<blockquote>const xAxis = d3.axisBottom(xScale);<br><br>svg.append("g")<br>&nbsp;&nbsp; .attr("transform", "translate(0, " + (h - padding) + ")")<br>&nbsp;&nbsp; .call(xAxis);</blockquote>
The above code places the x-axis at the bottom of the SVG canvas. Then it's passed as an argument to the <code>call()</code> method.
The y-axis works is the same way, except the <code>translate</code> argument is in the form (x, 0). Because <code>translate</code> is a string in the <code>attr()</code> method above, you can use concatenation to include variable values for its arguments.
</section>

## Instructions
<section id='instructions'>
The scatter plot now has an x-axis. Create a y-axis in a variable named <code>yAxis</code> using the <code>axisLeft()</code> method. Then render the axis using a <code>g</code> element. Make sure to use a <code>transform</code> attribute to translate the axis by the amount of padding units right, and 0 units down. Remember to <code>call()</code> the axis.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<body>
  <script>
    const dataset = [
                  [ 34,     78 ],
                  [ 109,   280 ],
                  [ 310,   120 ],
                  [ 79,   411 ],
                  [ 420,   220 ],
                  [ 233,   145 ],
                  [ 333,   96 ],
                  [ 222,    333 ],
                  [ 78,    320 ],
                  [ 21,   123 ]
                ];

    const w = 500;
    const h = 500;
    const padding = 60;

    const xScale = d3.scaleLinear()
                     .domain([0, d3.max(dataset, (d) => d[0])])
                     .range([padding, w - padding]);

    const yScale = d3.scaleLinear()
                     .domain([0, d3.max(dataset, (d) => d[1])])
                     .range([h - padding, padding]);

    const svg = d3.select("body")
                  .append("svg")
                  .attr("width", w)
                  .attr("height", h);

    svg.selectAll("circle")
       .data(dataset)
       .enter()
       .append("circle")
       .attr("cx", (d) => xScale(d[0]))
       .attr("cy",(d) => yScale(d[1]))
       .attr("r", (d) => 5);

    svg.selectAll("text")
       .data(dataset)
       .enter()
       .append("text")
       .text((d) =>  (d[0] + "," + d[1]))
       .attr("x", (d) => xScale(d[0] + 10))
       .attr("y", (d) => yScale(d[1]))

    const xAxis = d3.axisBottom(xScale);
    // Add your code below this line
    const yAxis = undefined;
    // Add your code above this line

    svg.append("g")
       .attr("transform", "translate(0," + (h - padding) + ")")
       .call(xAxis);

    // Add your code below this line



    // Add your code above this line

  </script>
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

# JSON APIs and Ajax
# 1. Handle Click Events with JavaScript using the onclick property

## Description
<section id='description'>
You want your code to execute only once your page has finished loading. For that purpose, you can attach a JavaScript event to the document called <code>DOMContentLoaded</code>. Here's the code that does this:
<blockquote>document.addEventListener('DOMContentLoaded',function() {<br><br>});</blockquote>
You can implement event handlers that go inside of the <code>DOMContentLoaded</code> function. You can implement an <code>onclick</code> event handler which triggers when the user clicks on the element with id <code>getMessage</code>, by adding the following code:
<blockquote>document.getElementById('getMessage').onclick=function(){};</blockquote>
</section>

## Instructions
<section id='instructions'>
Add a click event handler inside of the <code>DOMContentLoaded</code> function for the element with id of <code>getMessage</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  document.addEventListener('DOMContentLoaded',function(){
    // Add your code below this line


    // Add your code above this line
  });
</script>
<style>
  body {
    text-align: center;
    font-family: "Helvetica", sans-serif;
  }
  h1 {
    font-size: 2em;
    font-weight: bold;
  }
  .box {
    border-radius: 5px;
    background-color: #eee;
    padding: 20px 5px;
  }
  button {
    color: white;
    background-color: #4791d0;
    border-radius: 5px;
    border: 1px solid #4791d0;
    padding: 5px 10px 8px 10px;
  }
  button:hover {
    background-color: #0F5897;
    border: 1px solid #0F5897;
  }
</style>
<h1>Cat Photo Finder</h1>
<p class="message">
  The message will go here
</p>
<p>
  <button id="getMessage">
    Get Message
  </button>
</p>
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

# 2. Change Text with click Events

## Description
<section id='description'>
When the click event happens, you can use JavaScript to update an HTML element.
For example, when a user clicks the "Get Message" button, it changes the text of the element with the class <code>message</code> to say "Here is the message".
This works by adding the following code within the click event:
<code>document.getElementsByClassName('message')[0].textContent="Here is the message";</code>
</section>

## Instructions
<section id='instructions'>
Add code inside the <code>onclick</code> event handler to change the text inside the <code>message</code> element to say "Here is the message".
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  document.addEventListener('DOMContentLoaded',function(){
    document.getElementById('getMessage').onclick=function(){
      // Add your code below this line


      // Add your code above this line
    }
  });
</script>
<style>
  body {
    text-align: center;
    font-family: "Helvetica", sans-serif;
  }
  h1 {
    font-size: 2em;
    font-weight: bold;
  }
  .box {
    border-radius: 5px;
    background-color: #eee;
    padding: 20px 5px;
  }
  button {
    color: white;
    background-color: #4791d0;
    border-radius: 5px;
    border: 1px solid #4791d0;
    padding: 5px 10px 8px 10px;
  }
  button:hover {
    background-color: #0F5897;
    border: 1px solid #0F5897;
  }
</style>
<h1>Cat Photo Finder</h1>
<p class="message">
  The message will go here
</p>
<p>
  <button id="getMessage">
    Get Message
  </button>
</p>
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

# 3. Get JSON with the JavaScript XMLHttpRequest Method

## Description
<section id='description'>
You can also request data from an external source. This is where APIs come into play.
Remember that APIs - or Application Programming Interfaces - are tools that computers use to communicate with one another. You'll learn how to update HTML with the data we get from APIs using a technology called AJAX.
Most web APIs transfer data in a format called JSON. JSON stands for JavaScript Object Notation.
JSON syntax looks very similar to JavaScript object literal notation. JSON has object properties and their current values, sandwiched between a <code>{</code> and a <code>}</code>.
These properties and their values are often referred to as "key-value pairs".
However, JSON transmitted by APIs are sent as <code>bytes</code>, and your application receives it as a <code>string</code>. These can be converted into JavaScript objects, but they are not JavaScript objects by default. The <code>JSON.parse</code> method parses the string and constructs the JavaScript object described by it.
You can request the JSON from freeCodeCamp's Cat Photo API. Here's the code you can put in your click event to do this:
<blockquote>req=new XMLHttpRequest();<br>req.open("GET",'/json/cats.json',true);<br>req.send();<br>req.onload=function(){<br>&nbsp;&nbsp;json=JSON.parse(req.responseText);<br>&nbsp;&nbsp;document.getElementsByClassName('message')[0].innerHTML=JSON.stringify(json);<br>};</blockquote>
Here's a review of what each piece is doing. The JavaScript <code>XMLHttpRequest</code> object has a number of properties and methods that are used to transfer data. First, an instance of the <code>XMLHttpRequest</code> object is created and saved in the <code>req</code> variable.
Next, the <code>open</code> method initializes a request - this example is requesting data from an API, therefore is a "GET" request. The second argument for <code>open</code> is the URL of the API you are requesting data from. The third argument is a Boolean value where <code>true</code> makes it an asynchronous request.
The <code>send</code> method sends the request. Finally, the <code>onload</code> event handler parses the returned data and applies the <code>JSON.stringify</code> method to convert the JavaScript object into a string. This string is then inserted as the message text.
</section>

## Instructions
<section id='instructions'>
Update the code to create and send a "GET" request to the freeCodeCamp Cat Photo API. Then click the "Get Message" button. Your AJAX function will replace the "The message will go here" text with the raw JSON output from the API.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  document.addEventListener('DOMContentLoaded',function(){
    document.getElementById('getMessage').onclick=function(){
      // Add your code below this line


      // Add your code above this line
    };
  });
</script>
<style>
  body {
    text-align: center;
    font-family: "Helvetica", sans-serif;
  }
  h1 {
    font-size: 2em;
    font-weight: bold;
  }
  .box {
    border-radius: 5px;
    background-color: #eee;
    padding: 20px 5px;
  }
  button {
    color: white;
    background-color: #4791d0;
    border-radius: 5px;
    border: 1px solid #4791d0;
    padding: 5px 10px 8px 10px;
  }
  button:hover {
    background-color: #0F5897;
    border: 1px solid #0F5897;
  }
</style>
<h1>Cat Photo Finder</h1>
<p class="message">
  The message will go here
</p>
<p>
  <button id="getMessage">
    Get Message
  </button>
</p>
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
<script>
  document.addEventListener('DOMContentLoaded',function(){
    document.getElementById('getMessage').onclick=function(){
      const req = new XMLHttpRequest();
      req.open('GET', '/json/cats.json', true);
      req.send();
      req.onload = () => {
        const json = JSON.parse(req.responseText);
        document.getElementsByClassName('message')[0].innerHTML = JSON.stringify(json);
      };
    };
  });
</script>
<style>
  body {
    text-align: center;
    font-family: "Helvetica", sans-serif;
  }
  h1 {
    font-size: 2em;
    font-weight: bold;
  }
  .box {
    border-radius: 5px;
    background-color: #eee;
    padding: 20px 5px;
  }
  button {
    color: white;
    background-color: #4791d0;
    border-radius: 5px;
    border: 1px solid #4791d0;
    padding: 5px 10px 8px 10px;
  }
  button:hover {
    background-color: #0F5897;
    border: 1px solid #0F5897;
  }
</style>
<h1>Cat Photo Finder</h1>
<p class="message">
  The message will go here
</p>
<p>
  <button id="getMessage">
    Get Message
  </button>
</p>
```
</section>
<hr>

# 4. Access the JSON Data from an API

## Description
<section id='description'>
In the previous challenge, you saw how to get JSON data from the freeCodeCamp Cat Photo API.
Now you'll take a closer look at the returned data to better understand the JSON format. Recall some notation in JavaScript:
<blockquote>[ ] -> Square brackets represent an array<br>{ } -> Curly brackets represent an object<br>" " -> Double quotes represent a string. They are also used for key names in JSON</blockquote>
Understanding the structure of the data that an API returns is important because it influences how you retrieve the values you need.
On the right, click the "Get Message" button to load the freeCodeCamp Cat Photo API JSON into the HTML.
The first and last character you see in the JSON data are square brackets <code>[ ]</code>. This means that the returned data is an array. The second character in the JSON data is a curly <code>{</code> bracket, which starts an object. Looking closely, you can see that there are three separate objects. The JSON data is an array of three objects, where each object contains information about a cat photo.
You learned earlier that objects contain "key-value pairs" that are separated by commas. In the Cat Photo example, the first object has <code>"id":0</code> where "id" is a key and 0 is its corresponding value. Similarly, there are keys for "imageLink", "altText", and "codeNames". Each cat photo object has these same keys, but with different values.
Another interesting "key-value pair" in the first object is <code>"codeNames":["Juggernaut","Mrs. Wallace","ButterCup"]</code>. Here "codeNames" is the key and its value is an array of three strings. It's possible to have arrays of objects as well as a key with an array as a value.
Remember how to access data in arrays and objects. Arrays use bracket notation to access a specific index of an item. Objects use either bracket or dot notation to access the value of a given property. Here's an example that prints the "altText" of the first cat photo - note that the parsed JSON data in the editor is saved in a variable called <code>json</code>:
<blockquote>console.log(json[0].altText);<br>// Prints "A white cat wearing a green helmet shaped melon on its head."</blockquote>
</section>

## Instructions
<section id='instructions'>
For the cat with the "id" of 2, print to the console the second value in the <code>codeNames</code> array. You should use bracket and dot notation on the object (which is saved in the variable <code>json</code>) to access the value.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  document.addEventListener('DOMContentLoaded',function(){
    document.getElementById('getMessage').onclick=function(){
      req=new XMLHttpRequest();
      req.open("GET",'/json/cats.json',true);
      req.send();
      req.onload=function(){
        json=JSON.parse(req.responseText);
        document.getElementsByClassName('message')[0].innerHTML=JSON.stringify(json);
        // Add your code below this line


        // Add your code above this line
      };
    };
  });
</script>
<style>
  body {
    text-align: center;
    font-family: "Helvetica", sans-serif;
  }
  h1 {
    font-size: 2em;
    font-weight: bold;
  }
  .box {
    border-radius: 5px;
    background-color: #eee;
    padding: 20px 5px;
  }
  button {
    color: white;
    background-color: #4791d0;
    border-radius: 5px;
    border: 1px solid #4791d0;
    padding: 5px 10px 8px 10px;
  }
  button:hover {
    background-color: #0F5897;
    border: 1px solid #0F5897;
  }
</style>
<h1>Cat Photo Finder</h1>
<p class="message">
  The message will go here
</p>
<p>
  <button id="getMessage">
    Get Message
  </button>
</p>
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

# 5. Convert JSON Data to HTML

## Description
<section id='description'>
Now that you're getting data from a JSON API, you can display it in the HTML.
You can use a <code>forEach</code> method to loop through the data since the cat photo objects are held in an array. As you get to each item, you can modify the HTML elements.
First, declare an html variable with <code>var html = "";</code>.
Then, loop through the JSON, adding HTML to the variable that wraps the key names in <code>strong</code> tags, followed by the value. When the loop is finished, you render it.
Here's the code that does this:
<blockquote>json.forEach(function(val) {</br>&nbsp;&nbsp;var keys = Object.keys(val);</br>&nbsp;&nbsp;html += "&lt;div class = 'cat'&gt;";</br>&nbsp;&nbsp;keys.forEach(function(key) {</br>&nbsp;&nbsp;&nbsp;&nbsp;html += "&lt;strong&gt;" + key + "&lt;/strong&gt;: " + val[key] + "&lt;br&gt;";</br>&nbsp;&nbsp;});</br>&nbsp;&nbsp;html += "&lt;/div&gt;&lt;br&gt;";</br>});</blockquote>
</section>

## Instructions
<section id='instructions'>
Add a <code>forEach</code> method to loop over the JSON data and create the HTML elements to display it.
Here is some example JSON
<blockquote>[</br>&nbsp;&nbsp;{</br>&nbsp;&nbsp;&nbsp;&nbsp;"id":0,</br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"imageLink":"https://s3.amazonaws.com/freecodecamp/funny-cat.jpg",</br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"altText":"A white cat wearing a green helmet shaped melon on its head. ",</br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"codeNames":[ "Juggernaut", "Mrs. Wallace", "Buttercup"</br>&nbsp;&nbsp;&nbsp;&nbsp;]</br>&nbsp;&nbsp;}</br>]</blockquote>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  document.addEventListener('DOMContentLoaded',function(){
    document.getElementById('getMessage').onclick=function(){
      req=new XMLHttpRequest();
      req.open("GET",'/json/cats.json',true);
      req.send();
      req.onload=function(){
        json=JSON.parse(req.responseText);
        var html = "";
        // Add your code below this line



        // Add your code above this line
        document.getElementsByClassName('message')[0].innerHTML=html;
      };
    };
  });
</script>
<style>
  body {
    text-align: center;
    font-family: "Helvetica", sans-serif;
  }
  h1 {
    font-size: 2em;
    font-weight: bold;
  }
  .box {
    border-radius: 5px;
    background-color: #eee;
    padding: 20px 5px;
  }
  button {
    color: white;
    background-color: #4791d0;
    border-radius: 5px;
    border: 1px solid #4791d0;
    padding: 5px 10px 8px 10px;
  }
  button:hover {
    background-color: #0F5897;
    border: 1px solid #0F5897;
  }
</style>
<h1>Cat Photo Finder</h1>
<p class="message">
  The message will go here
</p>
<p>
  <button id="getMessage">
    Get Message
  </button>
</p>
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

# 6. Render Images from Data Sources

## Description
<section id='description'>
The last few challenges showed that each object in the JSON array contains an <code>imageLink</code> key with a value that is the URL of a cat's image.
When you're looping through these objects, you can use this <code>imageLink</code> property to display this image in an <code>img</code> element.
Here's the code that does this:
<code>html += "&lt;img src = '" + val.imageLink + "' " + "alt='" + val.altText + "'&gt;";</code>
</section>

## Instructions
<section id='instructions'>
Add code to use the <code>imageLink</code> and <code>altText</code> properties in an <code>img</code> tag.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  document.addEventListener('DOMContentLoaded',function(){
    document.getElementById('getMessage').onclick=function(){
      req=new XMLHttpRequest();
      req.open("GET",'/json/cats.json',true);
      req.send();
      req.onload=function(){
        json=JSON.parse(req.responseText);
        var html = "";
        json.forEach(function(val) {
          html += "<div class = 'cat'>";
          // Add your code below this line


          // Add your code above this line
          html += "</div><br>";
        });
        document.getElementsByClassName('message')[0].innerHTML=html;
      };
     };
  });
</script>
<style>
  body {
    text-align: center;
    font-family: "Helvetica", sans-serif;
  }
  h1 {
    font-size: 2em;
    font-weight: bold;
  }
  .box {
    border-radius: 5px;
    background-color: #eee;
    padding: 20px 5px;
  }
  button {
    color: white;
    background-color: #4791d0;
    border-radius: 5px;
    border: 1px solid #4791d0;
    padding: 5px 10px 8px 10px;
  }
  button:hover {
    background-color: #0F5897;
    border: 1px solid #0F5897;
  }
</style>
<h1>Cat Photo Finder</h1>
<p class="message">
  The message will go here
</p>
<p>
  <button id="getMessage">
    Get Message
  </button>
</p>
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

# 7. Pre-filter JSON to Get the Data You Need

## Description
<section id='description'>
If you don't want to render every cat photo you get from the freeCodeCamp Cat Photo API, you can pre-filter the JSON before looping through it.
Given that the JSON data is stored in an array, you can use the <code>filter</code> method to filter out the cat whose "id" key has a value of 1.
Here's the code to do this:
<blockquote>json = json.filter(function(val) {<br>&nbsp;&nbsp;return (val.id !== 1);<br>});</blockquote>
</section>

## Instructions
<section id='instructions'>
Add code to <code>filter</code> the json data to remove the cat with the "id" value of 1.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  document.addEventListener('DOMContentLoaded',function(){
    document.getElementById('getMessage').onclick=function(){
      req=new XMLHttpRequest();
      req.open("GET",'/json/cats.json',true);
      req.send();
      req.onload=function(){
        json=JSON.parse(req.responseText);
        var html = "";
        // Add your code below this line


        // Add your code above this line
         json.forEach(function(val) {
           html += "<div class = 'cat'>"

           html += "<img src = '" + val.imageLink + "' " + "alt='" + val.altText + "'>"

           html += "</div>"
         });
         document.getElementsByClassName('message')[0].innerHTML=html;
       };
     };
  });
</script>
<style>
  body {
    text-align: center;
    font-family: "Helvetica", sans-serif;
  }
  h1 {
    font-size: 2em;
    font-weight: bold;
  }
  .box {
    border-radius: 5px;
    background-color: #eee;
    padding: 20px 5px;
  }
  button {
    color: white;
    background-color: #4791d0;
    border-radius: 5px;
    border: 1px solid #4791d0;
    padding: 5px 10px 8px 10px;
  }
  button:hover {
    background-color: #0F5897;
    border: 1px solid #0F5897;
  }
</style>
<h1>Cat Photo Finder</h1>
<p class="message">
  The message will go here
</p>
<p>
  <button id="getMessage">
    Get Message
  </button>
</p>
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

# 8. Get Geolocation Data to Find A User's GPS Coordinates

## Description
<section id='description'>
Another cool thing you can do is access your user's current location. Every browser has a built in navigator that can give you this information.
The navigator will get the user's current longitude and latitude.
You will see a prompt to allow or block this site from knowing your current location. The challenge can be completed either way, as long as the code is correct.
By selecting allow, you will see the text on the output phone change to your latitude and longitude.
Here's code that does this:
<blockquote>if (navigator.geolocation){<br>&nbsp;&nbsp;navigator.geolocation.getCurrentPosition(function(position) {<br>&nbsp;&nbsp;&nbsp;&nbsp;document.getElementById('data').innerHTML="latitude: "+ position.coords.latitude +  "&lt;br&gt;longitude: " +  position.coords.longitude;<br>&nbsp;&nbsp;});<br>}</blockquote>
First, it checks if the <code>navigator.geolocation</code> object exists. If it does, the <code>getCurrentPosition</code> method on that object is called, which initiates an asynchronous request for the user's position. If the request is successful, the callback function in the method runs. This function accesses the <code>position</code> object's values for latitude and longitude using dot notation and updates the HTML.
</section>

## Instructions
<section id='instructions'>
Add the example code inside the <code>script</code> tags to check a user's current location and insert it into the HTML.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  // Add your code below this line


  // Add your code above this line
</script>
<h4>You are here:</h4>
<div id="data">

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

# 9. Post Data with the JavaScript XMLHttpRequest Method

## Description
<section id='description'>
In the previous examples, you received data from an external resource. You can also send data to an external resource, as long as that resource supports AJAX requests and you know the URL.
JavaScript's <code>XMLHttpRequest</code> method is also used to post data to a server. Here's an example:
<blockquote>req=new XMLHttpRequest();<br>req.open("POST",url,true);<br>req.setRequestHeader('Content-Type','text/plain');<br>req.onreadystatechange=function(){<br>&nbsp;&nbsp;if(req.readyState==4 && req.status==200){<br>&nbsp;&nbsp;&nbsp;&nbsp;document.getElementsByClassName('message')[0].innerHTML=req.responseText;<br>&nbsp;&nbsp;}<br>};<br>req.send(userName);</blockquote>
You've seen several of these methods before. Here the <code>open</code> method initializes the request as a "POST" to the given URL of the external resource, and uses the <code>true</code> Boolean to make it asynchronous.
The <code>setRequestHeader</code> method sets the value of an HTTP request header, which contains information about the sender and the request. It must be called after the <code>open</code> method, but before the <code>send</code> method. The two parameters are the name of the header and the value to set as the body of that header.
Next, the <code>onreadystatechange</code> event listener handles a change in the state of the request. A <code>readyState</code> of 4 means the operation is complete, and a <code>status</code> of 200 means it was a successful request. The document's HTML can be updated.
Finally, the <code>send</code> method sends the request with the <code>userName</code> value, which was given by the user in the <code>input</code> field.
</section>

## Instructions
<section id='instructions'>
Update the code to create and send a "POST" request. Then enter your name in input box and click "Send Message". Your AJAX function will replace "Reply from Server will be here." with the reply of the server. In this case, it is your name appended with " loves cats".
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='html-seed'>

```html
<script>
  document.addEventListener('DOMContentLoaded',function(){
    document.getElementById('sendMessage').onclick=function(){

      var userName=document.getElementById('name').value;
      // Add your code below this line


      // Add your code above this line
    };
  });
</script>
<style>
  body {
    text-align: center;
    font-family: "Helvetica", sans-serif;
  }
  h1 {
    font-size: 2em;
    font-weight: bold;
  }
  .box {
    border-radius: 5px;
    background-color: #eee;
    padding: 20px 5px;
  }
  button {
    color: white;
    background-color: #4791d0;
    border-radius: 5px;
    border: 1px solid #4791d0;
    padding: 5px 10px 8px 10px;
  }
  button:hover {
    background-color: #0F5897;
    border: 1px solid #0F5897;
  }
</style>
<h1>Cat Friends</h1>
<p class="message">
  Reply from Server will be here
</p>
<p>
  <label for="name">Your name:
    <input type="text" id="name"/>
  </label>
  <button id="sendMessage">
    Send Message
  </button>
</p>
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

# Data Visualization Projects
# 1. Visualize Data with a Bar Chart

## Description
<section id='description'>
<strong>Objective:</strong> Build a <a href='https://codepen.io' target='_blank'>CodePen.io</a> app that is functionally similar to this: <a href='https://codepen.io/freeCodeCamp/full/GrZVaM' target='_blank'>https://codepen.io/freeCodeCamp/full/GrZVaM</a>.
Fulfill the below <a href='https://en.wikipedia.org/wiki/User_story' target='_blank'>user stories</a> and get all of the tests to pass. Give it your own personal style.
You can use HTML, JavaScript, CSS, and the D3 svg-based visualization library. The tests require axes to be generated using the D3 axis property, which automatically generates ticks along the axis. These ticks are required for passing the D3 tests because their positions are used to determine alignment of graphed elements. You will find information about generating axes at <a href='https://github.com/d3/d3/blob/master/API.md#axes-d3-axis' target='_blank'>https://github.com/d3/d3/blob/master/API.md#axes-d3-axis</a>. Required (non-virtual) DOM elements are queried on the moment of each test. If you use a frontend framework (like Vue for example), the test results may be inaccurate for dynamic content. We hope to accommodate them eventually, but these frameworks are not currently supported for D3 projects.
<strong>User Story #1:</strong> My chart should have a title with a corresponding <code>id="title"</code>.
<strong>User Story #2:</strong> My chart should have a <code>g</code> element x-axis with a corresponding <code>id="x-axis"</code>.
<strong>User Story #3:</strong> My chart should have a <code>g</code> element y-axis with a corresponding <code>id="y-axis"</code>.
<strong>User Story #4:</strong> Both axes should contain multiple tick labels, each with the corresponding <code>class="tick"</code>.
<strong>User Story #5:</strong> My chart should have a <code>rect</code> element for each data point with a corresponding <code>class="bar"</code> displaying the data.
<strong>User Story #6:</strong> Each bar should have the properties <code>data-date</code> and <code>data-gdp</code> containing date and GDP values.
<strong>User Story #7:</strong> The bar elements' <code>data-date</code> properties should match the order of the provided data.
<strong>User Story #8:</strong> The bar elements' <code>data-gdp</code> properties should match the order of the provided data.
<strong>User Story #9:</strong> Each bar element's height should accurately represent the data's corresponding GDP.
<strong>User Story #10:</strong> The <code>data-date</code> attribute and its corresponding bar element should align with the corresponding value on the x-axis.
<strong>User Story #11:</strong> The <code>data-gdp</code> attribute and its corresponding bar element should align with the corresponding value on the y-axis.
<strong>User Story #12:</strong> I can mouse over an area and see a tooltip with a corresponding <code>id="tooltip"</code> which displays more information about the area.
<strong>User Story #13:</strong> My tooltip should have a <code>data-date</code> property that corresponds to the <code>data-date</code> of the active area.
Here is the dataset you will need to complete this project: <code>https://raw.githubusercontent.com/freeCodeCamp/ProjectReferenceData/master/GDP-data.json</code>
You can build your project by forking <a href='https://codepen.io/freeCodeCamp/pen/MJjpwO' target='_blank'>this CodePen pen</a>. Or you can use this CDN link to run the tests in any environment you like: <code>https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js</code>.
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

# 2. Visualize Data with a Scatterplot Graph

## Description
<section id='description'>
<strong>Objective:</strong> Build a <a href='https://codepen.io' target='_blank'>CodePen.io</a> app that is functionally similar to this: <a href='https://codepen.io/freeCodeCamp/full/bgpXyK' target='_blank'>https://codepen.io/freeCodeCamp/full/bgpXyK</a>.
Fulfill the below <a href='https://en.wikipedia.org/wiki/User_story' target='_blank'>user stories</a> and get all of the tests to pass. Give it your own personal style.
You can use HTML, JavaScript, CSS, and the D3 svg-based visualization library. The tests require axes to be generated using the D3 axis property, which automatically generates ticks along the axis. These ticks are required for passing the D3 tests because their positions are used to determine alignment of graphed elements. You will find information about generating axes at <a href='https://github.com/d3/d3/blob/master/API.md#axes-d3-axis' target='_blank'>https://github.com/d3/d3/blob/master/API.md#axes-d3-axis</a>. Required (non-virtual) DOM elements are queried on the moment of each test. If you use a frontend framework (like Vue for example), the test results may be inaccurate for dynamic content. We hope to accommodate them eventually, but these frameworks are not currently supported for D3 projects.
<strong>User Story #1:</strong> I can see a title element that has a corresponding <code>id="title"</code>.
<strong>User Story #2:</strong> I can see an x-axis that has a corresponding <code>id="x-axis"</code>.
<strong>User Story #3:</strong> I can see a y-axis that has a corresponding <code>id="y-axis"</code>.
<strong>User Story #4:</strong> I can see dots, that each have a class of <code>dot</code>, which represent the data being plotted.
<strong>User Story #5:</strong> Each dot should have the properties <code>data-xvalue</code> and <code>data-yvalue</code> containing their corresponding x and y values.
<strong>User Story #6:</strong> The <code>data-xvalue</code> and <code>data-yvalue</code> of each dot should be within the range of the actual data and in the correct data format. For <code>data-xvalue</code>, integers (full years) or Date objects are acceptable for test evaluation. For <code>data-yvalue</code> (minutes), use Date objects.
<strong>User Story #7:</strong> The <code>data-xvalue</code> and its corresponding dot should align with the corresponding point/value on the x-axis.
<strong>User Story #8:</strong> The <code>data-yvalue</code> and its corresponding dot should align with the corresponding point/value on the y-axis.
<strong>User Story #9:</strong> I can see multiple tick labels on the y-axis with <code>%M:%S</code> time format.
<strong>User Story #10:</strong> I can see multiple tick labels on the x-axis that show the year.
<strong>User Story #11:</strong> I can see that the range of the x-axis labels are within the range of the actual x-axis data.
<strong>User Story #12:</strong> I can see that the range of the y-axis labels are within the range of the actual y-axis data.
<strong>User Story #13:</strong> I can see a legend containing descriptive text that has <code>id="legend"</code>.
<strong>User Story #14:</strong> I can mouse over an area and see a tooltip with a corresponding <code>id="tooltip"</code> which displays more information about the area.
<strong>User Story #15:</strong> My tooltip should have a <code>data-year</code> property that corresponds to the <code>data-xvalue</code> of the active area.
Here is the dataset you will need to complete this project: <code>https://raw.githubusercontent.com/freeCodeCamp/ProjectReferenceData/master/cyclist-data.json</code>
You can build your project by forking <a href='https://codepen.io/freeCodeCamp/pen/MJjpwO' target='_blank'>this CodePen pen</a>. Or you can use this CDN link to run the tests in any environment you like: <code>https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js</code>
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

# 3. Visualize Data with a Heat Map

## Description
<section id='description'>
<strong>Objective:</strong> Build a <a href='https://codepen.io' target='_blank'>CodePen.io</a> app that is functionally similar to this: <a href='https://codepen.io/freeCodeCamp/full/JEXgeY' target='_blank'>https://codepen.io/freeCodeCamp/full/JEXgeY</a>.
Fulfill the below <a href='https://en.wikipedia.org/wiki/User_story' target='_blank'>user stories</a> and get all of the tests to pass. Give it your own personal style.
You can use HTML, JavaScript, CSS, and the D3 svg-based visualization library. Required (non-virtual) DOM elements are queried on the moment of each test. If you use a frontend framework (like Vue for example), the test results may be inaccurate for dynamic content. We hope to accommodate them eventually, but these frameworks are not currently supported for D3 projects.
<strong>User Story #1:</strong> My heat map should have a title with a corresponding <code>id="title"</code>.
<strong>User Story #2:</strong> My heat map should have a description with a corresponding <code>id="description"</code>.
<strong>User Story #3:</strong> My heat map should have an x-axis with a corresponding <code>id="x-axis"</code>.
<strong>User Story #4:</strong> My heat map should have a y-axis with a corresponding <code>id="y-axis"</code>.
<strong>User Story #5:</strong> My heat map should have <code>rect</code> elements with a <code>class="cell"</code> that represent the data.
<strong>User Story #6:</strong> There should be at least 4 different fill colors used for the cells.
<strong>User Story #7:</strong> Each cell will have the properties <code>data-month</code>, <code>data-year</code>, <code>data-temp</code> containing their corresponding month, year, and temperature values.
<strong>User Story #8:</strong> The <code>data-month</code>, <code>data-year</code> of each cell should be within the range of the data.
<strong>User Story #9:</strong> My heat map should have cells that align with the corresponding month on the y-axis.
<strong>User Story #10:</strong> My heat map should have cells that align with the corresponding year on the x-axis.
<strong>User Story #11:</strong> My heat map should have multiple tick labels on the y-axis with the full month name.
<strong>User Story #12:</strong> My heat map should have multiple tick labels on the x-axis with the years between 1754 and 2015.
<strong>User Story #13:</strong> My heat map should have a legend with a corresponding <code>id="legend"</code>.
<strong>User Story #14:</strong> My legend should contain <code>rect</code> elements.
<strong>User Story #15:</strong> The <code>rect</code> elements in the legend should use at least 4 different fill colors.
<strong>User Story #16:</strong> I can mouse over an area and see a tooltip with a corresponding <code>id="tooltip"</code> which displays more information about the area.
<strong>User Story #16:</strong> My tooltip should have a <code>data-year</code> property that corresponds to the <code>data-year</code> of the active area.
Here is the dataset you will need to complete this project: <code>https://raw.githubusercontent.com/freeCodeCamp/ProjectReferenceData/master/global-temperature.json</code>
You can build your project by forking <a href='https://codepen.io/freeCodeCamp/pen/MJjpwO' target='_blank'>this CodePen pen</a>. Or you can use this CDN link to run the tests in any environment you like: <code>https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js</code>
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

# 4. Visualize Data with a Choropleth Map

## Description
<section id='description'>
<strong>Objective:</strong> Build a <a href='https://codepen.io' target='_blank'>CodePen.io</a> app that is functionally similar to this: <a href='https://codepen.io/freeCodeCamp/full/EZKqza' target='_blank'>https://codepen.io/freeCodeCamp/full/EZKqza</a>.
Fulfill the below <a href='https://en.wikipedia.org/wiki/User_story' target='_blank'>user stories</a> and get all of the tests to pass. Give it your own personal style.
You can use HTML, JavaScript, CSS, and the D3 svg-based visualization library. Required (non-virtual) DOM elements are queried on the moment of each test. If you use a frontend framework (like Vue for example), the test results may be inaccurate for dynamic content. We hope to accommodate them eventually, but these frameworks are not currently supported for D3 projects.
<strong>User Story #1:</strong> My choropleth should have a title with a corresponding <code>id="title"</code>.
<strong>User Story #2:</strong> My choropleth should have a description element with a corresponding <code>id="description"</code>.
<strong>User Story #3:</strong> My choropleth should have counties with a corresponding <code>class="county"</code> that represent the data.
<strong>User Story #4:</strong> There should be at least 4 different fill colors used for the counties.
<strong>User Story #5:</strong> My counties should each have <code>data-fips</code> and <code>data-education</code> properties containing their corresponding fips and education values.
<strong>User Story #6:</strong> My choropleth should have a county for each provided data point.
<strong>User Story #7:</strong> The counties should have data-fips and data-education values that match the sample data.
<strong>User Story #8:</strong> My choropleth should have a legend with a corresponding <code>id="legend"</code>.
<strong>User Story #9:</strong> There should be at least 4 different fill colors used for the legend.
<strong>User Story #10:</strong> I can mouse over an area and see a tooltip with a corresponding <code>id="tooltip"</code> which displays more information about the area.
<strong>User Story #11:</strong> My tooltip should have a <code>data-education</code> property that corresponds to the <code>data-education</code> of the active area.
Here are the datasets you will need to complete this project:<br><ul><li><strong>US Education Data: </strong><code>https://cdn.freecodecamp.org/testable-projects-fcc/data/choropleth_map/for_user_education.json</code></li><li><strong>US County Data: </strong><code>https://cdn.freecodecamp.org/testable-projects-fcc/data/choropleth_map/counties.json</code></li></ul>
You can build your project by forking <a href='https://codepen.io/freeCodeCamp/pen/MJjpwO' target='_blank'>this CodePen pen</a>. Or you can use this CDN link to run the tests in any environment you like: <code>https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js</code>
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

# 5. Visualize Data with a Treemap Diagram

## Description
<section id='description'>
<strong>Objective:</strong> Build a <a href='https://codepen.io' target='_blank'>CodePen.io</a> app that is functionally similar to this: <a href='https://codepen.io/freeCodeCamp/full/KaNGNR' target='_blank'>https://codepen.io/freeCodeCamp/full/KaNGNR</a>.
Fulfill the below <a href='https://en.wikipedia.org/wiki/User_story' target='_blank'>user stories</a> and get all of the tests to pass. Give it your own personal style.
You can use HTML, JavaScript, CSS, and the D3 svg-based visualization library. The tests require axes to be generated using the D3 axis property, which automatically generates ticks along the axis. These ticks are required for passing the D3 tests because their positions are used to determine alignment of graphed elements. You will find information about generating axes at <a href='https://github.com/d3/d3/blob/master/API.md#axes-d3-axis' target='_blank'>https://github.com/d3/d3/blob/master/API.md#axes-d3-axis</a>. Required (non-virtual) DOM elements are queried on the moment of each test. If you use a frontend framework (like Vue for example), the test results may be inaccurate for dynamic content. We hope to accommodate them eventually, but these frameworks are not currently supported for D3 projects.
<strong>User Story #1:</strong> My tree map should have a title with a corresponding <code>id="title"</code>.
<strong>User Story #2:</strong> My tree map should have a description with a corresponding <code>id="description"</code>.
<strong>User Story #3:</strong> My tree map should have <code>rect</code> elements with a corresponding <code>class="tile"</code> that represent the data.
<strong>User Story #4:</strong> There should be at least 2 different fill colors used for the tiles.
<strong>User Story #5:</strong> Each tile should have the properties <code>data-name</code>, <code>data-category</code>, and <code>data-value</code> containing their corresponding name, category, and value.
<strong>User Story #6:</strong> The area of each tile should correspond to the data-value amount: tiles with a larger data-value should have a bigger area.
<strong>User Story #7:</strong> My tree map should have a legend with corresponding <code>id="legend"</code>.
<strong>User Story #8:</strong> My legend should have <code>rect</code> elements with a corresponding <code>class="legend-item"</code>.
<strong>User Story #9:</strong> The <code>rect</code> elements in the legend should use at least 2 different fill colors.
<strong>User Story #10:</strong> I can mouse over an area and see a tooltip with a corresponding <code>id="tooltip"</code> which displays more information about the area.
<strong>User Story #11:</strong> My tooltip should have a <code>data-value</code> property that corresponds to the <code>data-value</code> of the active area.
For this project you can use any of the following datasets:<br><ul><li><strong>Kickstarter Pledges:</strong> <code>https://cdn.freecodecamp.org/testable-projects-fcc/data/tree_map/kickstarter-funding-data.json</code></li><li><strong>Movie Sales:</strong> <code>https://cdn.freecodecamp.org/testable-projects-fcc/data/tree_map/movie-data.json</code></li><li><strong>Video Game Sales:</strong> <code>https://cdn.freecodecamp.org/testable-projects-fcc/data/tree_map/video-game-sales-data.json</code></li></ul>
You can build your project by forking <a href='https://codepen.io/freeCodeCamp/pen/MJjpwO' target='_blank'>this CodePen pen</a>. Or you can use this CDN link to run the tests in any environment you like: <code>https://cdn.freecodecamp.org/testable-projects-fcc/v1/bundle.js</code>
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

