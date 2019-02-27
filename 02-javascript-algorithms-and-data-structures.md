
# Basic JavaScript
# 1. Comment Your JavaScript Code

## Description
<section id='description'>
Comments are lines of code that JavaScript will intentionally ignore. Comments are a great way to leave notes to yourself and to other people who will later need to figure out what that code does.
There are two ways to write comments in JavaScript:
Using <code>//</code> will tell JavaScript to ignore the remainder of the text on the current line:
<blockquote>// This is an in-line comment.</blockquote>
You can make a multi-line comment beginning with <code>/*</code> and ending with <code>*/</code>:
<blockquote>/* This is a<br>multi-line comment */</blockquote>
<strong>Best Practice</strong><br>As you write code, you should regularly add comments to clarify the function of parts of your code. Good commenting can help communicate the intent of your code&mdash;both for others <em>and</em> for your future self.
</section>

## Instructions
<section id='instructions'>
Try creating one of each type of comment.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js

```

</div>



</section>

## Solution
<section id='solution'>


```js
// Fake Comment
/* Another Comment */
```

</section>
<hr>

# 2. Declare JavaScript Variables

## Description
<section id='description'>
In computer science, <dfn>data</dfn> is anything that is meaningful to the computer. JavaScript provides seven different <dfn>data types</dfn> which are <code>undefined</code>, <code>null</code>, <code>boolean</code>, <code>string</code>, <code>symbol</code>, <code>number</code>, and <code>object</code>.
For example, computers distinguish between numbers, such as the number <code>12</code>, and <code>strings</code>, such as <code>"12"</code>, <code>"dog"</code>, or <code>"123 cats"</code>, which are collections of characters. Computers can perform mathematical operations on a number, but not on a string.
<dfn>Variables</dfn> allow computers to store and manipulate data in a dynamic fashion. They do this by using a "label" to point to the data rather than using the data itself. Any of the seven data types may be stored in a variable.
<code>Variables</code> are similar to the x and y variables you use in mathematics, which means they're a simple name to represent the data we want to refer to. Computer <code>variables</code> differ from mathematical variables in that they can store different values at different times.
We tell JavaScript to create or <dfn>declare</dfn> a variable by putting the keyword <code>var</code> in front of it, like so:
<blockquote>var ourName;</blockquote>
creates a <code>variable</code> called <code>ourName</code>. In JavaScript we end statements with semicolons.
<code>Variable</code> names can be made up of numbers, letters, and <code>$</code> or <code>_</code>, but may not contain spaces or start with a number.
</section>

## Instructions
<section id='instructions'>
Use the <code>var</code> keyword to create a variable called <code>myName</code>.
<strong>Hint</strong><br>Look at the <code>ourName</code> example if you get stuck.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourName;

// Declare myName below this line

```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof myName !== "undefined"){(function(v){return v;})(myName);}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myName;
```

</section>
<hr>

# 3. Storing Values with the Assignment Operator

## Description
<section id='description'>
In JavaScript, you can store a value in a variable with the <dfn>assignment</dfn> operator.
<code>myVariable = 5;</code>
This assigns the <code>Number</code> value <code>5</code> to <code>myVariable</code>.
Assignment always goes from right to left. Everything to the right of the <code>=</code> operator is resolved before the value is assigned to the variable to the left of the operator.
<blockquote>myVar = 5;<br>myNum = myVar;</blockquote>
This assigns <code>5</code> to <code>myVar</code> and then resolves <code>myVar</code> to <code>5</code>  again and assigns it to <code>myNum</code>.
</section>

## Instructions
<section id='instructions'>
Assign the value <code>7</code> to variable <code>a</code>.
Assign the contents of <code>a</code> to variable <code>b</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var a;
var b = 2;

// Only change code below this line

```

</div>

### Before Test
<div id='js-setup'>

```js
if (typeof a != 'undefined') {
  a = undefined;
}
if (typeof b != 'undefined') {
  b = undefined;
}
```

</div>

### After Test
<div id='js-teardown'>

```js
(function(a,b){return "a = " + a + ", b = " + b;})(a,b);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var a;
var b = 2;
a = 7;
b = a;
```

</section>
<hr>

# 4. Initializing Variables with the Assignment Operator

## Description
<section id='description'>
It is common to <dfn>initialize</dfn> a variable to an initial value in the same line as it is declared.
<code>var myVar = 0;</code>
Creates a new variable called <code>myVar</code> and assigns it an initial value of <code>0</code>.
</section>

## Instructions
<section id='instructions'>
Define a variable <code>a</code> with <code>var</code> and initialize it to a value of <code>9</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourVar = 19;

// Only change code below this line

```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof a !== 'undefined') {(function(a){return "a = " + a;})(a);} else { (function() {return 'a is undefined';})(); }
```

</div>

</section>

## Solution
<section id='solution'>


```js
var a = 9;
```

</section>
<hr>

# 5. Understanding Uninitialized Variables

## Description
<section id='description'>
When JavaScript variables are declared, they have an initial value of <code>undefined</code>. If you do a mathematical operation on an <code>undefined</code> variable your result will be <code>NaN</code> which means <dfn>"Not a Number"</dfn>. If you concatenate a string with an <code>undefined</code> variable, you will get a literal <dfn>string</dfn> of <code>"undefined"</code>.
</section>

## Instructions
<section id='instructions'>
Initialize the three variables <code>a</code>, <code>b</code>, and <code>c</code> with <code>5</code>, <code>10</code>, and <code>"I am a"</code> respectively so that they will not be <code>undefined</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Initialize these three variables
var a;
var b;
var c;

// Do not change code below this line

a = a + 1;
b = b + 5;
c = c + " String!";

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(a,b,c){ return "a = " + a + ", b = " + b + ", c = '" + c + "'"; })(a,b,c);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var a = 5;
var b = 10;
var c = "I am a";
a = a + 1;
b = b + 5;
c = c + " String!";
```

</section>
<hr>

# 6. Understanding Case Sensitivity in Variables

## Description
<section id='description'>
In JavaScript all variables and function names are case sensitive. This means that capitalization matters.
<code>MYVAR</code> is not the same as <code>MyVar</code> nor <code>myvar</code>. It is possible to have multiple distinct variables with the same name but different casing. It is strongly recommended that for the sake of clarity, you <em>do not</em> use this language feature.
<h4>Best Practice</h4>
Write variable names in JavaScript in <dfn>camelCase</dfn>. In <dfn>camelCase</dfn>, multi-word variable names have the first word in lowercase and the first letter of each subsequent word is capitalized.
<strong>Examples:</strong>
<blockquote>var someVariable;<br>var anotherVariableName;<br>var thisVariableNameIsSoLong;</blockquote>
</section>

## Instructions
<section id='instructions'>
Modify the existing declarations and assignments so their names use <dfn>camelCase</dfn>.<br>Do not create any new variables.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Declarations
var StUdLyCapVaR;
var properCamelCase;
var TitleCaseOver;

// Assignments
STUDLYCAPVAR = 10;
PRoperCAmelCAse = "A String";
tITLEcASEoVER = 9000;
```

</div>



</section>

## Solution
<section id='solution'>


```js
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;
```

</section>
<hr>

# 7. Add Two Numbers with JavaScript

## Description
<section id='description'>
<code>Number</code> is a data type in JavaScript which represents numeric data.
Now let's try to add two numbers using JavaScript.
JavaScript uses the <code>+</code> symbol as an addition operation when placed between two numbers.
<strong>Example:</strong>
<blockquote>myVar = 5 + 10; // assigned 15</blockquote>
</section>

## Instructions
<section id='instructions'>
Change the <code>0</code> so that sum will equal <code>20</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var sum = 10 + 0;

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return 'sum = '+z;})(sum);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var sum = 10 + 10;
```

</section>
<hr>

# 8. Subtract One Number from Another with JavaScript

## Description
<section id='description'>
We can also subtract one number from another.
JavaScript uses the <code>-</code> symbol for subtraction.

<strong>Example</strong>
<blockquote>myVar = 12 - 6; // assigned 6</blockquote>

</section>

## Instructions
<section id='instructions'>
Change the <code>0</code> so the difference is <code>12</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var difference = 45 - 0;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return 'difference = '+z;})(difference);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var difference = 45 - 33;
```

</section>
<hr>

# 9. Multiply Two Numbers with JavaScript

## Description
<section id='description'>
We can also multiply one number by another.
JavaScript uses the <code>*</code> symbol for multiplication of two numbers.

<strong>Example</strong>
<blockquote>myVar = 13 * 13; // assigned 169</blockquote>

</section>

## Instructions
<section id='instructions'>
Change the <code>0</code> so that product will equal <code>80</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var product = 8 * 0;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return 'product = '+z;})(product);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var product = 8 * 10;
```

</section>
<hr>

# 10. Divide One Number by Another with JavaScript

## Description
<section id='description'>
We can also divide one number by another.
JavaScript uses the <code>/</code> symbol for division.

<strong>Example</strong>
<blockquote>myVar = 16 / 2; // assigned 8</blockquote>

</section>

## Instructions
<section id='instructions'>
Change the <code>0</code> so that the <code>quotient</code> is equal to <code>2</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var quotient = 66 / 0;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return 'quotient = '+z;})(quotient);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var quotient = 66 / 33;
```

</section>
<hr>

# 11. Increment a Number with JavaScript

## Description
<section id='description'>
You can easily <dfn>increment</dfn> or add one to a variable with the <code>++</code> operator.
<code>i++;</code>
is the equivalent of
<code>i = i + 1;</code>
<strong>Note</strong><br>The entire line becomes <code>i++;</code>, eliminating the need for the equal sign.
</section>

## Instructions
<section id='instructions'>
Change the code to use the <code>++</code> operator on <code>myVar</code>.
<strong>Hint</strong><br>Learn more about <a href="https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Operators/Arithmetic_Operators#Increment_()" target="_blank">Arithmetic operators - Increment (++)</a>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var myVar = 87;

// Only change code below this line
myVar = myVar + 1;

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return 'myVar = ' + z;})(myVar);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myVar = 87;
myVar++;
```

</section>
<hr>

# 12. Decrement a Number with JavaScript

## Description
<section id='description'>
You can easily <dfn>decrement</dfn> or decrease a variable by one with the <code>--</code> operator.
<code>i--;</code>
is the equivalent of
<code>i = i - 1;</code>
<strong>Note</strong><br>The entire line becomes <code>i--;</code>, eliminating the need for the equal sign.
</section>

## Instructions
<section id='instructions'>
Change the code to use the <code>--</code> operator on <code>myVar</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var myVar = 11;

// Only change code below this line
myVar = myVar - 1;

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return 'myVar = ' + z;})(myVar);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myVar = 11;
myVar--;
```

</section>
<hr>

# 13. Create Decimal Numbers with JavaScript

## Description
<section id='description'>
We can store decimal numbers in variables too. Decimal numbers are sometimes referred to as <dfn>floating point</dfn> numbers or <dfn>floats</dfn>.
<strong>Note</strong><br>Not all real numbers can accurately be represented in <dfn>floating point</dfn>. This can lead to rounding errors. <a href="https://en.wikipedia.org/wiki/Floating_point#Accuracy_problems" target="_blank">Details Here</a>.
</section>

## Instructions
<section id='instructions'>
Create a variable <code>myDecimal</code> and give it a decimal value with a fractional part (e.g. <code>5.7</code>).
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var ourDecimal = 5.7;

// Only change code below this line


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){if(typeof myDecimal !== "undefined"){return myDecimal;}})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myDecimal = 9.9;
```

</section>
<hr>

# 14. Multiply Two Decimals with JavaScript

## Description
<section id='description'>
In JavaScript, you can also perform calculations with decimal numbers, just like whole numbers.
Let's multiply two decimals together to get their product.
</section>

## Instructions
<section id='instructions'>
Change the <code>0.0</code> so that product will equal <code>5.0</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var product = 2.0 * 0.0;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(y){return 'product = '+y;})(product);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var product = 2.0 * 2.5;
```

</section>
<hr>

# 15. Divide One Decimal by Another with JavaScript

## Description
<section id='description'>
Now let's divide one decimal by another.
</section>

## Instructions
<section id='instructions'>
Change the <code>0.0</code> so that <code>quotient</code> will equal to <code>2.2</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var quotient = 0.0 / 2.0; // Fix this line
```

</div>


### After Test
<div id='js-teardown'>

```js
(function(y){return 'quotient = '+y;})(quotient);
```

</div>

</section>

## Solution
<section id='solution'>

```js
var quotient = 4.4 / 2.0;
```
</section>
<hr>

# 16. Finding a Remainder in JavaScript

## Description
<section id='description'>
The <dfn>remainder</dfn> operator <code>%</code> gives the remainder of the division of two numbers.
<strong>Example</strong>
<blockquote>5 % 2 = 1 because<br>Math.floor(5 / 2) = 2 (Quotient)<br>2 * 2 = 4<br>5 - 4 = 1 (Remainder)</blockquote>
<strong>Usage</strong><br>In mathematics, a number can be checked to be even or odd by checking the remainder of the division of the number by <code>2</code>.
<blockquote>17 % 2 = 1 (17 is Odd)<br>48 % 2 = 0 (48 is Even)</blockquote>
<strong>Note</strong><br>The <dfn>remainder</dfn> operator is sometimes incorrectly referred to as  the "modulus" operator. It is very similar to modulus, but does not work properly with negative numbers.
</section>

## Instructions
<section id='instructions'>
Set <code>remainder</code> equal to the remainder of <code>11</code> divided by <code>3</code> using the <dfn>remainder</dfn> (<code>%</code>) operator.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Only change code below this line

var remainder;

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(y){return 'remainder = '+y;})(remainder);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var remainder =  11 % 3;
```

</section>
<hr>

# 17. Compound Assignment With Augmented Addition

## Description
<section id='description'>
In programming, it is common to use assignments to modify the contents of a variable. Remember that everything to the right of the equals sign is evaluated first, so we can say:
<code>myVar = myVar + 5;</code>
to add <code>5</code> to <code>myVar</code>. Since this is such a common pattern, there are operators which do both a mathematical operation and assignment in one step.
One such operator is the <code>+=</code> operator.
<blockquote>var myVar = 1;<br>myVar += 5;<br>console.log(myVar); // Returns 6</blockquote>
</section>

## Instructions
<section id='instructions'>
Convert the assignments for <code>a</code>, <code>b</code>, and <code>c</code> to use the <code>+=</code> operator.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var a = 3;
var b = 17;
var c = 12;

// Only modify code below this line

a = a + 12;
b = 9 + b;
c = c + 7;

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(a,b,c){ return "a = " + a + ", b = " + b + ", c = " + c; })(a,b,c);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var a = 3;
var b = 17;
var c = 12;

a += 12;
b += 9;
c += 7;
```

</section>
<hr>

# 18. Compound Assignment With Augmented Subtraction

## Description
<section id='description'>
Like the <code>+=</code> operator, <code>-=</code> subtracts a number from a variable.
<code>myVar = myVar - 5;</code>
will subtract <code>5</code> from <code>myVar</code>. This can be rewritten as:
<code>myVar -= 5;</code>
</section>

## Instructions
<section id='instructions'>
Convert the assignments for <code>a</code>, <code>b</code>, and <code>c</code> to use the <code>-=</code> operator.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var a = 11;
var b = 9;
var c = 3;

// Only modify code below this line

a = a - 6;
b = b - 15;
c = c - 1;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(a,b,c){ return "a = " + a + ", b = " + b + ", c = " + c; })(a,b,c);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var a = 11;
var b = 9;
var c = 3;

a -= 6;
b -= 15;
c -= 1;


```

</section>
<hr>

# 19. Compound Assignment With Augmented Multiplication

## Description
<section id='description'>
The <code>*=</code> operator multiplies a variable by a number.
<code>myVar = myVar * 5;</code>
will multiply <code>myVar</code> by <code>5</code>. This can be rewritten as:
<code>myVar *= 5;</code>
</section>

## Instructions
<section id='instructions'>
Convert the assignments for <code>a</code>, <code>b</code>, and <code>c</code> to use the <code>*=</code> operator.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var a = 5;
var b = 12;
var c = 4.6;

// Only modify code below this line

a = a * 5;
b = 3 * b;
c = c * 10;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(a,b,c){ return "a = " + a + ", b = " + b + ", c = " + c; })(a,b,c);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var a = 5;
var b = 12;
var c = 4.6;

a *= 5;
b *= 3;
c *= 10;
```

</section>
<hr>

# 20. Compound Assignment With Augmented Division

## Description
<section id='description'>
The <code>/=</code> operator divides a variable by another number.
<code>myVar = myVar / 5;</code>
Will divide <code>myVar</code> by <code>5</code>. This can be rewritten as:
<code>myVar /= 5;</code>
</section>

## Instructions
<section id='instructions'>
Convert the assignments for <code>a</code>, <code>b</code>, and <code>c</code> to use the <code>/=</code> operator.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var a = 48;
var b = 108;
var c = 33;

// Only modify code below this line

a = a / 12;
b = b / 4;
c = c / 11;

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(a,b,c){ return "a = " + a + ", b = " + b + ", c = " + c; })(a,b,c);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var a = 48;
var b = 108;
var c = 33;

a /= 12;
b /= 4;
c /= 11;
```

</section>
<hr>

# 21. Declare String Variables

## Description
<section id='description'>
Previously we have used the code
<code>var myName = "your name";</code>
<code>"your name"</code> is called a <dfn>string</dfn> <dfn>literal</dfn>. It is a string because it is a series of zero or more characters enclosed in single or double quotes.
</section>

## Instructions
<section id='instructions'>
Create two new <code>string</code> variables: <code>myFirstName</code> and <code>myLastName</code> and assign them the values of your first and last name, respectively.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var firstName = "Alan";
var lastName = "Turing";

// Only change code below this line


```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof myFirstName !== "undefined" && typeof myLastName !== "undefined"){(function(){return myFirstName + ', ' + myLastName;})();}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myFirstName = "Alan";
var myLastName = "Turing";
```

</section>
<hr>

# 22. Escaping Literal Quotes in Strings

## Description
<section id='description'>
When you are defining a string you must start and end with a single or double quote. What happens when you need a literal quote: <code>"</code> or <code>'</code> inside of your string?
In JavaScript, you can <dfn>escape</dfn> a quote from considering it as an end of string quote by placing a <dfn>backslash</dfn> (<code>\</code>) in front of the quote.
<code>var sampleStr = "Alan said, \"Peter is learning JavaScript\".";</code>
This signals to JavaScript that the following quote is not the end of the string, but should instead appear inside the string. So if you were to print this to the console, you would get:
<code>Alan said, "Peter is learning JavaScript".</code>
</section>

## Instructions
<section id='instructions'>
Use <dfn>backslashes</dfn> to assign a string to the <code>myStr</code> variable so that if you were to print it to the console, you would see:
<code>I am a "double quoted" string inside "double quotes".</code>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var myStr = ""; // Change this line


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){
  if(typeof myStr === 'string') {
    console.log("myStr = \"" + myStr + "\"");
  } else {
    console.log("myStr is undefined");
  }
})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myStr = "I am a \"double quoted\" string inside \"double quotes\".";
```

</section>
<hr>

# 23. Quoting Strings with Single Quotes

## Description
<section id='description'>
<dfn>String</dfn> values in JavaScript may be written with single or double quotes, as long as you start and end with the same type of quote. Unlike some other programming languages, single and double quotes work the same in JavaScript.
<blockquote>doubleQuoteStr = "This is a string"; <br/>singleQuoteStr = 'This is also a string';</blockquote>
The reason why you might want to use one type of quote over the other is if you want to use both in a string. This might happen if you want to save a conversation in a string and have the conversation in quotes. Another use for it would be saving an <code>&#60;a&#62;</code> tag with various attributes in quotes, all within a string.
<blockquote>conversation = 'Finn exclaims to Jake, "Algebraic!"';</blockquote>
However, this becomes a problem if you need to use the outermost quotes within it. Remember, a string has the same kind of quote at the beginning and end. But if you have that same quote somewhere in the middle, the string will stop early and throw an error.
<blockquote>goodStr = 'Jake asks Finn, "Hey, let\'s go on an adventure?"'; <br/>badStr = 'Finn responds, "Let's go!"'; // Throws an error</blockquote>
In the <dfn>goodStr</dfn> above, you can use both quotes safely by using the backslash <code>\</code> as an escape character.
<strong>Note</strong><br/>The backslash <code>\</code> should not be confused with the forward slash <code>/</code>. They do not do the same thing.
</section>

## Instructions
<section id='instructions'>
Change the provided string to a string with single quotes at the beginning and end and no escape characters.
Right now, the <code>&#60;a&#62;</code> tag in the string uses double quotes everywhere. You will need to change the outer quotes to single quotes so you can remove the escape characters.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var myStr = "<a href=\"http://www.example.com\" target=\"_blank\">Link</a>";


```

</div>


### After Test
<div id='js-teardown'>

```js
(function() { return "myStr = " + myStr; })();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myStr = '<a href="http://www.example.com" target="_blank">Link</a>';
```

</section>
<hr>

# 24. Escape Sequences in Strings

## Description
<section id='description'>
Quotes are not the only characters that can be <dfn>escaped</dfn> inside a string. There are two reasons to use escaping characters:<ol><li>To allow you to use characters you may not otherwise be able to type out, such as a carriage returns.</li><li>To allow you to represent multiple quotes in a string without JavaScript misinterpreting what you mean.</li></ol>We learned this in the previous challenge.
<table class="table table-striped"><thead><tr><th>Code</th><th>Output</th></tr></thead><tbody><tr><td><code>\'</code></td><td>single quote</td></tr><tr><td><code>\"</code></td><td>double quote</td></tr><tr><td><code>\\</code></td><td>backslash</td></tr><tr><td><code>\n</code></td><td>newline</td></tr><tr><td><code>\r</code></td><td>carriage return</td></tr><tr><td><code>\t</code></td><td>tab</td></tr><tr><td><code>\b</code></td><td>word boundary</td></tr><tr><td><code>\f</code></td><td>form feed</td></tr></tbody></table>
<em>Note that the backslash itself must be escaped in order to display as a backslash.</em>
</section>

## Instructions
<section id='instructions'>
Assign the following three lines of text into the single variable <code>myStr</code> using escape sequences.
<blockquote>FirstLine<br/>&nbsp;&nbsp;&nbsp;&nbsp;\SecondLine<br/>ThirdLine</blockquote>
You will need to use escape sequences to insert special characters correctly. You will also need to follow the spacing as it looks above, with no spaces between escape sequences or words.
Here is the text with the escape sequences written out.
<q>FirstLine<code>newline</code><code>tab</code><code>backslash</code>SecondLine<code>newline</code>ThirdLine</q>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var myStr; // Change this line


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){
if (myStr !== undefined){
console.log('myStr:\n' + myStr);}})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myStr = "FirstLine\n\t\\SecondLine\nThirdLine";
```

</section>
<hr>

# 25. Concatenating Strings with Plus Operator

## Description
<section id='description'>
In JavaScript, when the <code>+</code> operator is used with a <code>String</code> value, it is called the <dfn>concatenation</dfn> operator. You can build a new string out of other strings by <dfn>concatenating</dfn> them together.
<strong>Example</strong>
<blockquote>'My name is Alan,' + ' I concatenate.'</blockquote>
<strong>Note</strong><br>Watch out for spaces. Concatenation does not add spaces between concatenated strings, so you'll need to add them yourself.
</section>

## Instructions
<section id='instructions'>
Build <code>myStr</code> from the strings <code>"This is the start. "</code> and <code>"This is the end."</code> using the <code>+</code> operator.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourStr = "I come first. " + "I come second.";

// Only change code below this line

var myStr;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){
  if(typeof myStr === 'string') {
    return 'myStr = "' + myStr + '"';
  } else {
    return 'myStr is not a string';
  }
})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var ourStr = "I come first. " + "I come second.";
var myStr = "This is the start. " + "This is the end.";
```

</section>
<hr>

# 26. Concatenating Strings with the Plus Equals Operator

## Description
<section id='description'>
We can also use the <code>+=</code> operator to <dfn>concatenate</dfn> a string onto the end of an existing string variable. This can be very helpful to break a long string over several lines.
<strong>Note</strong><br>Watch out for spaces. Concatenation does not add spaces between concatenated strings, so you'll need to add them yourself.
</section>

## Instructions
<section id='instructions'>
Build <code>myStr</code> over several lines by concatenating these two strings: <code>"This is the first sentence. "</code> and <code>"This is the second sentence."</code> using the <code>+=</code> operator. Use the <code>+=</code> operator similar to how it is shown in the editor. Start by assigning the first string to <code>myStr</code>, then add on the second string.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourStr = "I come first. ";
ourStr += "I come second.";

// Only change code below this line

var myStr;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){
  if(typeof myStr === 'string') {
    return 'myStr = "' + myStr + '"';
  } else {
    return 'myStr is not a string';
  }
})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var ourStr = "I come first. ";
ourStr += "I come second.";

var myStr = "This is the first sentence. ";
myStr += "This is the second sentence.";
```

</section>
<hr>

# 27. Constructing Strings with Variables

## Description
<section id='description'>
Sometimes you will need to build a string, <a href="https://en.wikipedia.org/wiki/Mad_Libs" target="_blank">Mad Libs</a> style. By using the concatenation operator (<code>+</code>), you can insert one or more variables into a string you're building.
</section>

## Instructions
<section id='instructions'>
Set <code>myName</code> to a string equal to your name and build <code>myStr</code> with <code>myName</code> between the strings <code>"My name is "</code> and <code>" and I am well!"</code>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourName = "freeCodeCamp";
var ourStr = "Hello, our name is " + ourName + ", how are you?";

// Only change code below this line
var myName;
var myStr;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){
  var output = [];
  if(typeof myName === 'string') {
    output.push('myName = "' + myName + '"');
  } else {
    output.push('myName is not a string');
  }
  if(typeof myStr === 'string') {
    output.push('myStr = "' + myStr + '"');
  } else {
    output.push('myStr is not a string');
  }
  return output.join('\n');
})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myName = "Bob";
var myStr = "My name is " + myName + " and I am well!";
```

</section>
<hr>

# 28. Appending Variables to Strings

## Description
<section id='description'>
Just as we can build a string over multiple lines out of string <dfn>literals</dfn>, we can also append variables to a string using the plus equals (<code>+=</code>) operator.
</section>

## Instructions
<section id='instructions'>
Set <code>someAdjective</code> and append it to <code>myStr</code> using the <code>+=</code> operator.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var anAdjective = "awesome!";
var ourStr = "freeCodeCamp is ";
ourStr += anAdjective;

// Only change code below this line

var someAdjective;
var myStr = "Learning to code is ";

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){
  var output = [];
  if(typeof someAdjective === 'string') {
    output.push('someAdjective = "' + someAdjective + '"');
  } else {
    output.push('someAdjective is not a string');
  }
  if(typeof myStr === 'string') {
    output.push('myStr = "' + myStr + '"');
  } else {
    output.push('myStr is not a string');
  }
  return output.join('\n');
})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var anAdjective = "awesome!";
var ourStr = "freeCodeCamp is ";
ourStr += anAdjective;

var someAdjective = "neat";
var myStr = "Learning to code is ";
myStr += someAdjective;
```

</section>
<hr>

# 29. Find the Length of a String

## Description
<section id='description'>
You can find the length of a <code>String</code> value by writing <code>.length</code> after the string variable or string literal.
<code>"Alan Peter".length; // 10</code>
For example, if we created a variable <code>var firstName = "Charles"</code>, we could find out how long the string <code>"Charles"</code> is by using the <code>firstName.length</code> property.
</section>

## Instructions
<section id='instructions'>
Use the <code>.length</code> property to count the number of characters in the <code>lastName</code> variable and assign it to <code>lastNameLength</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var firstNameLength = 0;
var firstName = "Ada";

firstNameLength = firstName.length;

// Setup
var lastNameLength = 0;
var lastName = "Lovelace";

// Only change code below this line.

lastNameLength = lastName;


```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof lastNameLength !== "undefined"){(function(){return lastNameLength;})();}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var firstNameLength = 0;
var firstName = "Ada";
firstNameLength = firstName.length;

var lastNameLength = 0;
var lastName = "Lovelace";
lastNameLength = lastName.length;
```

</section>
<hr>

# 30. Use Bracket Notation to Find the First Character in a String

## Description
<section id='description'>
<code>Bracket notation</code> is a way to get a character at a specific <code>index</code> within a string.
Most modern programming languages, like JavaScript, don't start counting at 1 like humans do. They start at 0. This is referred to as <dfn>Zero-based</dfn> indexing.
For example, the character at index 0 in the word "Charles" is "C". So if <code>var firstName = "Charles"</code>, you can get the value of the first letter of the string by using <code>firstName[0]</code>.
</section>

## Instructions
<section id='instructions'>
Use <dfn>bracket notation</dfn> to find the first character in the <code>lastName</code> variable and assign it to <code>firstLetterOfLastName</code>.
<strong>Hint</strong><br>Try looking at the <code>firstLetterOfFirstName</code> variable declaration if you get stuck.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var firstLetterOfFirstName = "";
var firstName = "Ada";

firstLetterOfFirstName = firstName[0];

// Setup
var firstLetterOfLastName = "";
var lastName = "Lovelace";

// Only change code below this line
firstLetterOfLastName = lastName;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(v){return v;})(firstLetterOfLastName);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var firstLetterOfLastName = "";
var lastName = "Lovelace";

// Only change code below this line
firstLetterOfLastName = lastName[0];
```

</section>
<hr>

# 31. Understand String Immutability

## Description
<section id='description'>
In JavaScript, <code>String</code> values are <dfn>immutable</dfn>, which means that they cannot be altered once created.
For example, the following code:
<blockquote>var myStr = "Bob";<br>myStr[0] = "J";</blockquote>
cannot change the value of <code>myStr</code> to "Job", because the contents of <code>myStr</code> cannot be altered. Note that this does <em>not</em> mean that <code>myStr</code> cannot be changed, just that the individual characters of a <dfn>string literal</dfn> cannot be changed. The only way to change <code>myStr</code> would be to assign it with a new string, like this:
<blockquote>var myStr = "Bob";<br>myStr = "Job";</blockquote>
</section>

## Instructions
<section id='instructions'>
Correct the assignment to <code>myStr</code> so it contains the string value of <code>Hello World</code> using the approach shown in the example above.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var myStr = "Jello World";

// Only change code below this line

myStr[0] = "H"; // Fix Me


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(v){return "myStr = " + v;})(myStr);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myStr = "Jello World";
myStr = "Hello World";
```

</section>
<hr>

# 32. Use Bracket Notation to Find the Nth Character in a String

## Description
<section id='description'>
You can also use <dfn>bracket notation</dfn> to get the character at other positions within a string.
Remember that computers start counting at <code>0</code>, so the first character is actually the zeroth character.
</section>

## Instructions
<section id='instructions'>
Let's try to set <code>thirdLetterOfLastName</code> to equal the third letter of the <code>lastName</code> variable using bracket notation.
<strong>Hint</strong><br>Try looking at the <code>secondLetterOfFirstName</code> variable declaration if you get stuck.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var firstName = "Ada";
var secondLetterOfFirstName = firstName[1];

// Setup
var lastName = "Lovelace";

// Only change code below this line.
var thirdLetterOfLastName = lastName;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(v){return v;})(thirdLetterOfLastName);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var lastName = "Lovelace";
var thirdLetterOfLastName = lastName[2];
```

</section>
<hr>

# 33. Use Bracket Notation to Find the Last Character in a String

## Description
<section id='description'>
In order to get the last letter of a string, you can subtract one from the string's length.
For example, if <code>var firstName = "Charles"</code>, you can get the value of the last letter of the string by using <code>firstName[firstName.length - 1]</code>.
</section>

## Instructions
<section id='instructions'>
Use <dfn>bracket notation</dfn> to find the last character in the <code>lastName</code> variable.
<strong>Hint</strong><br>Try looking at the <code>lastLetterOfFirstName</code> variable declaration if you get stuck.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var firstName = "Ada";
var lastLetterOfFirstName = firstName[firstName.length - 1];

// Setup
var lastName = "Lovelace";

// Only change code below this line.
var lastLetterOfLastName = lastName;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(v){return v;})(lastLetterOfLastName);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var firstName = "Ada";
var lastLetterOfFirstName = firstName[firstName.length - 1];

var lastName = "Lovelace";
var lastLetterOfLastName = lastName[lastName.length - 1];
```

</section>
<hr>

# 34. Use Bracket Notation to Find the Nth-to-Last Character in a String

## Description
<section id='description'>
You can use the same principle we just used to retrieve the last character in a string to retrieve the Nth-to-last character.
For example, you can get the value of the third-to-last letter of the <code>var firstName = "Charles"</code> string by using <code>firstName[firstName.length - 3]</code>
</section>

## Instructions
<section id='instructions'>
Use <dfn>bracket notation</dfn> to find the second-to-last character in the <code>lastName</code> string.
<strong>Hint</strong><br>Try looking at the <code>thirdToLastLetterOfFirstName</code> variable declaration if you get stuck.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var firstName = "Ada";
var thirdToLastLetterOfFirstName = firstName[firstName.length - 3];

// Setup
var lastName = "Lovelace";

// Only change code below this line
var secondToLastLetterOfLastName = lastName;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(v){return v;})(secondToLastLetterOfLastName);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var firstName = "Ada";
var thirdToLastLetterOfFirstName = firstName[firstName.length - 3];

var lastName = "Lovelace";
var secondToLastLetterOfLastName = lastName[lastName.length - 2];
```

</section>
<hr>

# 35. Word Blanks

## Description
<section id='description'>
We will now use our knowledge of strings to build a "<a href='https://en.wikipedia.org/wiki/Mad_Libs' target='_blank'>Mad Libs</a>" style word game we're calling "Word Blanks". You will create an (optionally humorous) "Fill in the Blanks" style sentence.
In a "Mad Libs" game, you are provided sentences with some missing words, like nouns, verbs, adjectives and adverbs. You then fill in the missing pieces with words of your choice in a way that the completed sentence makes sense.
Consider this sentence - "It was really <strong>____</strong>, and we <strong>____</strong> ourselves <strong>____</strong>". This sentence has three missing pieces- an adjective, a verb and an adverb, and we can add words of our choice to complete it. We can then assign the completed sentence to a variable as follows:
<blockquote>var sentence = "It was really" + "hot" + ", and we" + "laughed" + "ourselves" + "silly.";</blockquote>
</section>

## Instructions
<section id='instructions'>
In this challenge, we provide you with a noun, a verb, an adjective and an adverb. You need to form a complete sentence using words of your choice, along with the words we provide.
You will need to use the string concatenation operator <code>+</code> to build a new string, using the provided variables: <code>myNoun</code>, <code>myAdjective</code>, <code>myVerb</code>, and <code>myAdverb</code>. You will then assign the formed string to the <code>result</code> variable.
You will also need to account for spaces in your string, so that the final sentence has spaces between all the words. The result should be a complete sentence.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function wordBlanks(myNoun, myAdjective, myVerb, myAdverb) {
  // Your code below this line
  var result = "";

  // Your code above this line
  return result;
}

// Change the words here to test your function
wordBlanks("dog", "big", "ran", "quickly");
```

</div>


### After Test
<div id='js-teardown'>

```js
var test1 = wordBlanks("dog", "big", "ran", "quickly");
var test2 = wordBlanks("cat", "little", "hit", "slowly");
```

</div>

</section>

## Solution
<section id='solution'>


```js
function wordBlanks(myNoun, myAdjective, myVerb, myAdverb) {
  var result = "";

  result = "Once there was a " + myNoun + " which was very " + myAdjective + ". ";
  result += "It " + myVerb + " " + myAdverb + " around the yard.";

  return result;
}
```

</section>
<hr>

# 36. Store Multiple Values in one Variable using JavaScript Arrays

## Description
<section id='description'>
With JavaScript <code>array</code> variables, we can store several pieces of data in one place.
You start an array declaration with an opening square bracket, end it with a closing square bracket, and put a comma between each entry, like this:
<code>var sandwich = ["peanut butter", "jelly", "bread"]</code>.
</section>

## Instructions
<section id='instructions'>
Modify the new array <code>myArray</code> so that it contains both a <code>string</code> and a <code>number</code> (in that order).
<strong>Hint</strong><br>Refer to the example code in the text editor if you get stuck.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = ["John", 23];

// Only change code below this line.
var myArray = [];

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return z;})(myArray);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = ["The Answer", 42];
```

</section>
<hr>

# 37. Nest one Array within Another Array

## Description
<section id='description'>
You can also nest arrays within other arrays, like this: <code>[["Bulls", 23], ["White Sox", 45]]</code>. This is also called a <dfn>Multi-dimensional Array<dfn>.
</section>

## Instructions
<section id='instructions'>
Create a nested array called <code>myArray</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = [["the universe", 42], ["everything", 101010]];

// Only change code below this line.
var myArray = [];

```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof myArray !== "undefined"){(function(){return myArray;})();}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = [[1,2,3]];
```

</section>
<hr>

# 38. Access Array Data with Indexes

## Description
<section id='description'>
We can access the data inside arrays using <code>indexes</code>.
Array indexes are written in the same bracket notation that strings use, except that instead of specifying a character, they are specifying an entry in the array. Like strings, arrays use <dfn>zero-based</dfn> indexing, so the first element in an array is element <code>0</code>.
<br />
<strong>Example</strong>
<blockquote>var array = [50,60,70];<br>array[0]; // equals 50<br>var data = array[1];  // equals 60</blockquote>
<strong>Note</strong><br>There shouldn't be any spaces between the array name and the square brackets, like <code>array [0]</code>. Although JavaScript is able to process this correctly, this may confuse other programmers reading your code.
</section>

## Instructions
<section id='instructions'>
Create a variable called <code>myData</code> and set it to equal the first value of <code>myArray</code> using bracket notation.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = [50,60,70];
var ourData = ourArray[0]; // equals 50

// Setup
var myArray = [50,60,70];

// Only change code below this line.

```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof myArray !== "undefined" && typeof myData !== "undefined"){(function(y,z){return 'myArray = ' + JSON.stringify(y) + ', myData = ' + JSON.stringify(z);})(myArray, myData);}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = [50,60,70];
var myData = myArray[0];
```

</section>
<hr>

# 39. Modify Array Data With Indexes

## Description
<section id='description'>
Unlike strings, the entries of arrays are <dfn>mutable</dfn> and can be changed freely.
<strong>Example</strong>
<blockquote>var ourArray = [50,40,30];<br>ourArray[0] = 15; // equals [15,40,30]</blockquote>
<strong>Note</strong><br>There shouldn't be any spaces between the array name and the square brackets, like <code>array [0]</code>. Although JavaScript is able to process this correctly, this may confuse other programmers reading your code.
</section>

## Instructions
<section id='instructions'>
Modify the data stored at index <code>0</code> of <code>myArray</code> to a value of <code>45</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = [18,64,99];
ourArray[1] = 45; // ourArray now equals [18,45,99].

// Setup
var myArray = [18,64,99];

// Only change code below this line.


```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof myArray !== "undefined"){(function(){return myArray;})();}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = [18,64,99];
myArray[0] = 45;
```

</section>
<hr>

# 40. Access Multi-Dimensional Arrays With Indexes

## Description
<section id='description'>
One way to think of a <dfn>multi-dimensional</dfn> array, is as an <em>array of arrays</em>. When you use brackets to access your array, the first set of brackets refers to the entries in the outer-most (the first level) array, and each additional pair of brackets refers to the next level of entries inside.
<strong>Example</strong>
<blockquote>var arr = [<br>&nbsp;&nbsp;[1,2,3],<br>&nbsp;&nbsp;[4,5,6],<br>&nbsp;&nbsp;[7,8,9],<br>&nbsp;&nbsp;[[10,11,12], 13, 14]<br>];<br>arr[3]; // equals [[10,11,12], 13, 14]<br>arr[3][0]; // equals [10,11,12]<br>arr[3][0][1]; // equals 11</blockquote>
<strong>Note</strong><br>There shouldn't be any spaces between the array name and the square brackets, like <code>array [0][0]</code> and even this <code>array [0] [0]</code> is not allowed. Although JavaScript is able to process this correctly, this may confuse other programmers reading your code.
</section>

## Instructions
<section id='instructions'>
Using bracket notation select an element from <code>myArray</code> such that <code>myData</code> is equal to <code>8</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var myArray = [[1,2,3], [4,5,6], [7,8,9], [[10,11,12], 13, 14]];

// Only change code below this line.
var myData = myArray[0][0];

```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof myArray !== "undefined"){(function(){return "myData: " + myData + " myArray: " + JSON.stringify(myArray);})();}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = [[1,2,3],[4,5,6], [7,8,9], [[10,11,12], 13, 14]];
var myData = myArray[2][1];
```

</section>
<hr>

# 41. Manipulate Arrays With push()

## Description
<section id='description'>
An easy way to append data to the end of an array is via the <code>push()</code> function.
<code>.push()</code> takes one or more <dfn>parameters</dfn> and "pushes" them onto the end of the array.
<blockquote>var arr = [1,2,3];<br>arr.push(4);<br>// arr is now [1,2,3,4]</blockquote>
</section>

## Instructions
<section id='instructions'>
Push <code>["dog", 3]</code> onto the end of the <code>myArray</code> variable.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = ["Stimpson", "J", "cat"];
ourArray.push(["happy", "joy"]);
// ourArray now equals ["Stimpson", "J", "cat", ["happy", "joy"]]

// Setup
var myArray = [["John", 23], ["cat", 2]];

// Only change code below this line.


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return 'myArray = ' + JSON.stringify(z);})(myArray);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = [["John", 23], ["cat", 2]];
myArray.push(["dog",3]);
```

</section>
<hr>

# 42. Manipulate Arrays With pop()

## Description
<section id='description'>
Another way to change the data in an array is with the <code>.pop()</code> function.
<code>.pop()</code> is used to "pop" a value off of the end of an array. We can store this "popped off" value by assigning it to a variable. In other words, <code>.pop()</code> removes the last element from an array and returns that element.
Any type of entry can be "popped" off of an array - numbers, strings, even nested arrays.
<blockquote><code>var threeArr = [1, 4, 6];<br> var oneDown = threeArr.pop();<br> console.log(oneDown); // Returns 6<br> console.log(threeArr); // Returns [1, 4]</code></blockquote>
</section>

## Instructions
<section id='instructions'>
Use the <code>.pop()</code> function to remove the last item from <code>myArray</code>, assigning the "popped off" value to <code>removedFromMyArray</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = [1,2,3];
var removedFromOurArray = ourArray.pop();
// removedFromOurArray now equals 3, and ourArray now equals [1,2]

// Setup
var myArray = [["John", 23], ["cat", 2]];

// Only change code below this line.
var removedFromMyArray;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(y, z){return 'myArray = ' + JSON.stringify(y) + ' & removedFromMyArray = ' + JSON.stringify(z);})(myArray, removedFromMyArray);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = [["John", 23], ["cat", 2]];
var removedFromMyArray = myArray.pop();
```

</section>
<hr>

# 43. Manipulate Arrays With shift()

## Description
<section id='description'>
<code>pop()</code> always removes the last element of an array. What if you want to remove the first?
That's where <code>.shift()</code> comes in. It works just like <code>.pop()</code>, except it removes the first element instead of the last.
</section>

## Instructions
<section id='instructions'>
Use the <code>.shift()</code> function to remove the first item from <code>myArray</code>, assigning the "shifted off" value to <code>removedFromMyArray</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = ["Stimpson", "J", ["cat"]];
var removedFromOurArray = ourArray.shift();
// removedFromOurArray now equals "Stimpson" and ourArray now equals ["J", ["cat"]].

// Setup
var myArray = [["John", 23], ["dog", 3]];

// Only change code below this line.
var removedFromMyArray;


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(y, z){return 'myArray = ' + JSON.stringify(y) + ' & removedFromMyArray = ' + JSON.stringify(z);})(myArray, removedFromMyArray);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = [["John", 23], ["dog", 3]];

// Only change code below this line.
var removedFromMyArray = myArray.shift();
```

</section>
<hr>

# 44. Manipulate Arrays With unshift()

## Description
<section id='description'>
Not only can you <code>shift</code> elements off of the beginning of an array, you can also <code>unshift</code> elements to the beginning of an array i.e. add elements in front of the array.
<code>.unshift()</code> works exactly like <code>.push()</code>, but instead of adding the element at the end of the array, <code>unshift()</code> adds the element at the beginning of the array.
</section>

## Instructions
<section id='instructions'>
Add <code>["Paul",35]</code> to the beginning of the <code>myArray</code> variable using <code>unshift()</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = ["Stimpson", "J", "cat"];
ourArray.shift(); // ourArray now equals ["J", "cat"]
ourArray.unshift("Happy");
// ourArray now equals ["Happy", "J", "cat"]

// Setup
var myArray = [["John", 23], ["dog", 3]];
myArray.shift();

// Only change code below this line.


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(y, z){return 'myArray = ' + JSON.stringify(y);})(myArray);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = [["John", 23], ["dog", 3]];
myArray.shift();
myArray.unshift(["Paul", 35]);
```

</section>
<hr>

# 45. Shopping List

## Description
<section id='description'>
Create a shopping list in the variable <code>myList</code>. The list should be a multi-dimensional array containing several sub-arrays.
The first element in each sub-array should contain a string with the name of the item. The second element should be a number representing the quantity i.e.
<code>["Chocolate Bar", 15]</code>
There should be at least 5 sub-arrays in the list.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var myList = [];


```

</div>


### After Test
<div id='js-teardown'>

```js
var count = 0;
var isArray = false;
var hasString = false;
var hasNumber = false;
(function(list){
  if(Array.isArray(myList)) {
    isArray = true;
    if(myList.length > 0) {
      hasString = true;
      hasNumber = true;
      for (var elem of myList) {
        if(!elem || !elem[0] || typeof elem[0] !== 'string') {
          hasString = false;
        }
        if(!elem || typeof elem[1] !== 'number') {
          hasNumber = false;
        }
      }
    }
    count = myList.length;
    return JSON.stringify(myList);
  } else {
    return "myList is not an array";
  }

})(myList);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myList = [
  ["Candy", 10],
  ["Potatoes", 12],
  ["Eggs", 12],
  ["Catfood", 1],
  ["Toads", 9]
];
```

</section>
<hr>

# 46. Write Reusable JavaScript with Functions

## Description
<section id='description'>
In JavaScript, we can divide up our code into reusable parts called <dfn>functions</dfn>.
Here's an example of a function:
<blockquote>function functionName() {<br>&nbsp;&nbsp;console.log("Hello World");<br>}</blockquote>
You can call or <dfn>invoke</dfn> this function by using its name followed by parentheses, like this:
<code>functionName();</code>
Each time the function is called it will print out the message <code>"Hello World"</code> on the dev console. All of the code between the curly braces will be executed every time the function is called.
</section>

## Instructions
<section id='instructions'>
<ol><li>Create a function called <code>reusableFunction</code> which prints <code>"Hi World"</code> to the dev console.</li><li>Call the function.</li></ol>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
function ourReusableFunction() {
  console.log("Heyya, World");
}

ourReusableFunction();

// Only change code below this line

```

</div>

### Before Test
<div id='js-setup'>

```js
var logOutput = "";
var originalConsole = console
function capture() {
    var nativeLog = console.log;
    console.log = function (message) {
        if(message && message.trim) logOutput = message.trim();
        if(nativeLog.apply) {
          nativeLog.apply(originalConsole, arguments);
        } else {
          var nativeMsg = Array.prototype.slice.apply(arguments).join(' ');
          nativeLog(nativeMsg);
        }
    };
}

function uncapture() {
  console.log = originalConsole.log;
}

capture();
```

</div>

### After Test
<div id='js-teardown'>

```js
uncapture();

if (typeof reusableFunction !== "function") { 
  (function() { return "reusableFunction is not defined"; })();
} else {
  (function() { return logOutput || "console.log never called"; })();
}
```

</div>

</section>

## Solution
<section id='solution'>


```js
function reusableFunction() {
  console.log("Hi World");
}
reusableFunction();
```

</section>
<hr>

# 47. Passing Values to Functions with Arguments

## Description
<section id='description'>
<dfn>Parameters</dfn> are variables that act as placeholders for the values that are to be input to a function when it is called. When a function is defined, it is typically defined along with one or more parameters. The actual values that are input (or <dfn>"passed"</dfn>) into a function when it is called are known as <dfn>arguments</dfn>.
Here is a function with two parameters, <code>param1</code> and <code>param2</code>:
<blockquote>function testFun(param1, param2) {<br>&nbsp;&nbsp;console.log(param1, param2);<br>}</blockquote>
Then we can call <code>testFun</code>:
<code>testFun("Hello", "World");</code>
We have passed two arguments, <code>"Hello"</code> and <code>"World"</code>. Inside the function, <code>param1</code> will equal "Hello" and <code>param2</code> will equal "World". Note that you could call <code>testFun</code> again with different arguments and the parameters would take on the value of the new arguments.
</section>

## Instructions
<section id='instructions'>
<ol><li>Create a function called <code>functionWithArgs</code> that accepts two arguments and outputs their sum to the dev console.</li><li>Call the function with two numbers as arguments.</li></ol>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
function ourFunctionWithArgs(a, b) {
  console.log(a - b);
}
ourFunctionWithArgs(10, 5); // Outputs 5

// Only change code below this line.


```

</div>

### Before Test
<div id='js-setup'>

```js
var logOutput = "";
var originalConsole = console
function capture() {
    var nativeLog = console.log;
    console.log = function (message) {
        if(message) logOutput = JSON.stringify(message).trim();
        if(nativeLog.apply) {
          nativeLog.apply(originalConsole, arguments);
        } else {
          var nativeMsg = Array.prototype.slice.apply(arguments).join(' ');
          nativeLog(nativeMsg);
        }
    };
}

function uncapture() {
  console.log = originalConsole.log;
}

capture();
```

</div>

### After Test
<div id='js-teardown'>

```js
uncapture();

if (typeof functionWithArgs !== "function") { 
  (function() { return "functionWithArgs is not defined"; })();
} else {
  (function() { return logOutput || "console.log never called"; })();
}
```

</div>

</section>

## Solution
<section id='solution'>


```js
function functionWithArgs(a, b) {
  console.log(a + b);
}
functionWithArgs(10, 5);
```

</section>
<hr>

# 48. Global Scope and Functions

## Description
<section id='description'>
In JavaScript, <dfn>scope</dfn> refers to the visibility of variables. Variables which are defined outside of a function block have <dfn>Global</dfn> scope. This means, they can be seen everywhere in your JavaScript code.
Variables which are used without the <code>var</code> keyword are automatically created in the <code>global</code> scope. This can create unintended consequences elsewhere in your code or when running a function again. You should always declare your variables with <code>var</code>.
</section>

## Instructions
<section id='instructions'>
Using <code>var</code>, declare a <code>global</code> variable <code>myGlobal</code> outside of any function. Initialize it with a value of <code>10</code>.
Inside function <code>fun1</code>, assign <code>5</code> to <code>oopsGlobal</code> <strong><em>without</em></strong> using the <code>var</code> keyword.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Declare your variable here


function fun1() {
  // Assign 5 to oopsGlobal Here

}

// Only change code above this line
function fun2() {
  var output = "";
  if (typeof myGlobal != "undefined") {
    output += "myGlobal: " + myGlobal;
  }
  if (typeof oopsGlobal != "undefined") {
    output += " oopsGlobal: " + oopsGlobal;
  }
  console.log(output);
}
```

</div>

### Before Test
<div id='js-setup'>

```js
var logOutput = "";
var originalConsole = console
function capture() {
    var nativeLog = console.log;
    console.log = function (message) {
        logOutput = message;
        if(nativeLog.apply) {
          nativeLog.apply(originalConsole, arguments);
        } else {
          var nativeMsg = Array.prototype.slice.apply(arguments).join(' ');
          nativeLog(nativeMsg);
        }
    };
}

function uncapture() {
  console.log = originalConsole.log;
}
var oopsGlobal;
capture();
```

</div>

### After Test
<div id='js-teardown'>

```js
fun1();
fun2();
uncapture();
(function() { return logOutput || "console.log never called"; })();
```

</div>

</section>

## Solution
<section id='solution'>


```js
// Declare your variable here
var myGlobal = 10;

function fun1() {
  // Assign 5 to oopsGlobal Here
  oopsGlobal = 5;
}

// Only change code above this line
function fun2() {
  var output = "";
  if(typeof myGlobal != "undefined") {
    output += "myGlobal: " + myGlobal;
  }
  if(typeof oopsGlobal != "undefined") {
    output += " oopsGlobal: " + oopsGlobal;
  }
  console.log(output);
}
```

</section>
<hr>

# 49. Local Scope and Functions

## Description
<section id='description'>
Variables which are declared within a function, as well as the function parameters have <dfn>local</dfn> scope. That means, they are only visible within that function.
Here is a function <code>myTest</code> with a local variable called <code>loc</code>.
<blockquote>function myTest() {<br>&nbsp;&nbsp;var loc = "foo";<br>&nbsp;&nbsp;console.log(loc);<br>}<br>myTest(); // logs "foo"<br>console.log(loc); // loc is not defined</blockquote>
<code>loc</code> is not defined outside of the function.
</section>

## Instructions
<section id='instructions'>
Declare a local variable <code>myVar</code> inside <code>myLocalScope</code>. Run the tests and then follow the instructions commented out in the editor.
<strong>Hint</strong><br>Refreshing the page may help if you get stuck.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function myLocalScope() {
  'use strict'; // you shouldn't need to edit this line

  console.log(myVar);
}
myLocalScope();

// Run and check the console
// myVar is not defined outside of myLocalScope
console.log(myVar);

// Now remove the console log line to pass the test

```

</div>

### Before Test
<div id='js-setup'>

```js
var logOutput = "";
var originalConsole = console
function capture() {
  var nativeLog = console.log;
  console.log = function (message) {
    logOutput = message;
    if(nativeLog.apply) {
      nativeLog.apply(originalConsole, arguments);
    } else {
      var nativeMsg = Array.prototype.slice.apply(arguments).join(' ');
      nativeLog(nativeMsg);
    }
  };
}

function uncapture() {
  console.log = originalConsole.log;
}

```

</div>

### After Test
<div id='js-teardown'>

```js
typeof myLocalScope === 'function' && (capture(), myLocalScope(), uncapture());
(function() { return logOutput || "console.log never called"; })();
```

</div>

</section>

## Solution
<section id='solution'>


```js
function myLocalScope() {
  'use strict';

  var myVar;
  console.log(myVar);
}
myLocalScope();
```

</section>
<hr>

# 50. Global vs. Local Scope in Functions

## Description
<section id='description'>
It is possible to have both <dfn>local</dfn> and <dfn>global</dfn> variables with the same name. When you do this, the <code>local</code> variable takes precedence over the <code>global</code> variable.
In this example:
<blockquote>var someVar = "Hat";<br>function myFun() {<br>&nbsp;&nbsp;var someVar = "Head";<br>&nbsp;&nbsp;return someVar;<br>}</blockquote>
The function <code>myFun</code> will return <code>"Head"</code> because the <code>local</code> version of the variable is present.
</section>

## Instructions
<section id='instructions'>
Add a local variable to <code>myOutfit</code> function to override the value of <code>outerWear</code> with <code>"sweater"</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var outerWear = "T-Shirt";

function myOutfit() {
  // Only change code below this line



  // Only change code above this line
  return outerWear;
}

myOutfit();
```

</div>



</section>

## Solution
<section id='solution'>


```js
var outerWear = "T-Shirt";
function myOutfit() {
  var outerWear = "sweater";
  return outerWear;
}
```

</section>
<hr>

# 51. Return a Value from a Function with Return

## Description
<section id='description'>
We can pass values into a function with <dfn>arguments</dfn>. You can use a <code>return</code> statement to send a value back out of a function.
<strong>Example</strong>
<blockquote>function plusThree(num) {<br>&nbsp;&nbsp;return num + 3;<br>}<br>var answer = plusThree(5); // 8</blockquote>
<code>plusThree</code> takes an <dfn>argument</dfn> for <code>num</code> and returns a value equal to <code>num + 3</code>.
</section>

## Instructions
<section id='instructions'>
Create a function <code>timesFive</code> that accepts one argument, multiplies it by <code>5</code>, and returns the new value. See the last line in the editor for an example of how you can test your <code>timesFive</code> function.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
function minusSeven(num) {
  return num - 7;
}

// Only change code below this line



console.log(minusSeven(10));
```

</div>



</section>

## Solution
<section id='solution'>


```js
function timesFive(num) {
  return num * 5;
}
timesFive(10);
```

</section>
<hr>

# 52. Understanding Undefined Value returned from a Function

## Description
<section id='description'>
A function can include the <code>return</code> statement but it does not have to. In the case that the function doesn't have a <code>return</code> statement, when you call it, the function processes the inner code but the returned value is <code>undefined</code>.
<strong>Example</strong>
<blockquote>var sum = 0;<br>function addSum(num) {<br>&nbsp;&nbsp;sum = sum + num;<br>}<br>var returnedValue = addSum(3); // sum will be modified but returned value is undefined</blockquote>
<code>addSum</code> is a function without a <code>return</code> statement. The function will change the global <code>sum</code> variable but the returned value of the function is <code>undefined</code>
</section>

## Instructions
<section id='instructions'>
Create a function <code>addFive</code> without any arguments. This function adds 5 to the <code>sum</code> variable, but its returned value is <code>undefined</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var sum = 0;
function addThree() {
  sum = sum + 3;
}

// Only change code below this line



// Only change code above this line
var returnedValue = addFive();
```

</div>


### After Test
<div id='js-teardown'>

```js
var sum = 0;
function addThree() {sum = sum + 3;}
addThree();
addFive();
```

</div>

</section>

## Solution
<section id='solution'>


```js
function addFive() {
 sum = sum + 5;
}
```

</section>
<hr>

# 53. Assignment with a Returned Value

## Description
<section id='description'>
If you'll recall from our discussion of <a href="learn/javascript-algorithms-and-data-structures/basic-javascript/storing-values-with-the-assignment-operator" target="_blank">Storing Values with the Assignment Operator</a>, everything to the right of the equal sign is resolved before the value is assigned. This means we can take the return value of a function and assign it to a variable.
Assume we have pre-defined a function <code>sum</code> which adds two numbers together, then:
<code>ourSum = sum(5, 12);</code>
will call <code>sum</code> function, which returns a value of <code>17</code> and assigns it to <code>ourSum</code> variable.
</section>

## Instructions
<section id='instructions'>
Call the <code>processArg</code> function with an argument of <code>7</code> and assign its return value to the variable <code>processed</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var changed = 0;

function change(num) {
  return (num + 5) / 3;
}

changed = change(10);

// Setup
var processed = 0;

function processArg(num) {
  return (num + 3) / 5;
}

// Only change code below this line


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){return "processed = " + processed})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var processed = 0;

function processArg(num) {
  return (num + 3) / 5;
}

processed = processArg(7);
```

</section>
<hr>

# 54. Stand in Line

## Description
<section id='description'>
In Computer Science a <dfn>queue</dfn> is an abstract <dfn>Data Structure</dfn> where items are kept in order. New items can be added at the back of the <code>queue</code> and old items are taken off from the front of the <code>queue</code>.
Write a function <code>nextInLine</code> which takes an array (<code>arr</code>) and a number (<code>item</code>) as arguments.
Add the number to the end of the array, then remove the first element of the array.
The <code>nextInLine</code> function should then return the element that was removed.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function nextInLine(arr, item) {
  // Your code here

  return item;  // Change this line
}

// Test Setup
var testArr = [1,2,3,4,5];

// Display Code
console.log("Before: " + JSON.stringify(testArr));
console.log(nextInLine(testArr, 6)); // Modify this line to test
console.log("After: " + JSON.stringify(testArr));
```

</div>

### Before Test
<div id='js-setup'>

```js
var logOutput = [];
var originalConsole = console
function capture() {
    var nativeLog = console.log;
    console.log = function (message) {
        logOutput.push(message);
        if(nativeLog.apply) {
          nativeLog.apply(originalConsole, arguments);
        } else {
          var nativeMsg = Array.prototype.slice.apply(arguments).join(' ');
          nativeLog(nativeMsg);
        }
    };
}

function uncapture() {
  console.log = originalConsole.log;
}

capture();
```

</div>

### After Test
<div id='js-teardown'>

```js
uncapture();
testArr = [1,2,3,4,5];
(function() { return logOutput.join("\n");})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var testArr = [ 1,2,3,4,5];

function nextInLine(arr, item) {
    arr.push(item);
    return arr.shift();
}
```

</section>
<hr>

# 55. Understanding Boolean Values

## Description
<section id='description'>
Another data type is the <dfn>Boolean</dfn>. <code>Booleans</code> may only be one of two values: <code>true</code> or <code>false</code>. They are basically little on-off switches, where <code>true</code> is "on" and <code>false</code> is "off."  These two states are mutually exclusive.
<strong>Note</strong><br><code>Boolean</code> values are never written with quotes. The <code>strings</code> <code>"true"</code> and <code>"false"</code> are not <code>Boolean</code> and have no special meaning in JavaScript.
</section>

## Instructions
<section id='instructions'>
Modify the <code>welcomeToBooleans</code> function so that it returns <code>true</code> instead of <code>false</code> when the run button is clicked.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function welcomeToBooleans() {

  // Only change code below this line.

  return false; // Change this line

  // Only change code above this line.
}
```

</div>


### After Test
<div id='js-teardown'>

```js
welcomeToBooleans();
```

</div>

</section>

## Solution
<section id='solution'>


```js
function welcomeToBooleans() {
  return true; // Change this line
}
```

</section>
<hr>

# 56. Use Conditional Logic with If Statements

## Description
<section id='description'>
<code>If</code> statements are used to make decisions in code. The keyword <code>if</code> tells JavaScript to execute the code in the curly braces under certain conditions, defined in the parentheses. These conditions are known as <code>Boolean</code> conditions and they may only be <code>true</code> or <code>false</code>.
When the condition evaluates to <code>true</code>, the program executes the statement inside the curly braces. When the Boolean condition evaluates to <code>false</code>, the statement inside the curly braces will not execute.
<strong>Pseudocode</strong>
<blockquote>if (<i>condition is true</i>) {<br>&nbsp;&nbsp;<i>statement is executed</i><br>}</blockquote>
<strong>Example</strong>
<blockquote>function test (myCondition) {<br>&nbsp;&nbsp;if (myCondition) {<br>&nbsp;&nbsp;&nbsp;&nbsp; return "It was true";<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;return "It was false";<br>}<br>test(true);  // returns "It was true"<br>test(false); // returns "It was false"</blockquote>
When <code>test</code> is called with a value of <code>true</code>, the <code>if</code> statement evaluates <code>myCondition</code> to see if it is <code>true</code> or not. Since it is <code>true</code>, the function returns <code>"It was true"</code>. When we call <code>test</code> with a value of <code>false</code>, <code>myCondition</code> is <em>not</em> <code>true</code> and the statement in the curly braces is not executed and the function returns <code>"It was false"</code>.
</section>

## Instructions
<section id='instructions'>
Create an <code>if</code> statement inside the function to return <code>"Yes, that was true"</code> if the parameter <code>wasThatTrue</code> is <code>true</code> and return <code>"No, that was false"</code> otherwise.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
function ourTrueOrFalse(isItTrue) {
  if (isItTrue) {
    return "Yes, it's true";
  }
  return "No, it's false";
}

// Setup
function trueOrFalse(wasThatTrue) {

  // Only change code below this line.



  // Only change code above this line.

}

// Change this value to test
trueOrFalse(true);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function trueOrFalse(wasThatTrue) {
  if (wasThatTrue) {
    return "Yes, that was true";
  }
  return "No, that was false";
}
```

</section>
<hr>

# 57. Comparison with the Equality Operator

## Description
<section id='description'>
There are many <dfn>Comparison Operators</dfn> in JavaScript. All of these operators return a boolean <code>true</code> or <code>false</code> value.
The most basic operator is the equality operator <code>==</code>. The equality operator compares two values and returns <code>true</code> if they're equivalent or <code>false</code> if they are not. Note that equality is different from assignment (<code>=</code>), which assigns the value at the right of the operator to a variable in the left.
<blockquote>function equalityTest(myVal) {<br>&nbsp;&nbsp;if (myVal == 10) {<br>&nbsp;&nbsp;&nbsp;&nbsp; return "Equal";<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;return "Not Equal";<br>}</blockquote>
If <code>myVal</code> is equal to <code>10</code>, the equality operator returns <code>true</code>, so the code in the curly braces will execute, and the function will return <code>"Equal"</code>. Otherwise, the function will return <code>"Not Equal"</code>.
In order for JavaScript to compare two different <code>data types</code> (for example, <code>numbers</code> and <code>strings</code>), it must convert one type to another. This is known as "Type Coercion". Once it does, however, it can compare terms as follows:
<blockquote>1   ==  1    // true<br>1   ==  2    // false<br>1   == '1'   // true<br>"3"  ==  3    // true</blockquote>
</section>

## Instructions
<section id='instructions'>
Add the <code>equality operator</code> to the indicated line so that the function will return "Equal" when <code>val</code> is equivalent to <code>12</code>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
function testEqual(val) {
  if (val) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

// Change this value to test
testEqual(10);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function testEqual(val) {
  if (val == 12) {
    return "Equal";
  }
  return "Not Equal";
}
```

</section>
<hr>

# 58. Comparison with the Strict Equality Operator

## Description
<section id='description'>
Strict equality (<code>===</code>) is the counterpart to the equality operator (<code>==</code>). However, unlike the equality operator, which attempts to convert both values being compared to a common type, the strict equality operator does not perform a type conversion.
If the values being compared have different types, they are considered unequal, and the strict equality operator will return false.
<strong>Examples</strong>
<blockquote>3 === 3   // true<br>3 === '3' // false</blockquote>
In the second example, <code>3</code> is a <code>Number</code> type and <code>'3'</code> is a <code>String</code> type.
</section>

## Instructions
<section id='instructions'>
Use the strict equality operator in the <code>if</code> statement so the function will return "Equal" when <code>val</code> is strictly equal to <code>7</code>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
function testStrict(val) {
  if (val) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

// Change this value to test
testStrict(10);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function testStrict(val) {
  if (val === 7) {
    return "Equal";
  }
  return "Not Equal";
}
```

</section>
<hr>

# 59. Practice comparing different values

## Description
<section id='description'>
In the last two challenges, we learned about the equality operator (<code>==</code>) and the strict equality operator (<code>===</code>). Let's do a quick review and practice using these operators some more.
If the values being compared are not of the same type, the equality operator will perform a type conversion, and then evaluate the values. However, the strict equality operator will compare both the data type and value as-is, without converting one type to the other.
<strong>Examples</strong>
<blockquote>3 == '3'  // returns true because JavaScript performs type conversion from string to number<br>3 === '3' // returns false because the types are different and type conversion is not performed</blockquote>
<strong>Note</strong><br>In JavaScript, you can determine the type of a variable or a value with the <code>typeof</code> operator, as follows:
<blockquote>typeof 3   // returns 'number'<br>typeof '3' // returns 'string'</blockquote>
</section>

## Instructions
<section id='instructions'>
The <code>compareEquality</code> function in the editor compares two values using the <code>equality operator</code>. Modify the function so that it returns "Equal" only when the values are strictly equal.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
function compareEquality(a, b) {
  if (a == b) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

// Change this value to test
compareEquality(10, "10");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function compareEquality(a,b) {
  if (a === b) {
    return "Equal";
  }
  return "Not Equal";
}
```

</section>
<hr>

# 60. Comparison with the Inequality Operator

## Description
<section id='description'>
The inequality operator (<code>!=</code>) is the opposite of the equality operator. It means "Not Equal" and returns <code>false</code> where equality would return <code>true</code> and <em>vice versa</em>. Like the equality operator, the inequality operator will convert data types of values while comparing.
<strong>Examples</strong>
<blockquote>1 != 2      // true<br>1 != "1"    // false<br>1 != '1'    // false<br>1 != true   // false<br>0 != false  // false</blockquote>
</section>

## Instructions
<section id='instructions'>
Add the inequality operator <code>!=</code> in the <code>if</code> statement so that the function will return "Not Equal" when <code>val</code> is not equivalent to <code>99</code>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
function testNotEqual(val) {
  if (val) { // Change this line
    return "Not Equal";
  }
  return "Equal";
}

// Change this value to test
testNotEqual(10);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function testNotEqual(val) {
  if (val != 99) {
    return "Not Equal";
  }
  return "Equal";
}
```

</section>
<hr>

# 61. Comparison with the Strict Inequality Operator

## Description
<section id='description'>
The strict inequality operator (<code>!==</code>) is the logical opposite of the strict equality operator. It means "Strictly Not Equal" and returns <code>false</code> where strict equality would return <code>true</code> and <em>vice versa</em>. Strict inequality will not convert data types.
<strong>Examples</strong>
<blockquote>3 !== 3   // false<br>3 !== '3' // true<br>4 !== 3   // true</blockquote>
</section>

## Instructions
<section id='instructions'>
Add the <code>strict inequality operator</code> to the <code>if</code> statement so the function will return "Not Equal" when <code>val</code> is not strictly equal to <code>17</code>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
function testStrictNotEqual(val) {
  // Only Change Code Below this Line

  if (val) {

  // Only Change Code Above this Line

    return "Not Equal";
  }
  return "Equal";
}

// Change this value to test
testStrictNotEqual(10);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function testStrictNotEqual(val) {
  if (val !== 17) {
    return "Not Equal";
  }
  return "Equal";
}
```

</section>
<hr>

# 62. Comparison with the Greater Than Operator

## Description
<section id='description'>
The greater than operator (<code>&gt;</code>) compares the values of two numbers. If the number to the left is greater than the number to the right, it returns <code>true</code>. Otherwise, it returns <code>false</code>.
Like the equality operator, greater than operator will convert data types of values while comparing.
<strong>Examples</strong>
<blockquote> 5 > 3   // true<br> 7 > '3' // true<br> 2 > 3   // false<br>'1' > 9  // false</blockquote>
</section>

## Instructions
<section id='instructions'>
Add the <code>greater than</code> operator to the indicated lines so that the return statements make sense.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function testGreaterThan(val) {
  if (val) {  // Change this line
    return "Over 100";
  }

  if (val) {  // Change this line
    return "Over 10";
  }

  return "10 or Under";
}

// Change this value to test
testGreaterThan(10);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function testGreaterThan(val) {
  if (val > 100) {  // Change this line
    return "Over 100";
  }
  if (val > 10) {  // Change this line
    return "Over 10";
  }
  return "10 or Under";
}
```

</section>
<hr>

# 63. Comparison with the Greater Than Or Equal To Operator

## Description
<section id='description'>
The <code>greater than or equal to</code> operator (<code>&gt;=</code>) compares the values of two numbers. If the number to the left is greater than or equal to the number to the right, it returns <code>true</code>. Otherwise, it returns <code>false</code>.
Like the equality operator, <code>greater than or equal to</code> operator will convert data types while comparing.
<strong>Examples</strong>
<blockquote> 6  >=  6  // true<br> 7  >= '3' // true<br> 2  >=  3  // false<br>'7' >=  9  // false</blockquote>
</section>

## Instructions
<section id='instructions'>
Add the <code>greater than or equal to</code> operator to the indicated lines so that the return statements make sense.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function testGreaterOrEqual(val) {
  if (val) {  // Change this line
    return "20 or Over";
  }

  if (val) {  // Change this line
    return "10 or Over";
  }

  return "Less than 10";
}

// Change this value to test
testGreaterOrEqual(10);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function testGreaterOrEqual(val) {
  if (val >= 20) {  // Change this line
    return "20 or Over";
  }

  if (val >= 10) {  // Change this line
    return "10 or Over";
  }

  return "Less than 10";
}
```

</section>
<hr>

# 64. Comparison with the Less Than Operator

## Description
<section id='description'>
The <dfn>less than</dfn> operator (<code>&lt;</code>) compares the values of two numbers. If the number to the left is less than the number to the right, it returns <code>true</code>. Otherwise, it returns <code>false</code>. Like the equality operator, <dfn>less than</dfn> operator converts data types while comparing.
<strong>Examples</strong>
<blockquote>2 &lt; 5  // true<br>'3' &lt; 7  // true<br>5 &lt; 5  // false<br>3 &lt; 2  // false<br>'8' &lt; 4  // false</blockquote>
</section>

## Instructions
<section id='instructions'>
Add the <code>less than</code> operator to the indicated lines so that the return statements make sense.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function testLessThan(val) {
  if (val) {  // Change this line
    return "Under 25";
  }

  if (val) {  // Change this line
    return "Under 55";
  }

  return "55 or Over";
}

// Change this value to test
testLessThan(10);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function testLessThan(val) {
  if (val < 25) {  // Change this line
    return "Under 25";
  }

  if (val < 55) {  // Change this line
    return "Under 55";
  }

  return "55 or Over";
}
```

</section>
<hr>

# 65. Comparison with the Less Than Or Equal To Operator

## Description
<section id='description'>
The <code>less than or equal to</code> operator (<code>&lt;=</code>) compares the values of two numbers. If the number to the left is less than or equal to the number to the right, it returns <code>true</code>. If the number on the left is greater than the number on the right, it returns <code>false</code>. Like the equality operator, <code>less than or equal to</code> converts data types.
<strong>Examples</strong>
<blockquote>4 &lt;= 5  // true<br>'7' &lt;= 7  // true<br>5 &lt;= 5  // true<br>3 &lt;= 2  // false<br>'8' &lt;= 4  // false</blockquote>
</section>

## Instructions
<section id='instructions'>
Add the <code>less than or equal to</code> operator to the indicated lines so that the return statements make sense.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function testLessOrEqual(val) {
  if (val) {  // Change this line
    return "Smaller Than or Equal to 12";
  }

  if (val) {  // Change this line
    return "Smaller Than or Equal to 24";
  }

  return "More Than 24";
}

// Change this value to test
testLessOrEqual(10);

```

</div>



</section>

## Solution
<section id='solution'>


```js
function testLessOrEqual(val) {
  if (val <= 12) {  // Change this line
    return "Smaller Than or Equal to 12";
  }

  if (val <= 24) {  // Change this line
    return "Smaller Than or Equal to 24";
  }

  return "More Than 24";
}
```

</section>
<hr>

# 66. Comparisons with the Logical And Operator

## Description
<section id='description'>
Sometimes you will need to test more than one thing at a time. The <dfn>logical and</dfn> operator (<code>&&</code>) returns <code>true</code> if and only if the <dfn>operands</dfn> to the left and right of it are true.
The same effect could be achieved by nesting an if statement inside another if:
<blockquote>if (num > 5) {<br>&nbsp;&nbsp;if (num < 10) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "Yes";<br>&nbsp;&nbsp;}<br>}<br>return "No";</blockquote>
will only return "Yes" if <code>num</code> is greater than <code>5</code> and less than <code>10</code>. The same logic can be written as:
<blockquote>if (num > 5 && num < 10) {<br>&nbsp;&nbsp;return "Yes";<br>}<br>return "No";</blockquote>
</section>

## Instructions
<section id='instructions'>
Combine the two if statements into one statement which will return <code>"Yes"</code> if <code>val</code> is less than or equal to <code>50</code> and greater than or equal to <code>25</code>. Otherwise, will return <code>"No"</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function testLogicalAnd(val) {
  // Only change code below this line

  if (val) {
    if (val) {
      return "Yes";
    }
  }

  // Only change code above this line
  return "No";
}

// Change this value to test
testLogicalAnd(10);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function testLogicalAnd(val) {
  if (val >= 25 && val <= 50) {
    return "Yes";
  }
  return "No";
}
```

</section>
<hr>

# 67. Comparisons with the Logical Or Operator

## Description
<section id='description'>
The <dfn>logical or</dfn> operator (<code>||</code>) returns <code>true</code> if either of the <dfn>operands</dfn> is <code>true</code>. Otherwise, it returns <code>false</code>.
The <dfn>logical or</dfn> operator is composed of two pipe symbols (<code>|</code>). This can typically be found between your Backspace and Enter keys.
The pattern below should look familiar from prior waypoints:
<blockquote>if (num > 10) {<br>&nbsp;&nbsp;return "No";<br>}<br>if (num < 5) {<br>&nbsp;&nbsp;return "No";<br>}<br>return "Yes";</blockquote>
will return "Yes" only if <code>num</code> is between <code>5</code> and <code>10</code> (5 and 10 included). The same logic can be written as:
<blockquote>if (num > 10 || num < 5) {<br>&nbsp;&nbsp;return "No";<br>}<br>return "Yes";</blockquote>
</section>

## Instructions
<section id='instructions'>
Combine the two <code>if</code> statements into one statement which returns <code>"Outside"</code> if <code>val</code> is not between <code>10</code> and <code>20</code>, inclusive. Otherwise, return <code>"Inside"</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function testLogicalOr(val) {
  // Only change code below this line

  if (val) {
    return "Outside";
  }

  if (val) {
    return "Outside";
  }

  // Only change code above this line
  return "Inside";
}

// Change this value to test
testLogicalOr(15);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function testLogicalOr(val) {
  if (val < 10 || val > 20) {
    return "Outside";
  }
  return "Inside";
}
```

</section>
<hr>

# 68. Introducing Else Statements

## Description
<section id='description'>
When a condition for an <code>if</code> statement is true, the block of code following it is executed. What about when that condition is false?  Normally nothing would happen. With an <code>else</code> statement, an alternate block of code can be executed.
<blockquote>if (num > 10) {<br>&nbsp;&nbsp;return "Bigger than 10";<br>} else {<br>&nbsp;&nbsp;return "10 or Less";<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Combine the <code>if</code> statements into a single <code>if/else</code> statement.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function testElse(val) {
  var result = "";
  // Only change code below this line

  if (val > 5) {
    result = "Bigger than 5";
  }

  if (val <= 5) {
    result = "5 or Smaller";
  }

  // Only change code above this line
  return result;
}

// Change this value to test
testElse(4);

```

</div>



</section>

## Solution
<section id='solution'>


```js
function testElse(val) {
  var result = "";
  if(val > 5) {
    result = "Bigger than 5";
  } else {
    result = "5 or Smaller";
  }
  return result;
}
```

</section>
<hr>

# 69. Introducing Else If Statements

## Description
<section id='description'>
If you have multiple conditions that need to be addressed, you can chain <code>if</code> statements together with <code>else if</code> statements.
<blockquote>if (num > 15) {<br>&nbsp;&nbsp;return "Bigger than 15";<br>} else if (num < 5) {<br>&nbsp;&nbsp;return "Smaller than 5";<br>} else {<br>&nbsp;&nbsp;return "Between 5 and 15";<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Convert the logic to use <code>else if</code> statements.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  }

  if (val < 5) {
    return "Smaller than 5";
  }

  return "Between 5 and 10";
}

// Change this value to test
testElseIf(7);

```

</div>



</section>

## Solution
<section id='solution'>


```js
function testElseIf(val) {
  if(val > 10) {
    return "Greater than 10";
  } else if(val < 5) {
    return "Smaller than 5";
  } else {
    return "Between 5 and 10";
  }
}
```

</section>
<hr>

# 70. Logical Order in If Else Statements

## Description
<section id='description'>
Order is important in <code>if</code>, <code>else if</code> statements.
The function is executed from top to bottom so you will want to be careful of what statement comes first.
Take these two functions as an example.
Here's the first:
<blockquote>function foo(x) {<br>&nbsp;&nbsp;if (x < 1) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "Less than one";<br>&nbsp;&nbsp;} else if (x < 2) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "Less than two";<br>&nbsp;&nbsp;} else {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "Greater than or equal to two";<br>&nbsp;&nbsp;}<br>}</blockquote>
And the second just switches the order of the statements:
<blockquote>function bar(x) {<br>&nbsp;&nbsp;if (x < 2) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "Less than two";<br>&nbsp;&nbsp;} else if (x < 1) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "Less than one";<br>&nbsp;&nbsp;} else {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "Greater than or equal to two";<br>&nbsp;&nbsp;}<br>}</blockquote>
While these two functions look nearly identical if we pass a number to both we get different outputs.
<blockquote>foo(0) // "Less than one"<br>bar(0) // "Less than two"</blockquote>
</section>

## Instructions
<section id='instructions'>
Change the order of logic in the function so that it will return the correct statements in all cases.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function orderMyLogic(val) {
  if (val < 10) {
    return "Less than 10";
  } else if (val < 5) {
    return "Less than 5";
  } else {
    return "Greater than or equal to 10";
  }
}

// Change this value to test
orderMyLogic(7);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function orderMyLogic(val) {
  if(val < 5) {
    return "Less than 5";
  } else if (val < 10) {
    return "Less than 10";
  } else {
    return "Greater than or equal to 10";
  }
}
```

</section>
<hr>

# 71. Chaining If Else Statements

## Description
<section id='description'>
<code>if/else</code> statements can be chained together for complex logic. Here is <dfn>pseudocode</dfn> of multiple chained <code>if</code> / <code>else if</code> statements:
<blockquote>if (<em>condition1</em>) {<br>&nbsp;&nbsp;<em>statement1</em><br>} else if (<em>condition2</em>) {<br>&nbsp;&nbsp;<em>statement2</em><br>} else if (<em>condition3</em>) {<br>&nbsp;&nbsp;<em>statement3</em><br>. . .<br>} else {<br>&nbsp;&nbsp;<em>statementN</em><br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Write chained <code>if</code>/<code>else if</code> statements to fulfill the following conditions:
<code>num &lt;   5</code> - return "Tiny"<br><code>num &lt;  10</code> - return "Small"<br><code>num &lt; 15</code> - return "Medium"<br><code>num &lt; 20</code> - return "Large"<br><code>num >= 20</code>  - return "Huge"
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function testSize(num) {
  // Only change code below this line


  return "Change Me";
  // Only change code above this line
}

// Change this value to test
testSize(7);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function testSize(num) {
  if (num < 5) {
    return "Tiny";
  } else if (num < 10) {
    return "Small";
  } else if (num < 15) {
    return "Medium";
  } else if (num < 20) {
    return "Large";
  } else {
    return "Huge";
  }
}
```

</section>
<hr>

# 72. Golf Code

## Description
<section id='description'>
In the game of <a href="https://en.wikipedia.org/wiki/Golf" target="_blank">golf</a> each hole has a <code>par</code> meaning the average number of <code>strokes</code> a golfer is expected to make in order to sink the ball in a hole to complete the play. Depending on how far above or below <code>par</code> your <code>strokes</code> are, there is a different nickname.
Your function will be passed <code>par</code> and <code>strokes</code> arguments. Return the correct string according to this table which lists the strokes in order of priority; top (highest) to bottom (lowest):
<table class="table table-striped"><thead><tr><th>Strokes</th><th>Return</th></tr></thead><tbody><tr><td>1</td><td>"Hole-in-one!"</td></tr><tr><td>&lt;= par - 2</td><td>"Eagle"</td></tr><tr><td>par - 1</td><td>"Birdie"</td></tr><tr><td>par</td><td>"Par"</td></tr><tr><td>par + 1</td><td>"Bogey"</td></tr><tr><td>par + 2</td><td>"Double Bogey"</td></tr><tr><td>&gt;= par + 3</td><td>"Go Home!"</td></tr></tbody></table>
<code>par</code> and <code>strokes</code> will always be numeric and positive. We have added an array of all the names for your convenience.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];
function golfScore(par, strokes) {
  // Only change code below this line


  return "Change Me";
  // Only change code above this line
}

// Change these values to test
golfScore(5, 4);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function golfScore(par, strokes) {
  if (strokes === 1) {
    return "Hole-in-one!";
  }

  if (strokes <= par - 2) {
    return "Eagle";
  }

  if (strokes === par - 1) {
    return "Birdie";
  }

  if (strokes === par) {
    return "Par";
  }

  if (strokes === par + 1) {
    return "Bogey";
  }

  if(strokes === par + 2) {
    return "Double Bogey";
  }

  return "Go Home!";
}
```

</section>
<hr>

# 73. Selecting from Many Options with Switch Statements

## Description
<section id='description'>
If you have many options to choose from, use a <code>switch</code> statement. A <code>switch</code> statement tests a value and can have many <code>case</code> statements which define various possible values. Statements are executed from the first matched <code>case</code> value until a <code>break</code> is encountered.
Here is a <dfn>pseudocode</dfn> example:
<blockquote>switch(num) {<br>&nbsp;&nbsp;case value1:<br>&nbsp;&nbsp;&nbsp;&nbsp;statement1;<br>&nbsp;&nbsp;&nbsp;&nbsp;break;<br>&nbsp;&nbsp;case value2:<br>&nbsp;&nbsp;&nbsp;&nbsp;statement2;<br>&nbsp;&nbsp;&nbsp;&nbsp;break;<br>...<br>&nbsp;&nbsp;case valueN:<br>&nbsp;&nbsp;&nbsp;&nbsp;statementN;<br>&nbsp;&nbsp;&nbsp;&nbsp;break;<br>}</blockquote>
<code>case</code> values are tested with strict equality (<code>===</code>). The <code>break</code> tells JavaScript to stop executing statements. If the <code>break</code> is omitted, the next statement will be executed.
</section>

## Instructions
<section id='instructions'>
Write a switch statement which tests <code>val</code> and sets <code>answer</code> for the following conditions:<br><code>1</code> - "alpha"<br><code>2</code> - "beta"<br><code>3</code> - "gamma"<br><code>4</code> - "delta"
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function caseInSwitch(val) {
  var answer = "";
  // Only change code below this line



  // Only change code above this line
  return answer;
}

// Change this value to test
caseInSwitch(1);

```

</div>



</section>

## Solution
<section id='solution'>


```js
function caseInSwitch(val) {
  var answer = "";

  switch(val) {
    case 1:
      answer = "alpha";
      break;
    case 2:
      answer = "beta";
      break;
    case 3:
      answer = "gamma";
      break;
    case 4:
      answer = "delta";
  }
  return answer;
}
```

</section>
<hr>

# 74. Adding a Default Option in Switch Statements

## Description
<section id='description'>
In a <code>switch</code> statement you may not be able to specify all possible values as <code>case</code> statements. Instead, you can add the <code>default</code> statement which will be executed if no matching <code>case</code> statements are found. Think of it like the final <code>else</code> statement in an <code>if/else</code> chain.
A <code>default</code> statement should be the last case.
<blockquote>switch (num) {<br>&nbsp;&nbsp;case value1:<br>&nbsp;&nbsp;&nbsp;&nbsp;statement1;<br>&nbsp;&nbsp;&nbsp;&nbsp;break;<br>&nbsp;&nbsp;case value2:<br>&nbsp;&nbsp;&nbsp;&nbsp;statement2;<br>&nbsp;&nbsp;&nbsp;&nbsp;break;<br>...<br>&nbsp;&nbsp;default:<br>&nbsp;&nbsp;&nbsp;&nbsp;defaultStatement;<br>&nbsp;&nbsp;&nbsp;&nbsp;break;<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Write a switch statement to set <code>answer</code> for the following conditions:<br><code>"a"</code> - "apple"<br><code>"b"</code> - "bird"<br><code>"c"</code> - "cat"<br><code>default</code> - "stuff"
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function switchOfStuff(val) {
  var answer = "";
  // Only change code below this line



  // Only change code above this line
  return answer;
}

// Change this value to test
switchOfStuff(1);

```

</div>



</section>

## Solution
<section id='solution'>


```js
function switchOfStuff(val) {
  var answer = "";

  switch(val) {
    case "a":
      answer = "apple";
      break;
    case "b":
      answer = "bird";
      break;
    case "c":
      answer = "cat";
      break;
    default:
      answer = "stuff";
  }
  return answer;
}
```

</section>
<hr>

# 75. Multiple Identical Options in Switch Statements

## Description
<section id='description'>
If the <code>break</code> statement is omitted from a <code>switch</code> statement's <code>case</code>, the following <code>case</code> statement(s) are executed until a <code>break</code> is encountered. If you have multiple inputs with the same output, you can represent them in a <code>switch</code> statement like this:
<blockquote>switch(val) {<br>&nbsp;&nbsp;case 1:<br>&nbsp;&nbsp;case 2:<br>&nbsp;&nbsp;case 3:<br>&nbsp;&nbsp;&nbsp;&nbsp;result = "1, 2, or 3";<br>&nbsp;&nbsp;&nbsp;&nbsp;break;<br>&nbsp;&nbsp;case 4:<br>&nbsp;&nbsp;&nbsp;&nbsp;result = "4 alone";<br>}</blockquote>
Cases for 1, 2, and 3 will all produce the same result.
</section>

## Instructions
<section id='instructions'>
Write a switch statement to set <code>answer</code> for the following ranges:<br><code>1-3</code> - "Low"<br><code>4-6</code> - "Mid"<br><code>7-9</code> - "High"
<strong>Note</strong><br>You will need to have a <code>case</code> statement for each number in the range.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function sequentialSizes(val) {
  var answer = "";
  // Only change code below this line



  // Only change code above this line
  return answer;
}

// Change this value to test
sequentialSizes(1);

```

</div>



</section>

## Solution
<section id='solution'>


```js
function sequentialSizes(val) {
  var answer = "";

  switch(val) {
    case 1:
    case 2:
    case 3:
      answer = "Low";
      break;
    case 4:
    case 5:
    case 6:
      answer = "Mid";
      break;
    case 7:
    case 8:
    case 9:
      answer = "High";
  }

  return answer;
}
```

</section>
<hr>

# 76. Replacing If Else Chains with Switch

## Description
<section id='description'>
If you have many options to choose from, a <code>switch</code> statement can be easier to write than many chained <code>if</code>/<code>else if</code> statements. The following:
<blockquote>if (val === 1) {<br>&nbsp;&nbsp;answer = "a";<br>} else if (val === 2) {<br>&nbsp;&nbsp;answer = "b";<br>} else {<br>&nbsp;&nbsp;answer = "c";<br>}</blockquote>
can be replaced with:
<blockquote>switch(val) {<br>&nbsp;&nbsp;case 1:<br>&nbsp;&nbsp;&nbsp;&nbsp;answer = "a";<br>&nbsp;&nbsp;&nbsp;&nbsp;break;<br>&nbsp;&nbsp;case 2:<br>&nbsp;&nbsp;&nbsp;&nbsp;answer = "b";<br>&nbsp;&nbsp;&nbsp;&nbsp;break;<br>&nbsp;&nbsp;default:<br>&nbsp;&nbsp;&nbsp;&nbsp;answer = "c";<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Change the chained <code>if</code>/<code>else if</code> statements into a <code>switch</code> statement.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function chainToSwitch(val) {
  var answer = "";
  // Only change code below this line

  if (val === "bob") {
    answer = "Marley";
  } else if (val === 42) {
    answer = "The Answer";
  } else if (val === 1) {
    answer = "There is no #1";
  } else if (val === 99) {
    answer = "Missed me by this much!";
  } else if (val === 7) {
    answer = "Ate Nine";
  }

  // Only change code above this line
  return answer;
}

// Change this value to test
chainToSwitch(7);

```

</div>



</section>

## Solution
<section id='solution'>


```js
function chainToSwitch(val) {
  var answer = "";

  switch(val) {
    case "bob":
      answer = "Marley";
      break;
    case 42:
      answer = "The Answer";
      break;
    case 1:
      answer = "There is no #1";
      break;
    case 99:
      answer = "Missed me by this much!";
      break;
    case 7:
      answer = "Ate Nine";
  }
  return answer;
}
```

</section>
<hr>

# 77. Returning Boolean Values from Functions

## Description
<section id='description'>
You may recall from <a href="learn/javascript-algorithms-and-data-structures/basic-javascript/comparison-with-the-equality-operator" target="_blank">Comparison with the Equality Operator</a> that all comparison operators return a boolean <code>true</code> or <code>false</code> value.
Sometimes people use an if/else statement to do a comparison, like this:
<blockquote>function isEqual(a,b) {<br>&nbsp;&nbsp;if (a === b) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return true;<br>&nbsp;&nbsp;} else {<br>&nbsp;&nbsp;&nbsp;&nbsp;return false;<br>&nbsp;&nbsp;}<br>}</blockquote>
But there's a better way to do this. Since <code>===</code> returns <code>true</code> or <code>false</code>, we can return the result of the comparison:
<blockquote>function isEqual(a,b) {<br>&nbsp;&nbsp;return a === b;<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Fix the function <code>isLess</code> to remove the <code>if/else</code> statements.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function isLess(a, b) {
  // Fix this code
  if (a < b) {
    return true;
  } else {
    return false;
  }
}

// Change these values to test
isLess(10, 15);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function isLess(a, b) {
  return a < b;
}
```

</section>
<hr>

# 78. Return Early Pattern for Functions

## Description
<section id='description'>
When a <code>return</code> statement is reached, the execution of the current function stops and control returns to the calling location.
<strong>Example</strong>
<blockquote>function myFun() {<br>&nbsp;&nbsp;console.log("Hello");<br>&nbsp;&nbsp;return "World";<br>&nbsp;&nbsp;console.log("byebye")<br>}<br>myFun();</blockquote>
The above outputs "Hello" to the console, returns "World", but <code>"byebye"</code> is never output, because the function exits at the <code>return</code> statement.
</section>

## Instructions
<section id='instructions'>
Modify the function <code>abTest</code> so that if <code>a</code> or <code>b</code> are less than <code>0</code> the function will immediately exit with a value of <code>undefined</code>.
<strong>Hint</strong><br>Remember that <a href='http://www.freecodecamp.org/challenges/understanding-uninitialized-variables' target='_blank'><code>undefined</code> is a keyword</a>, not a string.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
function abTest(a, b) {
  // Only change code below this line



  // Only change code above this line

  return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
}

// Change values below to test your code
abTest(2,2);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function abTest(a, b) {
  if(a < 0 || b < 0) {
    return undefined;
  }
  return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
}
```

</section>
<hr>

# 79. Counting Cards

## Description
<section id='description'>
In the casino game Blackjack, a player can gain an advantage over the house by keeping track of the relative number of high and low cards remaining in the deck. This is called <a href='https://en.wikipedia.org/wiki/Card_counting' target='_blank'>Card Counting</a>.
Having more high cards remaining in the deck favors the player. Each card is assigned a value according to the table below. When the count is positive, the player should bet high. When the count is zero or negative, the player should bet low.
<table class="table table-striped"><thead><tr><th>Count Change</th><th>Cards</th></tr></thead><tbody><tr><td>+1</td><td>2, 3, 4, 5, 6</td></tr><tr><td>0</td><td>7, 8, 9</td></tr><tr><td>-1</td><td>10, 'J', 'Q', 'K', 'A'</td></tr></tbody></table>
You will write a card counting function. It will receive a <code>card</code> parameter, which can be a number or a string, and increment or decrement the global <code>count</code> variable according to the card's value (see table). The function will then return a string with the current count and the string <code>Bet</code> if the count is positive, or <code>Hold</code> if the count is zero or negative. The current count and the player's decision (<code>Bet</code> or <code>Hold</code>) should be separated by a single space.
<strong>Example Output</strong><br><code>-3 Hold</code><br><code>5 Bet</code>
<strong>Hint</strong><br>Do NOT reset <code>count</code> to 0 when value is 7, 8, or 9.<br>Do NOT return an array.<br>Do NOT include quotes (single or double) in the output.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var count = 0;

function cc(card) {
  // Only change code below this line


  return "Change Me";
  // Only change code above this line
}

// Add/remove calls to test your function.
// Note: Only the last will display
cc(2); cc(3); cc(7); cc('K'); cc('A');
```

</div>



</section>

## Solution
<section id='solution'>


```js
var count = 0;
function cc(card) {
  switch(card) {
    case 2:
    case 3:
    case 4:
    case 5:
    case 6:
      count++;
      break;
    case 10:
    case 'J':
    case 'Q':
    case 'K':
    case 'A':
      count--;
  }
  if(count > 0) {
    return count + " Bet";
  } else {
    return count + " Hold";
  }
}
```

</section>
<hr>

# 80. Build JavaScript Objects

## Description
<section id='description'>
You may have heard the term <code>object</code> before.
Objects are similar to <code>arrays</code>, except that instead of using indexes to access and modify their data, you access the data in objects through what are called <code>properties</code>.
Objects are useful for storing data in a structured way, and can represent real world objects, like a cat.
Here's a sample cat object:
<blockquote>var cat = {<br>&nbsp;&nbsp;"name": "Whiskers",<br>&nbsp;&nbsp;"legs": 4,<br>&nbsp;&nbsp;"tails": 1,<br>&nbsp;&nbsp;"enemies": ["Water", "Dogs"]<br>};</blockquote>
In this example, all the properties are stored as strings, such as - <code>"name"</code>, <code>"legs"</code>, and <code>"tails"</code>. However, you can also use numbers as properties. You can even omit the quotes for single-word string properties, as follows:
<blockquote>var anotherObject = {<br>&nbsp;&nbsp;make: "Ford",<br>&nbsp;&nbsp;5: "five",<br>&nbsp;&nbsp;"model": "focus"<br>};</blockquote>
However, if your object has any non-string properties, JavaScript will automatically typecast them as strings.
</section>

## Instructions
<section id='instructions'>
Make an object that represents a dog called <code>myDog</code> which contains the properties <code>"name"</code> (a string), <code>"legs"</code>, <code>"tails"</code> and <code>"friends"</code>.
You can set these object properties to whatever values you want, as long <code>"name"</code> is a string, <code>"legs"</code> and <code>"tails"</code> are numbers, and <code>"friends"</code> is an array.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};

// Only change code below this line.

var myDog = {




};
```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return z;})(myDog);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};
```

</section>
<hr>

# 81. Accessing Object Properties with Dot Notation

## Description
<section id='description'>
There are two ways to access the properties of an object: dot notation (<code>.</code>) and bracket notation (<code>[]</code>), similar to an array.
Dot notation is what you use when you know the name of the property you're trying to access ahead of time.
Here is a sample of using dot notation (<code>.</code>) to read an object's property:
<blockquote>var myObj = {<br>&nbsp;&nbsp;prop1: "val1",<br>&nbsp;&nbsp;prop2: "val2"<br>};<br>var prop1val = myObj.prop1; // val1<br>var prop2val = myObj.prop2; // val2</blockquote>
</section>

## Instructions
<section id='instructions'>
Read in the property values of <code>testObj</code> using dot notation. Set the variable <code>hatValue</code> equal to the object's property <code>hat</code> and set the variable <code>shirtValue</code> equal to the object's property <code>shirt</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

// Only change code below this line

var hatValue = testObj;      // Change this line
var shirtValue = testObj;    // Change this line
```

</div>


### After Test
<div id='js-teardown'>

```js
(function(a,b) { return "hatValue = '" + a + "', shirtValue = '" + b + "'"; })(hatValue,shirtValue);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

var hatValue = testObj.hat;
var shirtValue = testObj.shirt;
```

</section>
<hr>

# 82. Accessing Object Properties with Bracket Notation

## Description
<section id='description'>
The second way to access the properties of an object is bracket notation (<code>[]</code>). If the property of the object you are trying to access has a space in its name, you will need to use bracket notation.
However, you can still use bracket notation on object properties without spaces.
Here is a sample of using bracket notation to read an object's property:
<blockquote>var myObj = {<br>&nbsp;&nbsp;"Space Name": "Kirk",<br>&nbsp;&nbsp;"More Space": "Spock",<br>&nbsp;&nbsp;"NoSpace": "USS Enterprise"<br>};<br>myObj["Space Name"]; // Kirk<br>myObj['More Space']; // Spock<br>myObj["NoSpace"];    // USS Enterprise</blockquote>
Note that property names with spaces in them must be in quotes (single or double).
</section>

## Instructions
<section id='instructions'>
Read the values of the properties <code>"an entree"</code> and <code>"the drink"</code> of <code>testObj</code> using bracket notation and assign them to <code>entreeValue</code> and <code>drinkValue</code> respectively.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};

// Only change code below this line

var entreeValue = testObj;   // Change this line
var drinkValue = testObj;    // Change this line
```

</div>


### After Test
<div id='js-teardown'>

```js
(function(a,b) { return "entreeValue = '" + a + "', drinkValue = '" + b + "'"; })(entreeValue,drinkValue);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};
var entreeValue = testObj["an entree"];
var drinkValue = testObj['the drink'];
```

</section>
<hr>

# 83. Accessing Object Properties with Variables

## Description
<section id='description'>
Another use of bracket notation on objects is to access a property which is stored as the value of a variable. This can be very useful for iterating through an object's properties or when accessing a lookup table.
Here is an example of using a variable to access a property:
<blockquote>var dogs = {<br>&nbsp;&nbsp;Fido: "Mutt",
  Hunter: "Doberman",
  Snoopie: "Beagle"<br>};<br>var myDog = "Hunter";<br>var myBreed = dogs[myDog];<br>console.log(myBreed); // "Doberman"</blockquote>
Another way you can use this concept is when the property's name is collected dynamically during the program execution, as follows:
<blockquote>var someObj = {<br>&nbsp;&nbsp;propName: "John"<br>};<br>function propPrefix(str) {<br>&nbsp;&nbsp;var s = "prop";<br>&nbsp;&nbsp;return s + str;<br>}<br>var someProp = propPrefix("Name"); // someProp now holds the value 'propName'<br>console.log(someObj[someProp]); // "John"</blockquote>
Note that we do <em>not</em> use quotes around the variable name when using it to access the property because we are using the <em>value</em> of the variable, not the <em>name</em>.
</section>

## Instructions
<section id='instructions'>
Use the <code>playerNumber</code> variable to look up player <code>16</code> in <code>testObj</code> using bracket notation. Then assign that name to the <code>player</code> variable.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var testObj = {
  12: "Namath",
  16: "Montana",
  19: "Unitas"
};

// Only change code below this line;

var playerNumber;       // Change this Line
var player = testObj;   // Change this Line
```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof player !== "undefined"){(function(v){return v;})(player);}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var testObj = {
  12: "Namath",
  16: "Montana",
  19: "Unitas"
};
var playerNumber = 16;
var player = testObj[playerNumber];
```

</section>
<hr>

# 84. Updating Object Properties

## Description
<section id='description'>
After you've created a JavaScript object, you can update its properties at any time just like you would update any other variable. You can use either dot or bracket notation to update.
For example, let's look at <code>ourDog</code>:
<blockquote>var ourDog = {<br>&nbsp;&nbsp;"name": "Camper",<br>&nbsp;&nbsp;"legs": 4,<br>&nbsp;&nbsp;"tails": 1,<br>&nbsp;&nbsp;"friends": ["everything!"]<br>};</blockquote>
Since he's a particularly happy dog, let's change his name to "Happy Camper". Here's how we update his object's name property:
<code>ourDog.name = "Happy Camper";</code> or
<code>ourDog["name"] = "Happy Camper";</code>
Now when we evaluate <code>ourDog.name</code>, instead of getting "Camper", we'll get his new name, "Happy Camper".
</section>

## Instructions
<section id='instructions'>
Update the <code>myDog</code> object's name property. Let's change her name from "Coder" to "Happy Coder". You can use either dot or bracket notation.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};

ourDog.name = "Happy Camper";

// Setup
var myDog = {
  "name": "Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

// Only change code below this line.


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return z;})(myDog);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myDog = {
  "name": "Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};
myDog.name = "Happy Coder";
```

</section>
<hr>

# 85. Add New Properties to a JavaScript Object

## Description
<section id='description'>
You can add new properties to existing JavaScript objects the same way you would modify them.
Here's how we would add a <code>"bark"</code> property to <code>ourDog</code>:
<code>ourDog.bark = "bow-wow";</code>
or
<code>ourDog["bark"] = "bow-wow";</code>
Now when we evaluate <code>ourDog.bark</code>, we'll get his bark, "bow-wow".
</section>

## Instructions
<section id='instructions'>
Add a <code>"bark"</code> property to <code>myDog</code> and set it to a dog sound, such as "woof". You may use either dot or bracket notation.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"]
};

ourDog.bark = "bow-wow";

// Setup
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

// Only change code below this line.

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return z;})(myDog);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};
myDog.bark = "Woof Woof";
```

</section>
<hr>

# 86. Delete Properties from a JavaScript Object

## Description
<section id='description'>
We can also delete properties from objects like this:
<code>delete ourDog.bark;</code>
</section>

## Instructions
<section id='instructions'>
Delete the <code>"tails"</code> property from <code>myDog</code>. You may use either dot or bracket notation.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"],
  "bark": "bow-wow"
};

delete ourDog.bark;

// Setup
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};

// Only change code below this line.


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(z){return z;})(myDog);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var ourDog = {
  "name": "Camper",
  "legs": 4,
  "tails": 1,
  "friends": ["everything!"],
  "bark": "bow-wow"
};
var myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};
delete myDog.tails;
```

</section>
<hr>

# 87. Using Objects for Lookups

## Description
<section id='description'>
Objects can be thought of as a key/value storage, like a dictionary. If you have tabular data, you can use an object to "lookup" values rather than a <code>switch</code> statement or an <code>if/else</code> chain. This is most useful when you know that your input data is limited to a certain range.
Here is an example of a simple reverse alphabet lookup:
<blockquote>var alpha = {<br>&nbsp;&nbsp;1:"Z",<br>&nbsp;&nbsp;2:"Y",<br>&nbsp;&nbsp;3:"X",<br>&nbsp;&nbsp;4:"W",<br>&nbsp;&nbsp;...<br>&nbsp;&nbsp;24:"C",<br>&nbsp;&nbsp;25:"B",<br>&nbsp;&nbsp;26:"A"<br>};<br>alpha[2]; // "Y"<br>alpha[24]; // "C"<br><br>var value = 2;<br>alpha[value]; // "Y"</blockquote>
</section>

## Instructions
<section id='instructions'>
Convert the switch statement into an object called <code>lookup</code>. Use it to look up <code>val</code> and assign the associated string to the <code>result</code> variable.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
function phoneticLookup(val) {
  var result = "";

  // Only change code below this line
  switch(val) {
    case "alpha":
      result = "Adams";
      break;
    case "bravo":
      result = "Boston";
      break;
    case "charlie":
      result = "Chicago";
      break;
    case "delta":
      result = "Denver";
      break;
    case "echo":
      result = "Easy";
      break;
    case "foxtrot":
      result = "Frank";
  }

  // Only change code above this line
  return result;
}

// Change this value to test
phoneticLookup("charlie");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function phoneticLookup(val) {
  var result = "";

  var lookup = {
    alpha: "Adams",
    bravo: "Boston",
    charlie: "Chicago",
    delta: "Denver",
    echo: "Easy",
    foxtrot: "Frank"
  };

  result = lookup[val];

  return result;
}
```

</section>
<hr>

# 88. Testing Objects for Properties

## Description
<section id='description'>
Sometimes it is useful to check if the property of a given object exists or not. We can use the <code>.hasOwnProperty(propname)</code> method of objects to determine if that object has the given property name. <code>.hasOwnProperty()</code> returns <code>true</code> or <code>false</code> if the property is found or not.
<strong>Example</strong>
<blockquote>var myObj = {<br>&nbsp;&nbsp;top: "hat",<br>&nbsp;&nbsp;bottom: "pants"<br>};<br>myObj.hasOwnProperty("top");    // true<br>myObj.hasOwnProperty("middle"); // false</blockquote>
</section>

## Instructions
<section id='instructions'>
Modify the function <code>checkObj</code> to test <code>myObj</code> for <code>checkProp</code>. If the property is found, return that property's value. If not, return <code>"Not Found"</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var myObj = {
  gift: "pony",
  pet: "kitten",
  bed: "sleigh"
};

function checkObj(checkProp) {
  // Your Code Here

  return "Change Me!";
}

// Test your code by modifying these values
checkObj("gift");
```

</div>



</section>

## Solution
<section id='solution'>


```js
var myObj = {
  gift: "pony",
  pet: "kitten",
  bed: "sleigh"
};
function checkObj(checkProp) {
  if(myObj.hasOwnProperty(checkProp)) {
    return myObj[checkProp];
  } else {
    return "Not Found";
  }
}
```

</section>
<hr>

# 89. Manipulating Complex Objects

## Description
<section id='description'>
Sometimes you may want to store data in a flexible <dfn>Data Structure</dfn>. A JavaScript object is one way to handle flexible data. They allow for arbitrary combinations of <dfn>strings</dfn>, <dfn>numbers</dfn>, <dfn>booleans</dfn>, <dfn>arrays</dfn>, <dfn>functions</dfn>, and <dfn>objects</dfn>.
Here's an example of a complex data structure:
<blockquote>var ourMusic = [<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;"artist": "Daft Punk",<br>&nbsp;&nbsp;&nbsp;&nbsp;"title": "Homework",<br>&nbsp;&nbsp;&nbsp;&nbsp;"release_year": 1997,<br>&nbsp;&nbsp;&nbsp;&nbsp;"formats": [ <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"CD", <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Cassette", <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"LP"<br>&nbsp;&nbsp;&nbsp;&nbsp;],<br>&nbsp;&nbsp;&nbsp;&nbsp;"gold": true<br>&nbsp;&nbsp;}<br>];</blockquote>
This is an array which contains one object inside. The object has various pieces of <dfn>metadata</dfn> about an album. It also has a nested <code>"formats"</code> array. If you want to add more album records, you can do this by adding records to the top level array.
Objects hold data in a property, which has a key-value format. In the example above, <code>"artist": "Daft Punk"</code> is a property that has a key of <code>"artist"</code> and a value of <code>"Daft Punk"</code>.
<a href='http://www.json.org/' target=_blank>JavaScript Object Notation</a> or <code>JSON</code> is a related data interchange format used to store data.
<blockquote>{<br>&nbsp;&nbsp;"artist": "Daft Punk",<br>&nbsp;&nbsp;"title": "Homework",<br>&nbsp;&nbsp;"release_year": 1997,<br>&nbsp;&nbsp;"formats": [ <br>&nbsp;&nbsp;&nbsp;&nbsp;"CD",<br>&nbsp;&nbsp;&nbsp;&nbsp;"Cassette",<br>&nbsp;&nbsp;&nbsp;&nbsp;"LP"<br>&nbsp;&nbsp;],<br>&nbsp;&nbsp;"gold": true<br>}</blockquote>
<strong>Note</strong><br>You will need to place a comma after every object in the array, unless it is the last object in the array.
</section>

## Instructions
<section id='instructions'>
Add a new album to the <code>myMusic</code> array. Add <code>artist</code> and <code>title</code> strings, <code>release_year</code> number, and a <code>formats</code> array of strings.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var myMusic = [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  }
  // Add record here
];

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(x){ if (Array.isArray(x)) { return JSON.stringify(x); } return "myMusic is not an array"})(myMusic);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myMusic = [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [
      "CS",
      "8T",
      "LP" ],
    "gold": true
  },
  {
    "artist": "ABBA",
    "title": "Ring Ring",
    "release_year": 1973,
    "formats": [
      "CS",
      "8T",
      "LP",
    "CD",
  ]
  }
];
```

</section>
<hr>

# 90. Accessing Nested Objects

## Description
<section id='description'>
The sub-properties of objects can be accessed by chaining together the dot or bracket notation.
Here is a nested object:
<blockquote>var ourStorage = {<br>&nbsp;&nbsp;"desk": {<br>&nbsp;&nbsp;&nbsp;&nbsp;"drawer": "stapler"<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;"cabinet": {<br>&nbsp;&nbsp;&nbsp;&nbsp;"top drawer": { <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"folder1": "a file",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"folder2": "secrets"<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;"bottom drawer": "soda"<br>&nbsp;&nbsp;}<br>};<br>ourStorage.cabinet["top drawer"].folder2;  // "secrets"<br>ourStorage.desk.drawer; // "stapler"</blockquote>
</section>

## Instructions
<section id='instructions'>
Access the <code>myStorage</code> object and assign the contents of the <code>glove box</code> property to the <code>gloveBoxContents</code> variable. Use bracket notation for properties with a space in their name.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var myStorage = {
  "car": {
    "inside": {
      "glove box": "maps",
      "passenger seat": "crumbs"
     },
    "outside": {
      "trunk": "jack"
    }
  }
};

var gloveBoxContents = undefined; // Change this line

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(x) { 
  if(typeof x != 'undefined') { 
    return "gloveBoxContents = " + x;
  }
  return "gloveBoxContents is undefined";
})(gloveBoxContents);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myStorage = {
  "car":{
    "inside":{
      "glove box":"maps",
      "passenger seat":"crumbs"
    },
    "outside":{
      "trunk":"jack"
    }
  }
};
var gloveBoxContents = myStorage.car.inside["glove box"];
```

</section>
<hr>

# 91. Accessing Nested Arrays

## Description
<section id='description'>
As we have seen in earlier examples, objects can contain both nested objects and nested arrays. Similar to accessing nested objects, Array bracket notation can be chained to access nested arrays.
Here is an example of how to access a nested array:
<blockquote>var ourPets = [<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;animalType: "cat",<br>&nbsp;&nbsp;&nbsp;&nbsp;names: [<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Meowzer",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Fluffy",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Kit-Cat"<br>&nbsp;&nbsp;&nbsp;&nbsp;]<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;animalType: "dog",<br>&nbsp;&nbsp;&nbsp;&nbsp;names: [<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Spot",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Bowser",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Frankie"<br>&nbsp;&nbsp;&nbsp;&nbsp;]<br>&nbsp;&nbsp;}<br>];<br>ourPets[0].names[1]; // "Fluffy"<br>ourPets[1].names[0]; // "Spot"</blockquote>
</section>

## Instructions
<section id='instructions'>
Retrieve the second tree from the variable <code>myPlants</code> using object dot and array bracket notation.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var myPlants = [
  {
    type: "flowers",
    list: [
      "rose",
      "tulip",
      "dandelion"
    ]
  },
  {
    type: "trees",
    list: [
      "fir",
      "pine",
      "birch"
    ]
  }
];

// Only change code below this line

var secondTree = ""; // Change this line

```

</div>


### After Test
<div id='js-teardown'>

```js
(function(x) {
  if(typeof x != 'undefined') {
    return "secondTree = " + x;
  }
  return "secondTree is undefined";
})(secondTree);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myPlants = [
  {
    type: "flowers",
    list: [
      "rose",
      "tulip",
      "dandelion"
    ]
  },
  {
    type: "trees",
    list: [
      "fir",
      "pine",
      "birch"
    ]
  }
];

// Only change code below this line

var secondTree = myPlants[1].list[1];
```

</section>
<hr>

# 92. Record Collection

## Description
<section id='description'>
You are given a JSON object representing a part of your musical album collection. Each album has several properties and a unique id number as its key. Not all albums have complete information.
Write a function which takes an album's <code>id</code> (like <code>2548</code>), a property <code>prop</code> (like <code>"artist"</code> or <code>"tracks"</code>), and a <code>value</code> (like <code>"Addicted to Love"</code>) to modify the data in this collection.
If <code>prop</code> isn't <code>"tracks"</code> and <code>value</code> isn't empty (<code>""</code>), update or set the <code>value</code> for that record album's property.
Your function must always return the entire collection object.
There are several rules for handling incomplete data:
If <code>prop</code> is <code>"tracks"</code> but the album doesn't have a <code>"tracks"</code> property, create an empty array before adding the new value to the album's corresponding property.
If <code>prop</code> is <code>"tracks"</code> and <code>value</code> isn't empty (<code>""</code>), push the <code>value</code> onto the end of the album's existing <code>tracks</code> array.
If <code>value</code> is empty (<code>""</code>), delete the given <code>prop</code> property from the album.
<strong>Hints</strong><br>Use <code>bracket notation</code> when <a href="learn/javascript-algorithms-and-data-structures/basic-javascript/accessing-object-properties-with-variables" target="_blank">accessing object properties with variables</a>.
Push is an array method you can read about on <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push" target="_blank">Mozilla Developer Network</a>.
You may refer back to <a href="learn/javascript-algorithms-and-data-structures/basic-javascript/manipulating-complex-objects" target="_blank">Manipulating Complex Objects</a> Introducing JavaScript Object Notation (JSON) for a refresher.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var collection = {
    "2548": {
      "album": "Slippery When Wet",
      "artist": "Bon Jovi",
      "tracks": [
        "Let It Rock",
        "You Give Love a Bad Name"
      ]
    },
    "2468": {
      "album": "1999",
      "artist": "Prince",
      "tracks": [
        "1999",
        "Little Red Corvette"
      ]
    },
    "1245": {
      "artist": "Robert Palmer",
      "tracks": [ ]
    },
    "5439": {
      "album": "ABBA Gold"
    }
};
// Keep a copy of the collection for tests
var collectionCopy = JSON.parse(JSON.stringify(collection));

// Only change code below this line
function updateRecords(id, prop, value) {


  return collection;
}

// Alter values below to test your code
updateRecords(5439, "artist", "ABBA");

```

</div>


### After Test
<div id='js-teardown'>

```js
;(function(x) { return "collection = \n" + JSON.stringify(x, '\n', 2); })(collection);
```

</div>

</section>

## Solution
<section id='solution'>


```js
var collection = {
    2548: {
      album: "Slippery When Wet",
      artist: "Bon Jovi",
      tracks: [
        "Let It Rock",
        "You Give Love a Bad Name"
      ]
    },
    2468: {
      album: "1999",
      artist: "Prince",
      tracks: [
        "1999",
        "Little Red Corvette"
      ]
    },
    1245: {
      artist: "Robert Palmer",
      tracks: [ ]
    },
    5439: {
      album: "ABBA Gold"
    }
};
// Keep a copy of the collection for tests
var collectionCopy = JSON.parse(JSON.stringify(collection));

// Only change code below this line
function updateRecords(id, prop, value) {
  if(value === "") delete collection[id][prop];
  else if(prop === "tracks") {
    collection[id][prop] = collection[id][prop] || [];
    collection[id][prop].push(value);
  } else {
    collection[id][prop] = value;
  }

  return collection;
}
```

</section>
<hr>

# 93. Iterate with JavaScript While Loops

## Description
<section id='description'>
You can run the same code multiple times by using a loop.
The first type of loop we will learn is called a "<code>while</code>" loop because it runs "while" a specified condition is true and stops once that condition is no longer true.
<blockquote>var ourArray = [];<br>var i = 0;<br>while(i &#60; 5) {<br>&nbsp;&nbsp;ourArray.push(i);<br>&nbsp;&nbsp;i++;<br>}</blockquote>
Let's try getting a while loop to work by pushing values to an array.
</section>

## Instructions
<section id='instructions'>
Push the numbers 0 through 4 to <code>myArray</code> using a <code>while</code> loop.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var myArray = [];

// Only change code below this line.


```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof myArray !== "undefined"){(function(){return myArray;})();}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = [];
var i = 0;
while(i < 5) {
  myArray.push(i);
  i++;
}
```

</section>
<hr>

# 94. Iterate with JavaScript For Loops

## Description
<section id='description'>
You can run the same code multiple times by using a loop.
The most common type of JavaScript loop is called a "<code>for loop</code>" because it runs "for" a specific number of times.
For loops are declared with three optional expressions separated by semicolons:
<code>for ([initialization]; [condition]; [final-expression])</code>
The <code>initialization</code> statement is executed one time only before the loop starts. It is typically used to define and setup your loop variable.
The <code>condition</code> statement is evaluated at the beginning of every loop iteration and will continue as long as it evaluates to <code>true</code>. When <code>condition</code> is <code>false</code> at the start of the iteration, the loop will stop executing. This means if <code>condition</code> starts as <code>false</code>, your loop will never execute.
The <code>final-expression</code> is executed at the end of each loop iteration, prior to the next <code>condition</code> check and is usually used to increment or decrement your loop counter.
In the following example we initialize with <code>i = 0</code> and iterate while our condition <code>i &#60; 5</code> is true. We'll increment <code>i</code> by <code>1</code> in each loop iteration with <code>i++</code> as our <code>final-expression</code>.
<blockquote>var ourArray = [];<br>for (var i = 0; i &#60; 5; i++) {<br>&nbsp;&nbsp;ourArray.push(i);<br>}</blockquote>
<code>ourArray</code> will now contain <code>[0,1,2,3,4]</code>.
</section>

## Instructions
<section id='instructions'>
Use a <code>for</code> loop to work to push the values 1 through 5 onto <code>myArray</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = [];

for (var i = 0; i < 5; i++) {
  ourArray.push(i);
}

// Setup
var myArray = [];

// Only change code below this line.


```

</div>


### After Test
<div id='js-teardown'>

```js
if (typeof myArray !== "undefined"){(function(){return myArray;})();}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var ourArray = [];
for (var i = 0; i < 5; i++) {
  ourArray.push(i);
}
var myArray = [];
for (var i = 1; i < 6; i++) {
  myArray.push(i);
}
```

</section>
<hr>

# 95. Iterate Odd Numbers With a For Loop

## Description
<section id='description'>
For loops don't have to iterate one at a time. By changing our <code>final-expression</code>, we can count by even numbers.
We'll start at <code>i = 0</code> and loop while <code>i &#60; 10</code>. We'll increment <code>i</code> by 2 each loop with <code>i += 2</code>.
<blockquote>var ourArray = [];<br>for (var i = 0; i &#60; 10; i += 2) {<br>&nbsp;&nbsp;ourArray.push(i);<br>}</blockquote>
<code>ourArray</code> will now contain <code>[0,2,4,6,8]</code>.
Let's change our <code>initialization</code> so we can count by odd numbers.
</section>

## Instructions
<section id='instructions'>
Push the odd numbers from 1 through 9 to <code>myArray</code> using a <code>for</code> loop.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = [];

for (var i = 0; i < 10; i += 2) {
  ourArray.push(i);
}

// Setup
var myArray = [];

// Only change code below this line.


```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof myArray !== "undefined"){(function(){return myArray;})();}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var ourArray = [];
for (var i = 0; i < 10; i += 2) {
  ourArray.push(i);
}
var myArray = [];
for (var i = 1; i < 10; i += 2) {
  myArray.push(i);
}
```

</section>
<hr>

# 96. Count Backwards With a For Loop

## Description
<section id='description'>
A for loop can also count backwards, so long as we can define the right conditions.
In order to count backwards by twos, we'll need to change our <code>initialization</code>, <code>condition</code>, and <code>final-expression</code>.
We'll start at <code>i = 10</code> and loop while <code>i &#62; 0</code>. We'll decrement <code>i</code> by 2 each loop with <code>i -= 2</code>.
<blockquote>var ourArray = [];<br>for (var i=10; i &#62; 0; i-=2) {<br>&nbsp;&nbsp;ourArray.push(i);<br>}</blockquote>
<code>ourArray</code> will now contain <code>[10,8,6,4,2]</code>.
Let's change our <code>initialization</code> and <code>final-expression</code> so we can count backward by twos by odd numbers.
</section>

## Instructions
<section id='instructions'>
Push the odd numbers from 9 through 1 to <code>myArray</code> using a <code>for</code> loop.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArray = [];

for (var i = 10; i > 0; i -= 2) {
  ourArray.push(i);
}

// Setup
var myArray = [];

// Only change code below this line.


```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof myArray !== "undefined"){(function(){return myArray;})();}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var ourArray = [];
for (var i = 10; i > 0; i -= 2) {
  ourArray.push(i);
}
var myArray = [];
for (var i = 9; i > 0; i -= 2) {
  myArray.push(i);
}
```

</section>
<hr>

# 97. Iterate Through an Array with a For Loop

## Description
<section id='description'>
A common task in JavaScript is to iterate through the contents of an array. One way to do that is with a <code>for</code> loop. This code will output each element of the array <code>arr</code> to the console:
<blockquote>var arr = [10,9,8,7,6];<br>for (var i = 0; i < arr.length; i++) {<br>&nbsp;&nbsp; console.log(arr[i]);<br>}</blockquote>
Remember that Arrays have zero-based numbering, which means the last index of the array is length - 1. Our <dfn>condition</dfn> for this loop is <code>i < arr.length</code>, which stops when <code>i</code> is at length - 1.
</section>

## Instructions
<section id='instructions'>
Declare and initialize a variable <code>total</code> to <code>0</code>. Use a <code>for</code> loop to add the value of each element of the <code>myArr</code> array to <code>total</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
var ourArr = [ 9, 10, 11, 12];
var ourTotal = 0;

for (var i = 0; i < ourArr.length; i++) {
  ourTotal += ourArr[i];
}

// Setup
var myArr = [ 2, 3, 4, 5, 6];

// Only change code below this line


```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){if(typeof total !== 'undefined') { return "total = " + total; } else { return "total is undefined";}})()

```

</div>

</section>

## Solution
<section id='solution'>


```js
var ourArr = [ 9, 10, 11, 12];
var ourTotal = 0;

for (var i = 0; i < ourArr.length; i++) {
  ourTotal += ourArr[i];
}

var myArr = [ 2, 3, 4, 5, 6];
var total = 0;

for (var i = 0; i < myArr.length; i++) {
  total += myArr[i];
}
```

</section>
<hr>

# 98. Nesting For Loops

## Description
<section id='description'>
If you have a multi-dimensional array, you can use the same logic as the prior waypoint to loop through both the array and any sub-arrays. Here is an example:
<blockquote>var arr = [<br>&nbsp;&nbsp;[1,2], [3,4], [5,6]<br>];<br>for (var i=0; i &lt; arr.length; i++) {<br>&nbsp;&nbsp;for (var j=0; j &lt; arr[i].length; j++) {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log(arr[i][j]);<br>&nbsp;&nbsp;}<br>}</blockquote>
This outputs each sub-element in <code>arr</code> one at a time. Note that for the inner loop, we are checking the <code>.length</code> of <code>arr[i]</code>, since <code>arr[i]</code> is itself an array.
</section>

## Instructions
<section id='instructions'>
Modify function <code>multiplyAll</code> so that it multiplies the <code>product</code> variable by each number in the sub-arrays of <code>arr</code>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function multiplyAll(arr) {
  var product = 1;
  // Only change code below this line

  // Only change code above this line
  return product;
}

// Modify values below to test your code
multiplyAll([[1,2],[3,4],[5,6,7]]);

```

</div>



</section>

## Solution
<section id='solution'>


```js
function multiplyAll(arr) {
  var product = 1;
  for (var i = 0; i < arr.length; i++) {
    for (var j = 0; j < arr[i].length; j++) {
      product *= arr[i][j];
    }
  }
  return product;
}

multiplyAll([[1,2],[3,4],[5,6,7]]);
```

</section>
<hr>

# 99. Iterate with JavaScript Do...While Loops

## Description
<section id='description'>
You can run the same code multiple times by using a loop.
The next type of loop you will learn is called a "<code>do...while</code>" loop because it first will "<code>do</code>" one pass of the code inside the loop no matter what, and then it runs "<code>while</code>" a specified condition is true and stops once that condition is no longer true. Let's look at an example.
<blockquote>var ourArray = [];<br>var i = 0;<br>do {<br>&nbsp;&nbsp;ourArray.push(i);<br>&nbsp;&nbsp;i++;<br>} while (i < 5);</blockquote>
This behaves just as you would expect with any other type of loop, and the resulting array will look like <code>[0, 1, 2, 3, 4]</code>. However, what makes the <code>do...while</code> different from other loops is how it behaves when the condition fails on the first check. Let's see this in action.
Here is a regular while loop that will run the code in the loop as long as <code>i < 5</code>.
<blockquote>var ourArray = []; <br>var i = 5;<br>while (i < 5) {<br>&nbsp;&nbsp;ourArray.push(i);<br>&nbsp;&nbsp;i++;<br>}</blockquote>
Notice that we initialize the value of <code>i</code> to be 5. When we execute the next line, we notice that <code>i</code> is not less than 5. So we do not execute the code inside the loop. The result is that <code>ourArray</code> will end up with nothing added to it, so it will still look like this <code>[]</code> when all the code in the example above finishes running.
Now, take a look at a <code>do...while</code> loop.
<blockquote>var ourArray = []; <br>var i = 5;<br>do {<br>&nbsp;&nbsp;ourArray.push(i);<br>&nbsp;&nbsp;i++;<br>} while (i < 5);</blockquote>
In this case, we initialize the value of <code>i</code> as 5, just like we did with the while loop. When we get to the next line, there is no check for the value of <code>i</code>, so we go to the code inside the curly braces and execute it. We will add one element to the array and increment <code>i</code> before we get to the condition check. Then, when we get to checking if <code>i < 5</code> see that <code>i</code> is now 6, which fails the conditional check. So we exit the loop and are done. At the end of the above example, the value of <code>ourArray</code> is <code>[5]</code>.
Essentially, a <code>do...while</code> loop ensures that the code inside the loop will run at least once.
Let's try getting a <code>do...while</code> loop to work by pushing values to an array.
</section>

## Instructions
<section id='instructions'>
Change the <code>while</code> loop in the code to a <code>do...while</code> loop so that the loop will only push the number 10 to <code>myArray</code>, and <code>i</code> will be equal to <code>11</code> when your code finishes running.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Setup
var myArray = [];
var i = 10;

// Only change code below this line.

while (i < 5) {
  myArray.push(i);
  i++;
}

```

</div>


### After Test
<div id='js-teardown'>

```js
if(typeof myArray !== "undefined"){(function(){return myArray;})();}
```

</div>

</section>

## Solution
<section id='solution'>


```js
var myArray = [];
var i = 10;
do {
  myArray.push(i);
  i++;
} while (i < 5)
```

</section>
<hr>

# 100. Profile Lookup

## Description
<section id='description'>
We have an array of objects representing different people in our contacts lists.
A <code>lookUpProfile</code> function that takes <code>name</code> and a property (<code>prop</code>) as arguments has been pre-written for you.
The function should check if <code>name</code> is an actual contact's <code>firstName</code> and the given property (<code>prop</code>) is a property of that contact.
If both are true, then return the "value" of that property.
If <code>name</code> does not correspond to any contacts then return <code>"No such contact"</code>
If <code>prop</code> does not correspond to any valid properties of a contact found to match <code>name</code> then return <code>"No such property"</code>
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
//Setup
var contacts = [
    {
        "firstName": "Akira",
        "lastName": "Laine",
        "number": "0543236543",
        "likes": ["Pizza", "Coding", "Brownie Points"]
    },
    {
        "firstName": "Harry",
        "lastName": "Potter",
        "number": "0994372684",
        "likes": ["Hogwarts", "Magic", "Hagrid"]
    },
    {
        "firstName": "Sherlock",
        "lastName": "Holmes",
        "number": "0487345643",
        "likes": ["Intriguing Cases", "Violin"]
    },
    {
        "firstName": "Kristian",
        "lastName": "Vos",
        "number": "unknown",
        "likes": ["JavaScript", "Gaming", "Foxes"]
    }
];


function lookUpProfile(name, prop){
// Only change code below this line

// Only change code above this line
}

// Change these values to test your function
lookUpProfile("Akira", "likes");
```

</div>



</section>

## Solution
<section id='solution'>


```js
var contacts = [
    {
        "firstName": "Akira",
        "lastName": "Laine",
        "number": "0543236543",
        "likes": ["Pizza", "Coding", "Brownie Points"]
    },
    {
        "firstName": "Harry",
        "lastName": "Potter",
        "number": "0994372684",
        "likes": ["Hogwarts", "Magic", "Hagrid"]
    },
    {
        "firstName": "Sherlock",
        "lastName": "Holmes",
        "number": "0487345643",
        "likes": ["Intriguing Cases", "Violin"]
    },
    {
        "firstName": "Kristian",
        "lastName": "Vos",
        "number": "unknown",
        "likes": ["JavaScript", "Gaming", "Foxes"]
    },
];


//Write your function in between these comments
function lookUpProfile(name, prop){
    for(var i in contacts){
      if(contacts[i].firstName === name) {
        return contacts[i][prop] || "No such property";
      }
    }
   return "No such contact";
}
//Write your function in between these comments

lookUpProfile("Akira", "likes");
```

</section>
<hr>

# 101. Generate Random Fractions with JavaScript

## Description
<section id='description'>
Random numbers are useful for creating random behavior.
JavaScript has a <code>Math.random()</code> function that generates a random decimal number between <code>0</code> (inclusive) and not quite up to <code>1</code> (exclusive). Thus <code>Math.random()</code> can return a <code>0</code> but never quite return a <code>1</code>
<strong>Note</strong><br>Like <a href='learn/javascript-algorithms-and-data-structures/basic-javascript/storing-values-with-the-assignment-operator' target='_blank'>Storing Values with the Equal Operator</a>, all function calls will be resolved before the <code>return</code> executes, so we can <code>return</code> the value of the <code>Math.random()</code> function.
</section>

## Instructions
<section id='instructions'>
Change <code>randomFraction</code> to return a random number instead of returning <code>0</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function randomFraction() {

  // Only change code below this line.

  return 0;

  // Only change code above this line.
}
```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){return randomFraction();})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
function randomFraction() {
  return Math.random();
}
```

</section>
<hr>

# 102. Generate Random Whole Numbers with JavaScript

## Description
<section id='description'>
It's great that we can generate random decimal numbers, but it's even more useful if we use it to generate random whole numbers.
<ol><li>Use <code>Math.random()</code> to generate a random decimal.</li><li>Multiply that random decimal by <code>20</code>.</li><li>Use another function, <code>Math.floor()</code> to round the number down to its nearest whole number.</li></ol>
Remember that <code>Math.random()</code> can never quite return a <code>1</code> and, because we're rounding down, it's impossible to actually get <code>20</code>. This technique will give us a whole number between <code>0</code> and <code>19</code>.
Putting everything together, this is what our code looks like:
<code>Math.floor(Math.random() * 20);</code>
We are calling <code>Math.random()</code>, multiplying the result by 20, then passing the value to <code>Math.floor()</code> function to round the value down to the nearest whole number.
</section>

## Instructions
<section id='instructions'>
Use this technique to generate and return a random whole number between <code>0</code> and <code>9</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var randomNumberBetween0and19 = Math.floor(Math.random() * 20);

function randomWholeNum() {

  // Only change code below this line.

  return Math.random();
}
```

</div>


### After Test
<div id='js-teardown'>

```js
(function(){return randomWholeNum();})();
```

</div>

</section>

## Solution
<section id='solution'>


```js
var randomNumberBetween0and19 = Math.floor(Math.random() * 20);
function randomWholeNum() {
  return Math.floor(Math.random() * 10);
}
```

</section>
<hr>

# 103. Generate Random Whole Numbers within a Range

## Description
<section id='description'>
Instead of generating a random number between zero and a given number like we did before, we can generate a random number that falls within a range of two specific numbers.
To do this, we'll define a minimum number <code>min</code> and a maximum number <code>max</code>.
Here's the formula we'll use. Take a moment to read it and try to understand what this code is doing:
<code>Math.floor(Math.random() * (max - min + 1)) + min</code>
</section>

## Instructions
<section id='instructions'>
Create a function called <code>randomRange</code> that takes a range <code>myMin</code> and <code>myMax</code> and returns a random number that's greater than or equal to <code>myMin</code>, and is less than or equal to <code>myMax</code>, inclusive.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Example
function ourRandomRange(ourMin, ourMax) {

  return Math.floor(Math.random() * (ourMax - ourMin + 1)) + ourMin;
}

ourRandomRange(1, 9);

// Only change code below this line.

function randomRange(myMin, myMax) {

  return 0; // Change this line

}

// Change these values to test your function
var myRandom = randomRange(5, 15);
```

</div>


### After Test
<div id='js-teardown'>

```js
var calcMin = 100;
var calcMax = -100;
for(var i = 0; i < 100; i++) {
  var result = randomRange(5,15);
  calcMin = Math.min(calcMin, result);
  calcMax = Math.max(calcMax, result);
}
(function(){
  if(typeof myRandom === 'number') {
    return "myRandom = " + myRandom;
  } else {
    return "myRandom undefined";
  }
})()
```

</div>

</section>

## Solution
<section id='solution'>


```js
function randomRange(myMin, myMax) {
  return Math.floor(Math.random() * (myMax - myMin + 1)) + myMin;
}
```

</section>
<hr>

# 104. Use the parseInt Function

## Description
<section id='description'>
The <code>parseInt()</code> function parses a string and returns an integer. Here's an example:
<code>var a = parseInt("007");</code>
The above function converts the string "007" to an integer 7. If the first character in the string can't be converted into a number, then it returns <code>NaN</code>.
</section>

## Instructions
<section id='instructions'>
Use <code>parseInt()</code> in the <code>convertToInteger</code> function so it converts the input string <code>str</code> into an integer, and returns it.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function convertToInteger(str) {

}

convertToInteger("56");
```

</div>



</section>

## Solution
<section id='solution'>

```js
function convertToInteger(str) {
  return parseInt(str);
}
```
</section>
<hr>

# 105. Use the parseInt Function with a Radix

## Description
<section id='description'>
The <code>parseInt()</code> function parses a string and returns an integer. It takes a second argument for the radix, which specifies the base of the number in the string. The radix can be an integer between 2 and 36.
The function call looks like:
<code>parseInt(string, radix);</code>
And here's an example:
<code>var a = parseInt("11", 2);</code>
The radix variable says that "11" is in the binary system, or base 2. This example converts the string "11" to an integer 3.
</section>

## Instructions
<section id='instructions'>
Use <code>parseInt()</code> in the <code>convertToInteger</code> function so it converts a binary number to an integer and returns it.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function convertToInteger(str) {

}

convertToInteger("10011");
```

</div>



</section>

## Solution
<section id='solution'>

```js
function convertToInteger(str) {
  return parseInt(str, 2);
}
```
</section>
<hr>

# 106. Use the Conditional (Ternary) Operator

## Description
<section id='description'>
The <dfn>conditional operator</dfn>, also called the <dfn>ternary operator</dfn>, can be used as a one line if-else expression.
The syntax is:
<code>condition ? statement-if-true : statement-if-false;</code>
The following function uses an if-else statement to check a condition:
<blockquote>function findGreater(a, b) {<br>&nbsp;&nbsp;if(a > b) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "a is greater";<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;else {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "b is greater";<br>&nbsp;&nbsp;}<br>}</blockquote>
This can be re-written using the <code>conditional operator</code>:
<blockquote>function findGreater(a, b) {<br>&nbsp;&nbsp;return a > b ? "a is greater" : "b is greater";<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Use the <code>conditional operator</code> in the <code>checkEqual</code> function to check if two numbers are equal or not. The function should return either "Equal" or "Not Equal".
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function checkEqual(a, b) {

}

checkEqual(1, 2);
```

</div>



</section>

## Solution
<section id='solution'>

```js
function checkEqual(a, b) {
  return a === b ? "Equal" : "Not Equal";
}
```
</section>
<hr>

# 107. Use Multiple Conditional (Ternary) Operators

## Description
<section id='description'>
In the previous challenge, you used a single <code>conditional operator</code>. You can also chain them together to check for multiple conditions.
The following function uses if, else if, and else statements to check multiple conditions:
<blockquote>function findGreaterOrEqual(a, b) {<br>&nbsp;&nbsp;if(a === b) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "a and b are equal";<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;else if(a > b) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "a is greater";<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;else {<br>&nbsp;&nbsp;&nbsp;&nbsp;return "b is greater";<br>&nbsp;&nbsp;}<br>}</blockquote>
The above function can be re-written using multiple <code>conditional operators</code>:
<blockquote>function findGreaterOrEqual(a, b) {<br>&nbsp;&nbsp;return (a === b) ? "a and b are equal" : (a > b) ? "a is greater" : "b is greater";<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Use multiple <code>conditional operators</code> in the <code>checkSign</code> function to check if a number is positive, negative or zero.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function checkSign(num) {

}

checkSign(10);
```

</div>



</section>

## Solution
<section id='solution'>

```js
function checkSign(num) {
  return (num > 0) ? 'positive' : (num < 0) ? 'negative' : 'zero';
}
```
</section>
<hr>

