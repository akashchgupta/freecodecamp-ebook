
# Basic JavaScript
# 1. Comment Your JavaScript Code

## Description
<section id='description'>
Comments are lines of code that JavaScript will intentionally ignore. Comments are a great way to leave notes to yourself and to other people who will later need to figure out what that code does.
There are two ways to write comments in JavaScript:
Using <code>//</code> will tell JavaScript to ignore the remainder of the text on the current line:
<blockquote>// This is an in-line comment.</blockquote>
You can make a multi-line comment beginning with <code>/*</code> and ending with <code>*/</code>:
<blockquote>/*This is a<br>multi-line comment */</blockquote>
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
/*Another Comment */
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
<blockquote>myVar = 13 *13; // assigned 169</blockquote>

</section>

## Instructions
<section id='instructions'>
Change the <code>0</code> so that product will equal <code>80</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var product = 8 *0;


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
var product = 8 *10;
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
var product = 2.0 *0.0;


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
var product = 2.0 *2.5;
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
<blockquote>5 % 2 = 1 because<br>Math.floor(5 / 2) = 2 (Quotient)<br>2 *2 = 4<br>5 - 4 = 1 (Remainder)</blockquote>
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
<code>myVar = myVar *5;</code>
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

a = a *5;
b = 3 *b;
c = c *10;


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
  return num *5;
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
<code>Math.floor(Math.random() *20);</code>
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
var randomNumberBetween0and19 = Math.floor(Math.random() *20);

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
var randomNumberBetween0and19 = Math.floor(Math.random() *20);
function randomWholeNum() {
  return Math.floor(Math.random() *10);
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
<code>Math.floor(Math.random() *(max - min + 1)) + min</code>
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

  return Math.floor(Math.random() *(ourMax - ourMin + 1)) + ourMin;
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
  return Math.floor(Math.random() *(myMax - myMin + 1)) + myMin;
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

# ES6
# 1. Explore Differences Between the var and let Keywords

## Description
<section id='description'>
One of the biggest problems with declaring variables with the <code>var</code> keyword is that you can overwrite variable declarations without an error.
<blockquote>var camper = 'James';<br>var camper = 'David';<br>console.log(camper);<br>// logs 'David'</blockquote>
As you can see in the code above, the <code>camper</code> variable is originally declared as <code>James</code> and then overridden to be <code>David</code>.
In a small application, you might not run into this type of problem, but when your code becomes larger, you might accidentally overwrite a variable that you did not intend to overwrite.
Because this behavior does not throw an error, searching and fixing bugs becomes more difficult.<br>
A new keyword called <code>let</code> was introduced in ES6 to solve this potential issue with the <code>var</code> keyword.
If you were to replace <code>var</code> with <code>let</code> in the variable declarations of the code above, the result would be an error.
<blockquote>let camper = 'James';<br>let camper = 'David'; // throws an error</blockquote>
This error can be seen in the console of your browser.
So unlike <code>var</code>, when using <code>let</code>, a variable with the same name can only be declared once.
Note the <code>"use strict"</code>. This enables Strict Mode, which catches common coding mistakes and "unsafe" actions. For instance:
<blockquote>"use strict";<br>x = 3.14; // throws an error because x is not declared</blockquote>
</section>

## Instructions
<section id='instructions'>
Update the code so it only uses the <code>let</code> keyword.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var catName;
var quote;
function catTalk() {
  "use strict";

  catName = "Oliver";
  quote = catName + " says Meow!";

}
catTalk();
```

</div>



</section>

## Solution
<section id='solution'>

```js
let catName;
let quote;
function catTalk() {
  'use strict';

  catName = 'Oliver';
  quote = catName + ' says Meow!';
}
catTalk();
```
</section>
<hr>

# 2. Compare Scopes of the var and let Keywords

## Description
<section id='description'>
When you declare a variable with the <code>var</code> keyword, it is declared globally, or locally if declared inside a function.
The <code>let</code> keyword behaves similarly, but with some extra features. When you declare a variable with the <code>let</code> keyword inside a block, statement, or expression, its scope is limited to that block, statement, or expression.
For example:
<blockquote>var numArray = [];<br>for (var i = 0; i < 3; i++) {<br>&nbsp;&nbsp;numArray.push(i);<br>}<br>console.log(numArray);<br>// returns [0, 1, 2]<br>console.log(i);<br>// returns 3</blockquote>
With the <code>var</code> keyword, <code>i</code> is declared globally. So when <code>i++</code> is executed, it updates the global variable. This code is similar to the following:
<blockquote>var numArray = [];<br>var i;<br>for (i = 0; i < 3; i++) {<br>&nbsp;&nbsp;numArray.push(i);<br>}<br>console.log(numArray);<br>// returns [0, 1, 2]<br>console.log(i);<br>// returns 3</blockquote>
This behavior will cause problems if you were to create a function and store it for later use inside a for loop that uses the <code>i</code> variable. This is because the stored function will always refer to the value of the updated global <code>i</code> variable.
<blockquote>var printNumTwo;<br>for (var i = 0; i < 3; i++) {<br>&nbsp;&nbsp;if(i === 2){<br>&nbsp;&nbsp;&nbsp;&nbsp;printNumTwo = function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return i;<br>&nbsp;&nbsp;&nbsp;&nbsp;};<br>&nbsp;&nbsp;}<br>}<br>console.log(printNumTwo());<br>// returns 3</blockquote>
As you can see, <code>printNumTwo()</code> prints 3 and not 2. This is because the value assigned to <code>i</code> was updated and the <code>printNumTwo()</code> returns the global <code>i</code> and not the value <code>i</code> had when the function was created in the for loop. The <code>let</code> keyword does not follow this behavior:
<blockquote>'use strict';<br>let printNumTwo;<br>for (let i = 0; i < 3; i++) {<br>&nbsp;&nbsp;if (i === 2) {<br>&nbsp;&nbsp;&nbsp;&nbsp;printNumTwo = function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;return i;<br>&nbsp;&nbsp;&nbsp;&nbsp;};<br>&nbsp;&nbsp;}<br>}<br>console.log(printNumTwo());<br>// returns 2<br>console.log(i);<br>// returns "i is not defined"</blockquote>
<code>i</code> is not defined because it was not declared in the global scope. It is only declared within the for loop statement. <code>printNumTwo()</code> returned the correct value because three different <code>i</code> variables with unique values (0, 1, and 2) were created by the <code>let</code> keyword within the loop statement.
</section>

## Instructions
<section id='instructions'>
Fix the code so that <code>i</code> declared in the if statement is a separate variable than <code>i</code> declared in the first line of the function. Be certain not to use the <code>var</code> keyword anywhere in your code.
This exercise is designed to illustrate the difference between how <code>var</code> and <code>let</code> keywords assign scope to the declared variable. When programming a function similar to the one used in this exercise, it is often better to use different variable names to avoid confusion.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function checkScope() {
  'use strict';
  var i = 'function scope';
  if (true) {
    i = 'block scope';
    console.log('Block scope i is: ', i);
  }
  console.log('Function scope i is: ', i);
  return i;
}
```

</div>



</section>

## Solution
<section id='solution'>

```js
function checkScope() {
  'use strict';
  let i = 'function scope';
  if (true) {
    let i = 'block scope';
    console.log('Block scope i is: ', i);
  }
 
  console.log('Function scope i is: ', i);
  return i;
}
```
</section>
<hr>

# 3. Declare a Read-Only Variable with the const Keyword

## Description
<section id='description'>
The keyword <code>let</code> is not the only new way to declare variables. In ES6, you can also declare variables using the <code>const</code> keyword.
<code>const</code> has all the awesome features that <code>let</code> has, with the added bonus that variables declared using <code>const</code> are read-only. They are a constant value, which means that once a variable is assigned with <code>const</code>, it cannot be reassigned.
<blockquote>"use strict"<br>const FAV_PET = "Cats";<br>FAV_PET = "Dogs"; // returns error</blockquote>
As you can see, trying to reassign a variable declared with <code>const</code> will throw an error. You should always name variables you don't want to reassign using the <code>const</code> keyword. This helps when you accidentally attempt to reassign a variable that is meant to stay constant. A common practice when naming constants is to use all uppercase letters, with words separated by an underscore.
  
  <strong>Note:</strong> It is common for developers to use uppercase variable identifiers for immutable values and lowercase or camelCase for mutable values (objects and arrays). In a later challenge you will see an example of a lowercase variable identifier being used for an array.
</section>

## Instructions
<section id='instructions'>
Change the code so that all variables are declared using <code>let</code> or <code>const</code>. Use <code>let</code> when you want the variable to change, and <code>const</code> when you want the variable to remain constant. Also, rename variables declared with <code>const</code> to conform to common practices, meaning constants should be in all caps.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function printManyTimes(str) {
  "use strict";

  // change code below this line

  var sentence = str + " is cool!";
  for(var i = 0; i < str.length; i+=2) {
    console.log(sentence);
  }

  // change code above this line

}
printManyTimes("freeCodeCamp");
```

</div>



</section>

## Solution
<section id='solution'>

```js
function printManyTimes(str) {
  "use strict";

  // change code below this line

  const SENTENCE = str + " is cool!";
  for(let i = 0; i < str.length; i+=2) {
    console.log(SENTENCE);
  }

  // change code above this line

}
printManyTimes("freeCodeCamp");
```
</section>
<hr>

# 4. Mutate an Array Declared with const

## Description
<section id='description'>
The <code>const</code> declaration has many use cases in modern JavaScript.
Some developers prefer to assign all their variables using <code>const</code> by default, unless they know they will need to reassign the value. Only in that case, they use <code>let</code>.
However, it is important to understand that objects (including arrays and functions) assigned to a variable using <code>const</code> are still mutable. Using the <code>const</code> declaration only prevents reassignment of the variable identifier.
<blockquote>"use strict";<br>const s = [5, 6, 7];<br>s = [1, 2, 3]; // throws error, trying to assign a const<br>s[2] = 45; // works just as it would with an array declared with var or let<br>console.log(s); // returns [5, 6, 45]</blockquote>
As you can see, you can mutate the object <code>[5, 6, 7]</code> itself and the variable <code>s</code> will still point to the altered array <code>[5, 6, 45]</code>. Like all arrays, the array elements in <code>s</code> are mutable, but because <code>const</code> was used, you cannot use the variable identifier <code>s</code> to point to a different array using the assignment operator.
</section>

## Instructions
<section id='instructions'>
An array is declared as <code>const s = [5, 7, 2]</code>. Change the array to <code>[2, 5, 7]</code> using various element assignment.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const s = [5, 7, 2];
function editInPlace() {
  'use strict';
  // change code below this line

  // s = [2, 5, 7]; <- this is invalid

  // change code above this line
}
editInPlace();
```

</div>



</section>

## Solution
<section id='solution'>

```js
const s = [5, 7, 2];
function editInPlace() {
  'use strict';
  // change code below this line

  // s = [2, 5, 7]; <- this is invalid
  s[0] = 2;
  s[1] = 5;
  s[2] = 7;
  // change code above this line
}
editInPlace();
```
</section>
<hr>

# 5. Prevent Object Mutation

## Description
<section id='description'>
As seen in the previous challenge, <code>const</code> declaration alone doesn't really protect your data from mutation. To ensure your data doesn't change, JavaScript provides a function <code>Object.freeze</code> to prevent data mutation.
Once the object is frozen, you can no longer add, update, or delete properties from it. Any attempt at changing the object will be rejected without an error.
<blockquote>let obj = {<br>&nbsp;&nbsp;name:"FreeCodeCamp",<br>&nbsp;&nbsp;review:"Awesome"<br>};<br>Object.freeze(obj);<br>obj.review = "bad"; //will be ignored. Mutation not allowed<br>obj.newProp = "Test"; // will be ignored. Mutation not allowed<br>console.log(obj); <br>// { name: "FreeCodeCamp", review:"Awesome"}</blockquote>
</section>

## Instructions
<section id='instructions'>
In this challenge you are going to use <code>Object.freeze</code> to prevent mathematical constants from changing. You need to freeze the <code>MATH_CONSTANTS</code> object so that no one is able to alter the value of <code>PI</code>, add, or delete properties.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function freezeObj() {
  'use strict';
  const MATH_CONSTANTS = {
    PI: 3.14
  };
  // change code below this line


  // change code above this line
  try {
    MATH_CONSTANTS.PI = 99;
  } catch( ex ) {
    console.log(ex);
  }
  return MATH_CONSTANTS.PI;
}
const PI = freezeObj();
```

</div>



</section>

## Solution
<section id='solution'>

```js
function freezeObj() {
  'use strict';
  const MATH_CONSTANTS = {
    PI: 3.14
  };
  // change code below this line
  Object.freeze(MATH_CONSTANTS);

  // change code above this line
  try {
    MATH_CONSTANTS.PI = 99;
  } catch( ex ) {
    console.log(ex);
  }
  return MATH_CONSTANTS.PI;
}
const PI = freezeObj();
```
</section>
<hr>

# 6. Use Arrow Functions to Write Concise Anonymous Functions

## Description
<section id='description'>
In JavaScript, we often don't need to name our functions, especially when passing a function as an argument to another function. Instead, we create inline functions. We don't need to name these functions because we do not reuse them anywhere else.
To achieve this, we often use the following syntax:
<blockquote>const myFunc = function() {<br>&nbsp;&nbsp;const myVar = "value";<br>&nbsp;&nbsp;return myVar;<br>}</blockquote>
ES6 provides us with the syntactic sugar to not have to write anonymous functions this way. Instead, you can use <strong>arrow function syntax</strong>:
<blockquote>const myFunc = () => {<br>&nbsp;&nbsp;const myVar = "value";<br>&nbsp;&nbsp;return myVar;<br>}</blockquote>
When there is no function body, and only a return value, arrow function syntax allows you to omit the keyword <code>return</code> as well as the brackets surrounding the code. This helps simplify smaller functions into one-line statements:
<blockquote>const myFunc = () => "value"</blockquote>
This code will still return <code>value</code> by default.
</section>

## Instructions
<section id='instructions'>
Rewrite the function assigned to the variable <code>magic</code> which returns a new <code>Date()</code> to use arrow function syntax. Also make sure nothing is defined using the keyword <code>var</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var magic = function() {
  "use strict";
  return new Date();
};
```

</div>



</section>

## Solution
<section id='solution'>

```js
const magic = () => {
  "use strict";
  return new Date();
};
```
</section>
<hr>

# 7. Write Arrow Functions with Parameters

## Description
<section id='description'>
Just like a regular function, you can pass arguments into an arrow function.
<blockquote>// doubles input value and returns it<br>const doubler = (item) => item *2;</blockquote>
If an arrow function has a single argument, the parentheses enclosing the argument may be omitted.
<blockquote>// the same function, without the argument parentheses<br>const doubler = item => item *2;</blockquote>
It is possible to pass more than one argument into an arrow function.
<blockquote>// multiplies the first input value by the second and returns it<br>const multiplier = (item, multi) => item *multi;</blockquote>
</section>

## Instructions
<section id='instructions'>
Rewrite the <code>myConcat</code> function which appends contents of <code>arr2</code> to <code>arr1</code> so that the function uses arrow function syntax.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var myConcat = function(arr1, arr2) {
  "use strict";
  return arr1.concat(arr2);
};
// test your code
console.log(myConcat([1, 2], [3, 4, 5]));
```

</div>



</section>

## Solution
<section id='solution'>

```js
const myConcat = (arr1, arr2) =>  {
  "use strict";
  return arr1.concat(arr2);
};
// test your code
console.log(myConcat([1, 2], [3, 4, 5]));
```
</section>
<hr>

# 8. Write Higher Order Arrow Functions

## Description
<section id='description'>
It's time to look at higher-order functions and their common pair, arrow functions.
Arrow functions work really well when combined with higher-order functions, such as <code>map()</code>, <code>filter()</code>, and <code>reduce()</code>. <br>
But what are these functions? Lets look at the simplest example <code>forEach()</code>, and run it on the following array of sample Facebook posts.
<blockquote>let FBPosts = [<br>
    {thumbnail: "someIcon", likes:432, shares: 600},<br>
    {thumbnail: "Another icon", likes:300, shares: 501},<br>
    {thumbnail: "Yet another", likes:40, shares: 550},<br>
    {thumbnail: null, likes: 101, shares:0},<br>
]</br>
</blockquote>
Of the two <code>forEach()</code> versions below, both perform the exact same log function, and each takes an anonymous callback with a parameter <code>post</code>. The difference is the syntax. One uses an arrow function and the other does not.  
<blockquote>
<strong>ES5</strong><br>
FBpost.forEach(function(post) {<br>
    console.log(post) // log each post here<br>
    });<br>
<strong>ES6</strong><br>
FBpost.forEach((post) => {<br>
    console.log(post) // log each post here<br>
    });<br>

</blockquote>
<code>filter()</code> is very similar. Below it will iterate over the <code>FBPosts</code> array, perform the logic to filter out the items that do not meet the requirements, and return a new array, <code>results</code>.

<blockquote>
let results = arr1.filter((post) => {
	return post.thumbnail !== null && post.likes > 100 && post.shares > 500
});<br><br>
console.log(results); // [{thumbnail: "someIcon", likes: 432, shares: 600}, {thumbnail: "Another icon", likes: 300, shares: 501}]
</blockquote>

</section>



## Instructions
<section id='instructions'>
Use arrow function syntax to compute the square of <em>only</em> the positive integers (decimal numbers are not integers) in the array <code>realNumberArray</code> and store the new array in the variable <code>squaredIntegers</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const realNumberArray = [4, 5.6, -9.8, 3.14, 42, 6, 8.34, -2];
const squareList = (arr) => {
  "use strict";
  const positiveIntegers = arr.filter((num) => {
     // add code here
  });
  const squaredIntegers = positiveIntegers.map((num) => {
       // add code here
  });

  return squaredIntegers;
};
// test your code
const squaredIntegers = squareList(realNumberArray);
console.log(squaredIntegers);

```

</div>



</section>

## Solution
<section id='solution'>

```js
const realNumberArray = [4, 5.6, -9.8, 3.14, 42, 6, 8.34, -2];
const squareList = (arr) => {
  "use strict";
  const positiveIntegers = arr.filter((num) => {
    return num >= 0 && Number.isInteger(num);
      // add code here
  });
  const squaredIntegers = positiveIntegers.map((num) => {
    // add code here
    return num **2;
  });
  // add code here
  return squaredIntegers;
};
// test your code
const squaredIntegers = squareList(realNumberArray);
```
</section>
<hr>

# 9. Set Default Parameters for Your Functions

## Description
<section id='description'>
In order to help us create more flexible functions, ES6 introduces <dfn>default parameters</dfn> for functions.
Check out this code:
<blockquote>function greeting(name = "Anonymous") {<br>&nbsp;&nbsp;return "Hello " + name;<br>}<br>console.log(greeting("John")); // Hello John<br>console.log(greeting()); // Hello Anonymous</blockquote>
The default parameter kicks in when the argument is not specified (it is undefined). As you can see in the example above, the parameter <code>name</code> will receive its default value <code>"Anonymous"</code> when you do not provide a value for the parameter. You can add default values for as many parameters as you want.
</section>

## Instructions
<section id='instructions'>
Modify the function <code>increment</code> by adding default parameters so that it will add 1 to <code>number</code> if <code>value</code> is not specified.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const increment = (function() {
  "use strict";
  return function increment(number, value) {
    return number + value;
  };
})();
console.log(increment(5, 2)); // returns 7
console.log(increment(5)); // returns 6
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

# 10. Use the Rest Operator with Function Parameters

## Description
<section id='description'>
In order to help us create more flexible functions, ES6 introduces the <dfn>rest operator</dfn> for function parameters. With the rest operator, you can create functions that take a variable number of arguments. These arguments are stored in an array that can be accessed later from inside the function.
Check out this code:
<blockquote>function howMany(...args) {<br>&nbsp;&nbsp;return "You have passed " + args.length + " arguments.";<br>}<br>console.log(howMany(0, 1, 2)); // You have passed 3 arguments<br>console.log(howMany("string", null, [1, 2, 3], { })); // You have passed 4 arguments.</blockquote>
The rest operator eliminates the need to check the <code>args</code> array and allows us to apply <code>map()</code>, <code>filter()</code> and <code>reduce()</code> on the parameters array.
</section>

## Instructions
<section id='instructions'>
Modify the function <code>sum</code> using the rest parameter in such a way that the function <code>sum</code> is able to take any number of arguments and return their sum.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const sum = (function() {
  "use strict";
  return function sum(x, y, z) {
    const args = [ x, y, z ];
    return args.reduce((a, b) => a + b, 0);
  };
})();
console.log(sum(1, 2, 3)); // 6
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

# 11. Use the Spread Operator to Evaluate Arrays In-Place

## Description
<section id='description'>
ES6 introduces the <dfn>spread operator</dfn>, which allows us to expand arrays and other expressions in places where multiple parameters or elements are expected.
The ES5 code below uses <code>apply()</code> to compute the maximum value in an array:
<blockquote>var arr = [6, 89, 3, 45];<br>var maximus = Math.max.apply(null, arr); // returns 89</blockquote>
We had to use <code>Math.max.apply(null, arr)</code> because <code>Math.max(arr)</code> returns <code>NaN</code>. <code>Math.max()</code> expects comma-separated arguments, but not an array.
The spread operator makes this syntax much better to read and maintain.
<blockquote>const arr = [6, 89, 3, 45];<br>const maximus = Math.max(...arr); // returns 89</blockquote>
<code>...arr</code> returns an unpacked array. In other words, it <em>spreads</em> the array.
However, the spread operator only works in-place, like in an argument to a function or in an array literal. The following code will not work:
<blockquote>const spreaded = ...arr; // will throw a syntax error</blockquote>
</section>

## Instructions
<section id='instructions'>
Copy all contents of <code>arr1</code> into another array <code>arr2</code> using the spread operator.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const arr1 = ['JAN', 'FEB', 'MAR', 'APR', 'MAY'];
let arr2;
(function() {
  "use strict";
  arr2 = []; // change this line
})();
console.log(arr2);
```

</div>



</section>

## Solution
<section id='solution'>

```js
const arr1 = ['JAN', 'FEB', 'MAR', 'APR', 'MAY'];
let arr2;
(function() {
  "use strict";
  arr2 = [...arr1]; // change this line
})();
console.log(arr2);
```
</section>
<hr>

# 12. Use Destructuring Assignment to Assign Variables from Objects

## Description
<section id='description'>
We saw earlier how spread operator can effectively spread, or unpack, the contents of the array.
We can do something similar with objects as well. <dfn>Destructuring assignment</dfn> is special syntax for neatly assigning values taken directly from an object to variables.
Consider the following ES5 code:
<blockquote>var voxel = {x: 3.6, y: 7.4, z: 6.54 };<br>var x = voxel.x; // x = 3.6<br>var y = voxel.y; // y = 7.4<br>var z = voxel.z; // z = 6.54</blockquote>
Here's the same assignment statement with ES6 destructuring syntax:
<blockquote>const { x, y, z } = voxel; // x = 3.6, y = 7.4, z = 6.54</blockquote>
If instead you want to store the values of <code>voxel.x</code> into <code>a</code>, <code>voxel.y</code> into <code>b</code>, and <code>voxel.z</code> into <code>c</code>, you have that freedom as well.
<blockquote>const { x : a, y : b, z : c } = voxel; // a = 3.6, b = 7.4, c = 6.54</blockquote>
You may read it as "get the field <code>x</code> and copy the value into <code>a</code>," and so on.
</section>

## Instructions
<section id='instructions'>
Use destructuring to obtain the average temperature for tomorrow from the input object <code>AVG_TEMPERATURES</code>, and assign value with key <code>tomorrow</code> to <code>tempOfTomorrow</code> in line.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const AVG_TEMPERATURES = {
  today: 77.5,
  tomorrow: 79
};

function getTempOfTmrw(avgTemperatures) {
  "use strict";
  // change code below this line
  const tempOfTomorrow = undefined; // change this line
  // change code above this line
  return tempOfTomorrow;
}

console.log(getTempOfTmrw(AVG_TEMPERATURES)); // should be 79
```

</div>



</section>

## Solution
<section id='solution'>

```js
const AVG_TEMPERATURES = {
  today: 77.5,
  tomorrow: 79
};

function getTempOfTmrw(avgTemperatures) {
  "use strict";
  // change code below this line
  const {tomorrow:tempOfTomorrow} = avgTemperatures; // change this line
  // change code above this line
  return tempOfTomorrow;
}

console.log(getTempOfTmrw(AVG_TEMPERATURES)); // should be 79
```
</section>
<hr>

# 13. Use Destructuring Assignment to Assign Variables from Nested Objects

## Description
<section id='description'>
We can similarly destructure <em>nested</em> objects into variables.
Consider the following code:
<blockquote>const a = {<br>&nbsp;&nbsp;start: { x: 5, y: 6},<br>&nbsp;&nbsp;end: { x: 6, y: -9 }<br>};<br>const { start : { x: startX, y: startY }} = a;<br>console.log(startX, startY); // 5, 6</blockquote>
In the example above, the variable <code>startX</code> is assigned the value of <code>a.start.x</code>.
</section>

## Instructions
<section id='instructions'>
Use destructuring assignment to obtain <code>max</code> of <code>forecast.tomorrow</code> and assign it to <code>maxOfTomorrow</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const LOCAL_FORECAST = {
  today: { min: 72, max: 83 },
  tomorrow: { min: 73.3, max: 84.6 }
};

function getMaxOfTmrw(forecast) {
  "use strict";
  // change code below this line
  const maxOfTomorrow = undefined; // change this line
  // change code above this line
  return maxOfTomorrow;
}

console.log(getMaxOfTmrw(LOCAL_FORECAST)); // should be 84.6
```

</div>



</section>

## Solution
<section id='solution'>

```js
const LOCAL_FORECAST = {
  today: { min: 72, max: 83 },
  tomorrow: { min: 73.3, max: 84.6 }
};

function getMaxOfTmrw(forecast) {
  "use strict";
  // change code below this line
   const {tomorrow : {max : maxOfTomorrow}} = forecast; // change this line
  // change code above this line
  return maxOfTomorrow;
}

console.log(getMaxOfTmrw(LOCAL_FORECAST)); // should be 84.6
```
</section>
<hr>

# 14. Use Destructuring Assignment to Assign Variables from Arrays

## Description
<section id='description'>
ES6 makes destructuring arrays as easy as destructuring objects.
One key difference between the spread operator and array destructuring is that the spread operator unpacks all contents of an array into a comma-separated list. Consequently, you cannot pick or choose which elements you want to assign to variables.
Destructuring an array lets us do exactly that:
<blockquote>const [a, b] = [1, 2, 3, 4, 5, 6];<br>console.log(a, b); // 1, 2</blockquote>
The variable <code>a</code> is assigned the first value of the array, and <code>b</code> is assigned the second value of the array.
We can also access the value at any index in an array with destructuring by using commas to reach the desired index:
<blockquote>const [a, b,,, c] = [1, 2, 3, 4, 5, 6];<br>console.log(a, b, c); // 1, 2, 5 </blockquote>
</section>

## Instructions
<section id='instructions'>
Use destructuring assignment to swap the values of <code>a</code> and <code>b</code> so that <code>a</code> receives the value stored in <code>b</code>, and <code>b</code> receives the value stored in <code>a</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let a = 8, b = 6;
(() => {
  "use strict";
  // change code below this line

  // change code above this line
})();
console.log(a); // should be 6
console.log(b); // should be 8
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

# 15. Use Destructuring Assignment with the Rest Operator to Reassign Array Elements

## Description
<section id='description'>
In some situations involving array destructuring, we might want to collect the rest of the elements into a separate array.
The result is similar to <code>Array.prototype.slice()</code>, as shown below:
<blockquote>const [a, b, ...arr] = [1, 2, 3, 4, 5, 7];<br>console.log(a, b); // 1, 2<br>console.log(arr); // [3, 4, 5, 7]</blockquote>
Variables <code>a</code> and <code>b</code> take the first and second values from the array. After that, because of rest operator's presence, <code>arr</code> gets rest of the values in the form of an array.
The rest element only works correctly as the last variable in the list. As in, you cannot use the rest operator to catch a subarray that leaves out last element of the original array.
</section>

## Instructions
<section id='instructions'>
Use destructuring assignment with the rest operator to perform an effective <code>Array.prototype.slice()</code> so that <code>arr</code> is a sub-array of the original array <code>source</code> with the first two elements omitted.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const source = [1,2,3,4,5,6,7,8,9,10];
function removeFirstTwo(list) {
  "use strict";
  // change code below this line
  const arr = list; // change this
  // change code above this line
  return arr;
}
const arr = removeFirstTwo(source);
console.log(arr); // should be [3,4,5,6,7,8,9,10]
console.log(source); // should be [1,2,3,4,5,6,7,8,9,10];
```

</div>



</section>

## Solution
<section id='solution'>

```js
const source = [1,2,3,4,5,6,7,8,9,10];
function removeFirstTwo(list) {
  "use strict";
  // change code below this line
  const [, , ...arr] = list;
  // change code above this line
  return arr;
}
const arr = removeFirstTwo(source);
```
</section>
<hr>

# 16. Use Destructuring Assignment to Pass an Object as a Function's Parameters

## Description
<section id='description'>
In some cases, you can destructure the object in a function argument itself.
Consider the code below:
<blockquote>const profileUpdate = (profileData) => {<br>&nbsp;&nbsp;const { name, age, nationality, location } = profileData;<br>&nbsp;&nbsp;// do something with these variables<br>}</blockquote>
This effectively destructures the object sent into the function. This can also be done in-place:
<blockquote>const profileUpdate = ({ name, age, nationality, location }) => {<br>&nbsp;&nbsp;/*do something with these fields */<br>}</blockquote>
This removes some extra lines and makes our code look neat.
This has the added benefit of not having to manipulate an entire object in a function; only the fields that are needed are copied inside the function.
</section>

## Instructions
<section id='instructions'>
Use destructuring assignment within the argument to the function <code>half</code> to send only <code>max</code> and <code>min</code> inside the function.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const stats = {
  max: 56.78,
  standard_deviation: 4.34,
  median: 34.54,
  mode: 23.87,
  min: -0.75,
  average: 35.85
};
const half = (function() {
  "use strict"; // do not change this line

  // change code below this line
  return function half(stats) {
    // use function argument destructuring
    return (stats.max + stats.min) / 2.0;
  };
  // change code above this line

})();
console.log(stats); // should be object
console.log(half(stats)); // should be 28.015
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

# 17. Create Strings using Template Literals

## Description
<section id='description'>
A new feature of ES6 is the <dfn>template literal</dfn>. This is a special type of string that makes creating complex strings easier.
Template literals allow you to create multi-line strings and to use string interpolation features to create strings.
Consider the code below:
<blockquote>const person = {<br>&nbsp;&nbsp;name: "Zodiac Hasbro",<br>&nbsp;&nbsp;age: 56<br>};<br><br>// Template literal with multi-line and string interpolation<br>const greeting = `Hello, my name is ${person.name}!<br>I am ${person.age} years old.`;<br><br>console.log(greeting); // prints<br>// Hello, my name is Zodiac Hasbro!<br>// I am 56 years old.<br></blockquote>
A lot of things happened there.
Firstly, the example uses backticks (<code>`</code>), not quotes (<code>'</code> or <code>"</code>), to wrap the string.
Secondly, notice that the string is multi-line, both in the code and the output. This saves inserting <code>\n</code> within strings.
The <code>${variable}</code> syntax used above is a placeholder. Basically, you won't have to use concatenation with the <code>+</code> operator anymore. To add variables to strings, you just drop the variable in a template string and wrap it with <code>${</code> and <code>}</code>. Similarly, you can include other expressions in your string literal, for example <code>${a + b}</code>.
This new way of creating strings gives you more flexibility to create robust strings.
</section>

## Instructions
<section id='instructions'>
Use template literal syntax with backticks to display each entry of the <code>result</code> object's <code>failure</code> array. Each entry should be wrapped inside an <code>li</code> element with the class attribute <code>text-warning</code>, and listed within the <code>resultDisplayArray</code>.
Use an iterator method (any kind of loop) to get the desired output.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const result = {
  success: ["max-length", "no-amd", "prefer-arrow-functions"],
  failure: ["no-var", "var-on-top", "linebreak"],
  skipped: ["id-blacklist", "no-dup-keys"]
};
function makeList(arr) {
  "use strict";

  // change code below this line
  const resultDisplayArray = null;
  // change code above this line

  return resultDisplayArray;
}
/** *makeList(result.failure) should return:
 *[ `<li class="text-warning">no-var</li>`,
 *  `<li class="text-warning">var-on-top</li>`,
 *  `<li class="text-warning">linebreak</li>` ]
 **/
const resultDisplayArray = makeList(result.failure);
```

</div>



</section>

## Solution
<section id='solution'>

```js
const result = {
  success: ["max-length", "no-amd", "prefer-arrow-functions"],
  failure: ["no-var", "var-on-top", "linebreak"],
  skipped: ["id-blacklist", "no-dup-keys"]
};
function makeList(arr) {
  "use strict";
  
  const resultDisplayArray = arr.map(val => `<li class="text-warning">${val}</li>`);
  
  return resultDisplayArray;
}
/** *makeList(result.failure) should return:
 *[ `<li class="text-warning">no-var</li>`,
 *  `<li class="text-warning">var-on-top</li>`,
 *  `<li class="text-warning">linebreak</li>` ]
 **/
const resultDisplayArray = makeList(result.failure);
```
</section>
<hr>

# 18. Write Concise Object Literal Declarations Using Simple Fields

## Description
<section id='description'>
ES6 adds some nice support for easily defining object literals.
Consider the following code:
<blockquote>const getMousePosition = (x, y) => ({<br>&nbsp;&nbsp;x: x,<br>&nbsp;&nbsp;y: y<br>});</blockquote>
<code>getMousePosition</code> is a simple function that returns an object containing two fields.
ES6 provides the syntactic sugar to eliminate the redundancy of having to write <code>x: x</code>. You can simply write <code>x</code> once, and it will be converted to<code>x: x</code> (or something equivalent) under the hood.
Here is the same function from above rewritten to use this new syntax:
<blockquote>const getMousePosition = (x, y) => ({ x, y });</blockquote>
</section>

## Instructions
<section id='instructions'>
Use simple fields with object literals to create and return a <code>Person</code> object with <code>name</code>, <code>age</code> and <code>gender</code> properties.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
const createPerson = (name, age, gender) => {
  "use strict";
  // change code below this line
  return {
    name: name,
    age: age,
    gender: gender
  };
  // change code above this line
};
console.log(createPerson("Zodiac Hasbro", 56, "male")); // returns a proper object
```

</div>



</section>

## Solution
<section id='solution'>

```js
const createPerson = (name, age, gender) => {
  "use strict";
  return {
    name,
    age,
    gender
  };
};
```
</section>
<hr>

# 19. Write Concise Declarative Functions with ES6

## Description
<section id='description'>
When defining functions within objects in ES5, we have to use the keyword <code>function</code> as follows:
<blockquote>const person = {<br>&nbsp;&nbsp;name: "Taylor",<br>&nbsp;&nbsp;sayHello: function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;return `Hello! My name is ${this.name}.`;<br>&nbsp;&nbsp;}<br>};</blockquote>
With ES6, You can remove the <code>function</code> keyword and colon altogether when defining functions in objects. Here's an example of this syntax:
<blockquote>const person = {<br>&nbsp;&nbsp;name: "Taylor",<br>&nbsp;&nbsp;sayHello() {<br>&nbsp;&nbsp;&nbsp;&nbsp;return `Hello! My name is ${this.name}.`;<br>&nbsp;&nbsp;}<br>};</blockquote>
</section>

## Instructions
<section id='instructions'>
Refactor the function <code>setGear</code> inside the object <code>bicycle</code> to use the shorthand syntax described above.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// change code below this line
const bicycle = {
  gear: 2,
  setGear: function(newGear) {
    this.gear = newGear;
  }
};
// change code above this line
bicycle.setGear(3);
console.log(bicycle.gear);
```

</div>

</section>

## Solution
<section id='solution'>

```js
const bicycle = {
  gear: 2,
  setGear(newGear) {
    this.gear = newGear;
  }
};
bicycle.setGear(3);
```

</section>
<hr>

# 20. Use class Syntax to Define a Constructor Function

## Description
<section id='description'>
ES6 provides a new syntax to help create objects, using the keyword <dfn>class</dfn>.
This is to be noted, that the <code>class</code> syntax is just a syntax, and not a full-fledged class based implementation of object oriented paradigm, unlike in languages like Java, or Python, or Ruby etc.
In ES5, we usually define a constructor function, and use the <code>new</code> keyword to instantiate an object.
<blockquote>var SpaceShuttle = function(targetPlanet){<br>&nbsp;&nbsp;this.targetPlanet = targetPlanet;<br>}<br>var zeus = new SpaceShuttle('Jupiter');</blockquote>
The class syntax simply replaces the constructor function creation:
<blockquote>class SpaceShuttle {<br>&nbsp;&nbsp;constructor(targetPlanet){<br>&nbsp;&nbsp;&nbsp;&nbsp;this.targetPlanet = targetPlanet;<br>&nbsp;&nbsp;}<br>}<br>const zeus = new SpaceShuttle('Jupiter');</blockquote>
Notice that the <code>class</code> keyword declares a new function, and a constructor was added, which would be invoked when <code>new</code> is called - to create a new object.<br>
<strong>Note</strong><br>
UpperCamelCase should be used by convention for ES6 class names, as in <code>SpaceShuttle</code> used above.
</section>

## Instructions
<section id='instructions'>
Use <code>class</code> keyword and write a proper constructor to create the <code>Vegetable</code> class.
The <code>Vegetable</code> lets you create a vegetable object, with a property <code>name</code>, to be passed to constructor.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function makeClass() {
  "use strict";
  /*Alter code below this line */

  /*Alter code above this line */
  return Vegetable;
}
const Vegetable = makeClass();
const carrot = new Vegetable('carrot');
console.log(carrot.name); // => should be 'carrot'
```

</div>



</section>

## Solution
<section id='solution'>

```js
function makeClass() {
  "use strict";
  /*Alter code below this line */
  class Vegetable {
    constructor(name){
      this.name = name;
    }
  }
  /*Alter code above this line */
  return Vegetable;
}
const Vegetable = makeClass();
const carrot = new Vegetable('carrot');
console.log(carrot.name); // => should be 'carrot'
```
</section>
<hr>

# 21. Use getters and setters to Control Access to an Object

## Description
<section id='description'>
You can obtain values from an object, and set a value of a property within an object.
These are classically called <dfn>getters</dfn> and <dfn>setters</dfn>.
Getter functions are meant to simply return (get) the value of an object's private variable to the user without the user directly accessing the private variable.
Setter functions are meant to modify (set) the value of an object's private variable based on the value passed into the setter function. This change could involve calculations, or even overwriting the previous value completely.<br><br>
<blockquote>class Book {<br>&nbsp;&nbsp;constructor(author) {<br>&nbsp;&nbsp;&nbsp;&nbsp;this._author = author;<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;// getter<br>&nbsp;&nbsp;get writer(){<br>&nbsp;&nbsp;&nbsp;&nbsp;return this._author;<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;// setter<br>&nbsp;&nbsp;set writer(updatedAuthor){<br>&nbsp;&nbsp;&nbsp;&nbsp;this._author = updatedAuthor;<br>&nbsp;&nbsp;}<br>}<br>const lol = new Book('anonymous');<br>console.log(lol.writer);&nbsp;&nbsp;// anonymous<br>lol.writer = 'wut';<br>console.log(lol.writer);&nbsp;&nbsp;// wut</blockquote>
Notice the syntax we are using to invoke the getter and setter - as if they are not even functions.
Getters and setters are important, because they hide internal implementation details.
<br><br>
<strong>Note:</strong><br>It is a convention to precede the name of a private variable with an underscore (<code>_</code>). The practice itself does not make a variable private.
</section>

## Instructions
<section id='instructions'>
Use <code>class</code> keyword to create a Thermostat class. The constructor accepts Fahrenheit temperature.
Now create <code>getter</code> and <code>setter</code> in the class, to obtain the temperature in Celsius scale.
Remember that <code>C = 5/9 *(F - 32)</code> and <code>F = C *9.0 / 5 + 32</code>, where F is the value of temperature in Fahrenheit scale, and C is the value of the same temperature in Celsius scale
Note
When you implement this, you would be tracking the temperature inside the class in one scale - either Fahrenheit or Celsius.
This is the power of getter or setter - you are creating an API for another user, who would get the correct result, no matter which one you track.
In other words, you are abstracting implementation details from the consumer.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function makeClass() {
  "use strict";
  /*Alter code below this line */

  /*Alter code above this line */
  return Thermostat;
}
const Thermostat = makeClass();
const thermos = new Thermostat(76); // setting in Fahrenheit scale
let temp = thermos.temperature; // 24.44 in C
thermos.temperature = 26;
temp = thermos.temperature; // 26 in C
```

</div>



</section>

## Solution
<section id='solution'>

```js
function makeClass() {
  "use strict";
  /*Alter code below this line */
  class Thermostat {
    constructor(fahrenheit) {
      this._tempInCelsius = 5/9 *(fahrenheit - 32);
    }
    get tempInCelsius(){
      return _tempInCelsius;
    }
    set tempInCelsius(newTemp){
      this._tempInCelsius = newTemp;
    }
  }
  /*Alter code above this line */
  return Thermostat;
}
const Thermostat = makeClass();
const thermos = new Thermostat(76); // setting in Fahrenheit scale
let temp = thermos.temperature; // 24.44 in C
thermos.temperature = 26;
temp = thermos.temperature; // 26 in C
```
</section>
<hr>

# 22. Understand the Differences Between import and require

## Description
<section id='description'>
In the past, the function <code>require()</code> would be used to import the functions and code in external files and modules. While handy, this presents a problem: some files and modules are rather large, and you may only need certain code from those external resources.
ES6 gives us a very handy tool known as <dfn>import</dfn>. With it, we can choose which parts of a module or file to load into a given file, saving time and memory.
Consider the following example. Imagine that <code>math_array_functions</code> has about 20 functions, but I only need one, <code>countItems</code>, in my current file. The old <code>require()</code> approach would force me to bring in all 20 functions. With this new <code>import</code> syntax, I can bring in just the desired function, like so:
<blockquote>import { countItems } from "math_array_functions"</blockquote>
A description of the above code:
<blockquote>import { function } from "file_path_goes_here"<br>// We can also import variables the same way!</blockquote>
There are a few ways to write an <code>import</code> statement, but the above is a very common use-case.
<strong>Note</strong><br>The whitespace surrounding the function inside the curly braces is a best practice - it makes it easier to read the <code>import</code> statement.
<strong>Note</strong><br>The lessons in this section handle non-browser features. <code>import</code>, and the statements we introduce in the rest of these lessons, won't work on a browser directly. However, we can use various tools to create code out of this to make it work in browser.
<strong>Note</strong><br>In most cases, the file path requires a <code>./</code> before it; otherwise, node will look in the <code>node_modules</code> directory first trying to load it as a dependency.
</section>

## Instructions
<section id='instructions'>
Add the appropriate <code>import</code> statement that will allow the current file to use the <code>capitalizeString</code> function. The file where this function lives is called <code>"string_functions"</code>, and it is in the same directory as the current file.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
"use strict";
capitalizeString("hello!");
```

</div>

### Before Test
<div id='js-setup'>

```js
self.require = function (str) {
  if (str === 'string_functions') {
    return {
      capitalizeString: str => str.toUpperCase()
    }
  }
};
```

</div>

</section>

## Solution
<section id='solution'>

```js
import { capitalizeString } from 'string_functions';
capitalizeString("hello!");
```

</section>
<hr>

# 23. Use export to Reuse a Code Block

## Description
<section id='description'>
In the previous challenge, you learned about <code>import</code> and how it can be leveraged to import small amounts of code from large files. In order for this to work, though, we must utilize one of the statements that goes with <code>import</code>, known as <dfn>export</dfn>. When we want some code - a function, or a variable - to be usable in another file, we must export it in order to import it into another file. Like <code>import</code>, <code>export</code> is a non-browser feature.
The following is what we refer to as a <dfn>named export</dfn>. With this, we can import any code we export into another file with the <code>import</code> syntax you learned in the last lesson. Here's an example:
<blockquote>const capitalizeString = (string) => {<br>&nbsp;&nbsp;return string.charAt(0).toUpperCase() + string.slice(1);<br>}<br>export { capitalizeString } //How to export functions.<br>export const foo = "bar"; //How to export variables.</blockquote>
Alternatively, if you would like to compact all your <code>export</code> statements into one line, you can take this approach:
<blockquote>const capitalizeString = (string) => {<br>&nbsp;&nbsp;return string.charAt(0).toUpperCase() + string.slice(1);<br>}<br>const foo = "bar";<br>export { capitalizeString, foo }</blockquote>
Either approach is perfectly acceptable.
</section>

## Instructions
<section id='instructions'>
Below are two variables that I want to make available for other files to use. Utilizing the first way I demonstrated <code>export</code>, export the two variables.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
"use strict";
const foo = "bar";
const bar = "foo";
```

</div>

### Before Test
<div id='js-setup'>

```js
self.exports = function(){};
```

</div>


</section>

## Solution
<section id='solution'>

```js
"use strict";
export const foo = "bar";
export const bar = "foo";
```
</section>
<hr>

# 24. Use * to Import Everything from a File

## Description
<section id='description'>
Suppose you have a file that you wish to import all of its contents into the current file. This can be done with the <dfn>import *</dfn> syntax.
Here's an example where the contents of a file named <code>"math_functions"</code> are imported into a file in the same directory:
<blockquote>import *as myMathModule from "math_functions";<br>myMathModule.add(2,3);<br>myMathModule.subtract(5,3);</blockquote>
And breaking down that code:
<blockquote>import *as object_with_name_of_your_choice from "file_path_goes_here"<br>object_with_name_of_your_choice.imported_function</blockquote>
You may use any name following the <code>import *as </code>portion of the statement. In order to utilize this method, it requires an object that receives the imported values. From here, you will use the dot notation to call your imported values.
</section>

## Instructions
<section id='instructions'>
The code below requires the contents of a file, <code>"capitalize_strings"</code>, found in the same directory as it, imported. Add the appropriate <code>import *</code> statement to the top of the file, using the object provided.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
"use strict";
```

</div>

### Before Test
<div id='js-setup'>

```js
self.require = function(str) {
  if (str === 'capitalize_strings') {
    return {
      capitalize: str => str.toUpperCase(),
      lowercase: str => str.toLowerCase()
    }
  }
};
```

</div>

</section>

## Solution
<section id='solution'>

```js
import *as capitalize_strings from "capitalize_strings";
```

</section>
<hr>

# 25. Create an Export Fallback with export default

## Description
<section id='description'>
In the <code>export</code> lesson, you learned about the syntax referred to as a <dfn>named export</dfn>. This allowed you to make multiple functions and variables available for use in other files.
There is another <code>export</code> syntax you need to know, known as <dfn>export default</dfn>. Usually you will use this syntax if only one value is being exported from a file. It is also used to create a fallback value for a file or module.
Here is a quick example of <code>export default</code>:
<blockquote>export default function add(x,y) {<br>&nbsp;&nbsp;return x + y;<br>}</blockquote>
Note: Since <code>export default</code> is used to declare a fallback value for a module or file, you can only have one value be a default export in each module or file. Additionally, you cannot use <code>export default</code> with <code>var</code>, <code>let</code>, or <code>const</code>
</section>

## Instructions
<section id='instructions'>
The following function should be the fallback value for the module. Please add the necessary code to do so.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
"use strict";
function subtract(x,y) {return x - y;}
```

</div>

### Before Test
<div id='js-setup'>

```js
self.exports = function(){};
```

</div>

</section>

## Solution
<section id='solution'>

```js
export default function subtract(x,y) {return x - y;}
```

</section>
<hr>

# 26. Import a Default Export

## Description
<section id='description'>
In the last challenge, you learned about <code>export default</code> and its uses. It is important to note that, to import a default export, you need to use a different <code>import</code> syntax.
In the following example, we have a function, <code>add</code>, that is the default export of a file, <code>"math_functions"</code>. Here is how to import it:
<blockquote>import add from "math_functions";<br>add(5,4); //Will return 9</blockquote>
The syntax differs in one key place - the imported value, <code>add</code>, is not surrounded by curly braces, <code>{}</code>. Unlike exported values, the primary method of importing a default export is to simply write the value's name after <code>import</code>.
</section>

## Instructions
<section id='instructions'>
In the following code, please import the default export, <code>subtract</code>, from the file <code>"math_functions"</code>, found in the same directory as this file.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
"use strict";
subtract(7,4);
```

</div>

### Before Test
<div id='js-setup'>

```js
self.require = function(str) {
  if (str === 'math_functions') {
    return function(a, b) {
      return a - b;
    }
  }
};
```

</div>

</section>

## Solution
<section id='solution'>

```js
import subtract from "math_functions";
subtract(7,4);
```

</section>
<hr>

# Regular Expressions
# 1. Using the Test Method

## Description
<section id='description'>
Regular expressions are used in programming languages to match parts of strings. You create patterns to help you do that matching.
If you want to find the word <code>"the"</code> in the string <code>"The dog chased the cat"</code>, you could use the following regular expression: <code>/the/</code>. Notice that quote marks are not required within the regular expression.
JavaScript has multiple ways to use regexes. One way to test a regex is using the <code>.test()</code> method. The <code>.test()</code> method takes the regex, applies it to a string (which is placed inside the parentheses), and returns <code>true</code> or <code>false</code> if your pattern finds something or not.
<blockquote>let testStr = "freeCodeCamp";<br>let testRegex = /Code/;<br>testRegex.test(testStr);<br>// Returns true</blockquote>
</section>

## Instructions
<section id='instructions'>
Apply the regex <code>myRegex</code> on the string <code>myString</code> using the <code>.test()</code> method.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let myString = "Hello, World!";
let myRegex = /Hello/;
let result = myRegex; // Change this line
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

# 2. Match Literal Strings

## Description
<section id='description'>
In the last challenge, you searched for the word <code>"Hello"</code> using the regular expression <code>/Hello/</code>. That regex searched for a literal match of the string <code>"Hello"</code>. Here's another example searching for a literal match of the string <code>"Kevin"</code>:
<blockquote>let testStr = "Hello, my name is Kevin.";<br>let testRegex = /Kevin/;<br>testRegex.test(testStr);<br>// Returns true</blockquote>
Any other forms of <code>"Kevin"</code> will not match. For example, the regex <code>/Kevin/</code> will not match <code>"kevin"</code> or <code>"KEVIN"</code>.
<blockquote>let wrongRegex = /kevin/;<br>wrongRegex.test(testStr);<br>// Returns false</blockquote>
A future challenge will show how to match those other forms as well.
</section>

## Instructions
<section id='instructions'>
Complete the regex <code>waldoRegex</code> to find <code>"Waldo"</code> in the string <code>waldoIsHiding</code> with a literal match.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let waldoIsHiding = "Somewhere Waldo is hiding in this text.";
let waldoRegex = /search/; // Change this line
let result = waldoRegex.test(waldoIsHiding);
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

# 3. Match a Literal String with Different Possibilities

## Description
<section id='description'>
Using regexes like <code>/coding/</code>, you can look for the pattern <code>"coding"</code> in another string.
This is powerful to search single strings, but it's limited to only one pattern. You can search for multiple patterns using the <code>alternation</code> or <code>OR</code> operator: <code>|</code>.
This operator matches patterns either before or after it. For example, if you wanted to match <code>"yes"</code> or <code>"no"</code>, the regex you want is <code>/yes|no/</code>.
You can also search for more than just two patterns. You can do this by adding more patterns with more <code>OR</code> operators separating them, like <code>/yes|no|maybe/</code>.
</section>

## Instructions
<section id='instructions'>
Complete the regex <code>petRegex</code> to match the pets <code>"dog"</code>, <code>"cat"</code>, <code>"bird"</code>, or <code>"fish"</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let petString = "James has a pet cat.";
let petRegex = /change/; // Change this line
let result = petRegex.test(petString);
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

# 4. Ignore Case While Matching

## Description
<section id='description'>
Up until now, you've looked at regexes to do literal matches of strings. But sometimes, you might want to also match case differences.
Case (or sometimes letter case) is the difference between uppercase letters and lowercase letters. Examples of uppercase are <code>"A"</code>, <code>"B"</code>, and <code>"C"</code>. Examples of lowercase are <code>"a"</code>, <code>"b"</code>, and <code>"c"</code>.
You can match both cases using what is called a flag. There are other flags but here you'll focus on the flag that ignores case - the <code>i</code> flag. You can use it by appending it to the regex.  An example of using this flag is <code>/ignorecase/i</code>. This regex can match the strings <code>"ignorecase"</code>, <code>"igNoreCase"</code>, and <code>"IgnoreCase"</code>.
</section>

## Instructions
<section id='instructions'>
Write a regex <code>fccRegex</code> to match <code>"freeCodeCamp"</code>, no matter its case. Your regex should not match any abbreviations or variations with spaces.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let myString = "freeCodeCamp";
let fccRegex = /change/; // Change this line
let result = fccRegex.test(myString);
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

# 5. Extract Matches

## Description
<section id='description'>
So far, you have only been checking if a pattern exists or not within a string. You can also extract the actual matches you found with the <code>.match()</code> method.
To use the <code>.match()</code> method, apply the method on a string and pass in the regex inside the parentheses. Here's an example:
<blockquote>"Hello, World!".match(/Hello/);<br>// Returns ["Hello"]<br>let ourStr = "Regular expressions";<br>let ourRegex = /expressions/;<br>ourStr.match(ourRegex);<br>// Returns ["expressions"]</blockquote>
</section>

## Instructions
<section id='instructions'>
Apply the <code>.match()</code> method to extract the word <code>coding</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let extractStr = "Extract the word 'coding' from this string.";
let codingRegex = /change/; // Change this line
let result = extractStr; // Change this line
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

# 6. Find More Than the First Match

## Description
<section id='description'>
So far, you have only been able to extract or search a pattern once.
<blockquote>let testStr = "Repeat, Repeat, Repeat";<br>let ourRegex = /Repeat/;<br>testStr.match(ourRegex);<br>// Returns ["Repeat"]</blockquote>
To search or extract a pattern more than once, you can use the <code>g</code> flag.
<blockquote>let repeatRegex = /Repeat/g;<br>testStr.match(repeatRegex);<br>// Returns ["Repeat", "Repeat", "Repeat"]</blockquote>
</section>

## Instructions
<section id='instructions'>
Using the regex <code>starRegex</code>, find and extract both <code>"Twinkle"</code> words from the string <code>twinkleStar</code>.
<strong>Note</strong><br>You can have multiple flags on your regex like <code>/search/gi</code>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let twinkleStar = "Twinkle, twinkle, little star";
let starRegex = /change/; // Change this line
let result = twinkleStar; // Change this line
```

</div>



</section>

## Solution
<section id='solution'>

```js
let twinkleStar = "Twinkle, twinkle, little star";
let starRegex = /twinkle/gi;
let result = twinkleStar.match(starRegex);
```
</section>
<hr>

# 7. Match Anything with Wildcard Period

## Description
<section id='description'>
Sometimes you won't (or don't need to) know the exact characters in your patterns. Thinking of all words that match, say, a misspelling would take a long time. Luckily, you can save time using the wildcard character: <code>.</code>
The wildcard character <code>.</code> will match any one character. The wildcard is also called <code>dot</code> and <code>period</code>. You can use the wildcard character just like any other character in the regex. For example, if you wanted to match <code>"hug"</code>, <code>"huh"</code>, <code>"hut"</code>, and <code>"hum"</code>, you can use the regex <code>/hu./</code> to match all four words.
<blockquote>let humStr = "I'll hum a song";<br>let hugStr = "Bear hug";<br>let huRegex = /hu./;<br>humStr.match(huRegex); // Returns ["hum"]<br>hugStr.match(huRegex); // Returns ["hug"]</blockquote>
</section>

## Instructions
<section id='instructions'>
Complete the regex <code>unRegex</code> so that it matches the strings <code>"run"</code>, <code>"sun"</code>, <code>"fun"</code>, <code>"pun"</code>, <code>"nun"</code>, and <code>"bun"</code>. Your regex should use the wildcard character.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let exampleStr = "Let's have fun with regular expressions!";
let unRegex = /change/; // Change this line
let result = unRegex.test(exampleStr);
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

# 8. Match Single Character with Multiple Possibilities

## Description
<section id='description'>
You learned how to match literal patterns (<code>/literal/</code>) and wildcard character (<code>/./</code>). Those are the extremes of regular expressions, where one finds exact matches and the other matches everything. There are options that are a balance between the two extremes.
You can search for a literal pattern with some flexibility with <code>character classes</code>. Character classes allow you to define a group of characters you wish to match by placing them inside square (<code>[</code> and <code>]</code>) brackets.
For example, you want to match <code>"bag"</code>, <code>"big"</code>, and <code>"bug"</code> but not <code>"bog"</code>. You can create the regex <code>/b[aiu]g/</code> to do this. The <code>[aiu]</code> is the character class that will only match the characters <code>"a"</code>, <code>"i"</code>, or <code>"u"</code>.
<blockquote>let bigStr = "big";<br>let bagStr = "bag";<br>let bugStr = "bug";<br>let bogStr = "bog";<br>let bgRegex = /b[aiu]g/;<br>bigStr.match(bgRegex); // Returns ["big"]<br>bagStr.match(bgRegex); // Returns ["bag"]<br>bugStr.match(bgRegex); // Returns ["bug"]<br>bogStr.match(bgRegex); // Returns null</blockquote>
</section>

## Instructions
<section id='instructions'>
Use a character class with vowels (<code>a</code>, <code>e</code>, <code>i</code>, <code>o</code>, <code>u</code>) in your regex <code>vowelRegex</code> to find all the vowels in the string <code>quoteSample</code>.
<strong>Note</strong><br>Be sure to match both upper- and lowercase vowels.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let quoteSample = "Beware of bugs in the above code; I have only proved it correct, not tried it.";
let vowelRegex = /change/; // Change this line
let result = vowelRegex; // Change this line
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

# 9. Match Letters of the Alphabet

## Description
<section id='description'>
You saw how you can use <code>character sets</code> to specify a group of characters to match, but that's a lot of typing when you need to match a large range of characters (for example, every letter in the alphabet). Fortunately, there is a built-in feature that makes this short and simple.
Inside a <code>character set</code>, you can define a range of characters to match using a <code>hyphen</code> character: <code>-</code>.
For example, to match lowercase letters <code>a</code> through <code>e</code> you would use <code>[a-e]</code>.
<blockquote>let catStr = "cat";<br>let batStr = "bat";<br>let matStr = "mat";<br>let bgRegex = /[a-e]at/;<br>catStr.match(bgRegex); // Returns ["cat"]<br>batStr.match(bgRegex); // Returns ["bat"]<br>matStr.match(bgRegex); // Returns null</blockquote>
</section>

## Instructions
<section id='instructions'>
Match all the letters in the string <code>quoteSample</code>.
<strong>Note</strong><br>Be sure to match both upper- and lowercase <strong>letters<strong>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let quoteSample = "The quick brown fox jumps over the lazy dog.";
let alphabetRegex = /change/; // Change this line
let result = alphabetRegex; // Change this line
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

# 10. Match Numbers and Letters of the Alphabet

## Description
<section id='description'>
Using the hyphen (<code>-</code>) to match a range of characters is not limited to letters. It also works to match a range of numbers.
For example, <code>/[0-5]/</code> matches any number between <code>0</code> and <code>5</code>, including the <code>0</code> and <code>5</code>.
Also, it is possible to combine a range of letters and numbers in a single character set.
<blockquote>let jennyStr = "Jenny8675309";<br>let myRegex = /[a-z0-9]/ig;<br>// matches all letters and numbers in jennyStr<br>jennyStr.match(myRegex);</blockquote>
</section>

## Instructions
<section id='instructions'>
Create a single regex that matches a range of letters between <code>h</code> and <code>s</code>, and a range of numbers between <code>2</code> and <code>6</code>. Remember to include the appropriate flags in the regex.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let quoteSample = "Blueberry 3.141592653s are delicious.";
let myRegex = /change/; // Change this line
let result = myRegex; // Change this line
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

# 11. Match Single Characters Not Specified

## Description
<section id='description'>
So far, you have created a set of characters that you want to match, but you could also create a set of characters that you do not want to match. These types of character sets are called <code>negated character sets</code>.
To create a <code>negated character set</code>, you place a <code>caret</code> character (<code>^</code>) after the opening bracket and before the characters you do not want to match.
For example, <code>/[^aeiou]/gi</code> matches all characters that are not a vowel. Note that characters like <code>.</code>, <code>!</code>, <code>[</code>, <code>@</code>, <code>/</code> and white space are matched - the negated vowel character set only excludes the vowel characters.
</section>

## Instructions
<section id='instructions'>
Create a single regex that matches all characters that are not a number or a vowel. Remember to include the appropriate flags in the regex.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let quoteSample = "3 blind mice.";
let myRegex = /change/; // Change this line
let result = myRegex; // Change this line
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

# 12. Match Characters that Occur One or More Times

## Description
<section id='description'>
Sometimes, you need to match a character (or group of characters) that appears one or more times in a row. This means it occurs at least once, and may be repeated.
You can use the <code>+</code> character to check if that is the case. Remember, the character or pattern has to be present consecutively. That is, the character has to repeat one after the other.
For example, <code>/a+/g</code> would find one match in <code>"abc"</code> and return <code>["a"]</code>. Because of the <code>+</code>, it would also find a single match in <code>"aabc"</code> and return <code>["aa"]</code>.
If it were instead checking the string <code>"abab"</code>, it would find two matches and return <code>["a", "a"]</code> because the <code>a</code> characters are not in a row - there is a <code>b</code> between them. Finally, since there is no <code>"a"</code> in the string <code>"bcd"</code>, it wouldn't find a match.
</section>

## Instructions
<section id='instructions'>
You want to find matches when the letter <code>s</code> occurs one or more times in <code>"Mississippi"</code>. Write a regex that uses the <code>+</code> sign.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let difficultSpelling = "Mississippi";
let myRegex = /change/; // Change this line
let result = difficultSpelling.match(myRegex);
```

</div>



</section>

## Solution
<section id='solution'>

```js
let difficultSpelling = "Mississippi";
let myRegex = /s+/g; // Change this line
let result = difficultSpelling.match(myRegex);
```
</section>
<hr>

# 13. Match Characters that Occur Zero or More Times

## Description
<section id='description'>
The last challenge used the plus <code>+</code> sign to look for characters that occur one or more times. There's also an option that matches characters that occur zero or more times.
The character to do this is the <code>asterisk</code> or <code>star</code>: <code>*</code>.
<blockquote>let soccerWord = "gooooooooal!";<br>let gPhrase = "gut feeling";<br>let oPhrase = "over the moon";<br>let goRegex = /go*/;<br>soccerWord.match(goRegex); // Returns ["goooooooo"]<br>gPhrase.match(goRegex); // Returns ["g"]<br>oPhrase.match(goRegex); // Returns null</blockquote>
</section>

## Instructions
<section id='instructions'>
Create a regex <code>chewieRegex</code> that uses the <code>*</code> character to match all the upper and lowercase <code>"a"</code> characters in <code>chewieQuote</code>. Your regex does not need flags, and it should not match any of the other quotes.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let chewieQuote = "Aaaaaaaaaaaaaaaarrrgh!";
let chewieRegex = /change/; // Change this line
let result = chewieQuote.match(chewieRegex);
```

</div>



</section>

## Solution
<section id='solution'>

```js
  let chewieQuote = "Aaaaaaaaaaaaaaaarrrgh!";
  let chewieRegex = /Aa*/;
  let result = chewieQuote.match(chewieRegex);
```
</section>
<hr>

# 14. Find Characters with Lazy Matching

## Description
<section id='description'>
In regular expressions, a <code>greedy</code> match finds the longest possible part of a string that fits the regex pattern and returns it as a match. The alternative is called a <code>lazy</code> match, which finds the smallest possible part of the string that satisfies the regex pattern.
You can apply the regex <code>/t[a-z]*i/</code> to the string <code>"titanic"</code>. This regex is basically a pattern that starts with <code>t</code>, ends with <code>i</code>, and has some letters in between.
Regular expressions are by default <code>greedy</code>, so the match would return <code>["titani"]</code>. It finds the largest sub-string possible to fit the pattern.
However, you can use the <code>?</code> character to change it to <code>lazy</code> matching. <code>"titanic"</code> matched against the adjusted regex of <code>/t[a-z]*?i/</code> returns <code>["ti"]</code>.
</section>

## Instructions
<section id='instructions'>
Fix the regex <code>/&lt;.*&gt;/</code> to return the HTML tag <code>&lt;h1&gt;</code> and not the text <code>"&lt;h1&gt;Winter is coming&lt;/h1&gt;"</code>. Remember the wildcard <code>.</code> in a regular expression matches any character.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let text = "<h1>Winter is coming</h1>";
let myRegex = /<.*>/; // Change this line
let result = text.match(myRegex);
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

# 15. Find One or More Criminals in a Hunt

## Description
<section id='description'>
Time to pause and test your new regex writing skills. A group of criminals escaped from jail and ran away, but you don't know how many. However, you do know that they stay close together when they are around other people. You are responsible for finding all of the criminals at once.
Here's an example to review how to do this:
The regex <code>/z+/</code> matches the letter <code>z</code> when it appears one or more times in a row. It would find matches in all of the following strings:
<blockquote>"z"<br>"zzzzzz"<br>"ABCzzzz"<br>"zzzzABC"<br>"abczzzzzzzzzzzzzzzzzzzzzabc"</blockquote>
But it does not find matches in the following strings since there are no letter <code>z</code> characters:
<blockquote>""<br>"ABC"<br>"abcabc"</blockquote>
</section>

## Instructions
<section id='instructions'>
Write a <code>greedy</code> regex that finds one or more criminals within a group of other people. A criminal is represented by the capital letter <code>C</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// example crowd gathering
let crowd = 'P1P2P3P4P5P6CCCP7P8P9';

let reCriminals = /./; // Change this line

let matchedCriminals = crowd.match(reCriminals);
console.log(matchedCriminals);
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

# 16. Match Beginning String Patterns

## Description
<section id='description'>
Prior challenges showed that regular expressions can be used to look for a number of matches. They are also used to search for patterns in specific positions in strings.
In an earlier challenge, you used the <code>caret</code> character (<code>^</code>) inside a <code>character set</code> to create a <code>negated character set</code> in the form <code>[^thingsThatWillNotBeMatched]</code>. Outside of a <code>character set</code>, the <code>caret</code> is used to search for patterns at the beginning of strings.
<blockquote>let firstString = "Ricky is first and can be found.";<br>let firstRegex = /^Ricky/;<br>firstRegex.test(firstString);<br>// Returns true<br>let notFirst = "You can't find Ricky now.";<br>firstRegex.test(notFirst);<br>// Returns false</blockquote>
</section>

## Instructions
<section id='instructions'>
Use the <code>caret</code> character in a regex to find <code>"Cal"</code> only in the beginning of the string <code>rickyAndCal</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let rickyAndCal = "Cal and Ricky both like racing.";
let calRegex = /change/; // Change this line
let result = calRegex.test(rickyAndCal);
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

# 17. Match Ending String Patterns

## Description
<section id='description'>
In the last challenge, you learned to use the <code>caret</code> character to search for patterns at the beginning of strings. There is also a way to search for patterns at the end of strings.
You can search the end of strings using the <code>dollar sign</code> character <code>$</code> at the end of the regex.
<blockquote>let theEnding = "This is a never ending story";<br>let storyRegex = /story$/;<br>storyRegex.test(theEnding);<br>// Returns true<br>let noEnding = "Sometimes a story will have to end";<br>storyRegex.test(noEnding);<br>// Returns false<br></blockquote>
</section>

## Instructions
<section id='instructions'>
Use the anchor character (<code>$</code>) to match the string <code>"caboose"</code> at the end of the string <code>caboose</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let caboose = "The last car on a train is the caboose";
let lastRegex = /change/; // Change this line
let result = lastRegex.test(caboose);
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

# 18. Match All Letters and Numbers

## Description
<section id='description'>
Using character classes, you were able to search for all letters of the alphabet with <code>[a-z]</code>. This kind of character class is common enough that there is a shortcut for it, although it includes a few extra characters as well.
The closest character class in JavaScript to match the alphabet is <code>\w</code>. This shortcut is equal to <code>[A-Za-z0-9_]</code>. This character class matches upper and lowercase letters plus numbers. Note, this character class also includes the underscore character (<code>_</code>).
<blockquote>let longHand = /[A-Za-z0-9_]+/;<br>let shortHand = /\w+/;<br>let numbers = "42";<br>let varNames = "important_var";<br>longHand.test(numbers); // Returns true<br>shortHand.test(numbers); // Returns true<br>longHand.test(varNames); // Returns true<br>shortHand.test(varNames); // Returns true</blockquote>
These shortcut character classes are also known as <code>shorthand character classes</code>.
</section>

## Instructions
<section id='instructions'>
Use the shorthand character class <code>\w</code> to count the number of alphanumeric characters in various quotes and strings.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let quoteSample = "The five boxing wizards jump quickly.";
let alphabetRegexV2 = /change/; // Change this line
let result = quoteSample.match(alphabetRegexV2).length;
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

# 19. Match Everything But Letters and Numbers

## Description
<section id='description'>
You've learned that you can use a shortcut to match alphanumerics <code>[A-Za-z0-9_]</code> using <code>\w</code>. A natural pattern you might want to search for is the opposite of alphanumerics.
You can search for the opposite of the <code>\w</code> with <code>\W</code>. Note, the opposite pattern uses a capital letter. This shortcut is the same as <code>[^A-Za-z0-9_]</code>.
<blockquote>let shortHand = /\W/;<br>let numbers = "42%";<br>let sentence = "Coding!";<br>numbers.match(shortHand); // Returns ["%"]<br>sentence.match(shortHand); // Returns ["!"]<br></blockquote>
</section>

## Instructions
<section id='instructions'>
Use the shorthand character class <code>\W</code> to count the number of non-alphanumeric characters in various quotes and strings.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let quoteSample = "The five boxing wizards jump quickly.";
let nonAlphabetRegex = /change/; // Change this line
let result = quoteSample.match(nonAlphabetRegex).length;
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

# 20. Match All Numbers

## Description
<section id='description'>
You've learned shortcuts for common string patterns like alphanumerics. Another common pattern is looking for just digits or numbers.
The shortcut to look for digit characters is <code>\d</code>, with a lowercase <code>d</code>. This is equal to the character class <code>[0-9]</code>, which looks for a single character of any number between zero and nine.
</section>

## Instructions
<section id='instructions'>
Use the shorthand character class <code>\d</code> to count how many digits are in movie titles. Written out numbers ("six" instead of 6) do not count.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let numString = "Your sandwich will be $5.00";
let numRegex = /change/; // Change this line
let result = numString.match(numRegex).length;
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

# 21. Match All Non-Numbers

## Description
<section id='description'>
The last challenge showed how to search for digits using the shortcut <code>\d</code> with a lowercase <code>d</code>. You can also search for non-digits using a similar shortcut that uses an uppercase <code>D</code> instead.
The shortcut to look for non-digit characters is <code>\D</code>. This is equal to the character class <code>[^0-9]</code>, which looks for a single character that is not a number between zero and nine.
</section>

## Instructions
<section id='instructions'>
Use the shorthand character class for non-digits <code>\D</code> to count how many non-digits are in movie titles.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let numString = "Your sandwich will be $5.00";
let noNumRegex = /change/; // Change this line
let result = numString.match(noNumRegex).length;
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

# 22. Restrict Possible Usernames

## Description
<section id='description'>
Usernames are used everywhere on the internet. They are what give users a unique identity on their favorite sites.
You need to check all the usernames in a database. Here are some simple rules that users have to follow when creating their username.
1) The only numbers in the username have to be at the end. There can be zero or more of them at the end.
2) Username letters can be lowercase and uppercase.
3) Usernames have to be at least two characters long. A two-letter username can only use alphabet letter characters.
</section>

## Instructions
<section id='instructions'>
Change the regex <code>userCheck</code> to fit the constraints listed above.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let username = "JackOfAllTrades";
let userCheck = /change/; // Change this line
let result = userCheck.test(username);
```

</div>



</section>

## Solution
<section id='solution'>

```js
const userCheck = /^[A-Za-z]{2,}\d*$/;
```

</section>
<hr>

# 23. Match Whitespace

## Description
<section id='description'>
The challenges so far have covered matching letters of the alphabet and numbers. You can also match the whitespace or spaces between letters.
You can search for whitespace using <code>\s</code>, which is a lowercase <code>s</code>. This pattern not only matches whitespace, but also carriage return, tab, form feed, and new line characters. You can think of it as similar to the character class <code>[ \r\t\f\n\v]</code>.
<blockquote>let whiteSpace = "Whitespace. Whitespace everywhere!"<br>let spaceRegex = /\s/g;<br>whiteSpace.match(spaceRegex);<br>// Returns [" ", " "]<br></blockquote>
</section>

## Instructions
<section id='instructions'>
Change the regex <code>countWhiteSpace</code> to look for multiple whitespace characters in a string.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let sample = "Whitespace is important in separating words";
let countWhiteSpace = /change/; // Change this line
let result = sample.match(countWhiteSpace);
```

</div>



</section>

## Solution
<section id='solution'>

```js
let sample = "Whitespace is important in separating words";
let countWhiteSpace = /\s/g;
let result = sample.match(countWhiteSpace);
```
</section>
<hr>

# 24. Match Non-Whitespace Characters

## Description
<section id='description'>
You learned about searching for whitespace using <code>\s</code>, with a lowercase <code>s</code>. You can also search for everything except whitespace.
Search for non-whitespace using <code>\S</code>, which is an uppercase <code>s</code>. This pattern will not match whitespace, carriage return, tab, form feed, and new line characters. You can think of it being similar to the character class <code>[^ \r\t\f\n\v]</code>.
<blockquote>let whiteSpace = "Whitespace. Whitespace everywhere!"<br>let nonSpaceRegex = /\S/g;<br>whiteSpace.match(nonSpaceRegex).length; // Returns 32</blockquote>
</section>

## Instructions
<section id='instructions'>
Change the regex <code>countNonWhiteSpace</code> to look for multiple non-whitespace characters in a string.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let sample = "Whitespace is important in separating words";
let countNonWhiteSpace = /change/; // Change this line
let result = sample.match(countNonWhiteSpace);
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

# 25. Specify Upper and Lower Number of Matches

## Description
<section id='description'>
Recall that you use the plus sign <code>+</code> to look for one or more characters and the asterisk <code>*</code> to look for zero or more characters. These are convenient but sometimes you want to match a certain range of patterns.
You can specify the lower and upper number of patterns with <code>quantity specifiers</code>. Quantity specifiers are used with curly brackets (<code>{</code> and <code>}</code>). You put two numbers between the curly brackets - for the lower and upper number of patterns.
For example, to match only the letter <code>a</code> appearing between <code>3</code> and <code>5</code> times in the string <code>"ah"</code>, your regex would be <code>/a{3,5}h/</code>.
<blockquote>let A4 = "aaaah";<br>let A2 = "aah";<br>let multipleA = /a{3,5}h/;<br>multipleA.test(A4); // Returns true<br>multipleA.test(A2); // Returns false</blockquote>
</section>

## Instructions
<section id='instructions'>
Change the regex <code>ohRegex</code> to match only <code>3</code> to <code>6</code> letter <code>h</code>'s in the word <code>"Oh no"</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let ohStr = "Ohhh no";
let ohRegex = /change/; // Change this line
let result = ohRegex.test(ohStr);
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

# 26. Specify Only the Lower Number of Matches

## Description
<section id='description'>
You can specify the lower and upper number of patterns with <code>quantity specifiers</code> using curly brackets. Sometimes you only want to specify the lower number of patterns with no upper limit.
To only specify the lower number of patterns, keep the first number followed by a comma.
For example, to match only the string <code>"hah"</code> with the letter <code>a</code> appearing at least <code>3</code> times, your regex would be <code>/ha{3,}h/</code>.
<blockquote>let A4 = "haaaah";<br>let A2 = "haah";<br>let A100 = "h" + "a".repeat(100) + "h";<br>let multipleA = /ha{3,}h/;<br>multipleA.test(A4); // Returns true<br>multipleA.test(A2); // Returns false<br>multipleA.test(A100); // Returns true</blockquote>
</section>

## Instructions
<section id='instructions'>
Change the regex <code>haRegex</code> to match the word <code>"Hazzah"</code> only when it has four or more letter <code>z</code>'s.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let haStr = "Hazzzzah";
let haRegex = /change/; // Change this line
let result = haRegex.test(haStr);
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

# 27. Specify Exact Number of Matches

## Description
<section id='description'>
You can specify the lower and upper number of patterns with <code>quantity specifiers</code> using curly brackets. Sometimes you only want a specific number of matches.
To specify a certain number of patterns, just have that one number between the curly brackets.
For example, to match only the word <code>"hah"</code> with the letter <code>a</code> <code>3</code> times, your regex would be <code>/ha{3}h/</code>.
<blockquote>let A4 = "haaaah";<br>let A3 = "haaah";<br>let A100 = "h" + "a".repeat(100) + "h";<br>let multipleHA = /ha{3}h/;<br>multipleHA.test(A4); // Returns false<br>multipleHA.test(A3); // Returns true<br>multipleHA.test(A100); // Returns false</blockquote>
</section>

## Instructions
<section id='instructions'>
Change the regex <code>timRegex</code> to match the word <code>"Timber"</code> only when it has four letter <code>m</code>'s.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let timStr = "Timmmmber";
let timRegex = /change/; // Change this line
let result = timRegex.test(timStr);
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

# 28. Check for All or None

## Description
<section id='description'>
Sometimes the patterns you want to search for may have parts of it that may or may not exist. However, it may be important to check for them nonetheless.
You can specify the possible existence of an element with a question mark, <code>?</code>. This checks for zero or one of the preceding element. You can think of this symbol as saying the previous element is optional.
For example, there are slight differences in American and British English and you can use the question mark to match both spellings.
<blockquote>let american = "color";<br>let british = "colour";<br>let rainbowRegex= /colou?r/;<br>rainbowRegex.test(american); // Returns true<br>rainbowRegex.test(british); // Returns true</blockquote>
</section>

## Instructions
<section id='instructions'>
Change the regex <code>favRegex</code> to match both the American English (favorite) and the British English (favourite) version of the word.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let favWord = "favorite";
let favRegex = /change/; // Change this line
let result = favRegex.test(favWord);
```

</div>



</section>

## Solution
<section id='solution'>

```js
let favWord = "favorite";
let favRegex = /favou?r/;
let result = favRegex.test(favWord);
```
</section>
<hr>

# 29. Positive and Negative Lookahead

## Description
<section id='description'>
<code>Lookaheads</code> are patterns that tell JavaScript to look-ahead in your string to check for patterns further along. This can be useful when you want to search for multiple patterns over the same string.
There are two kinds of <code>lookaheads</code>: <code>positive lookahead</code> and <code>negative lookahead</code>.
A <code>positive lookahead</code> will look to make sure the element in the search pattern is there, but won't actually match it. A positive lookahead is used as <code>(?=...)</code> where the <code>...</code> is the required part that is not matched.
On the other hand, a <code>negative lookahead</code> will look to make sure the element in the search pattern is not there. A negative lookahead is used as <code>(?!...)</code> where the <code>...</code> is the pattern that you do not want to be there. The rest of the pattern is returned if the negative lookahead part is not present.
Lookaheads are a bit confusing but some examples will help.
<blockquote>let quit = "qu";<br>let noquit = "qt";<br>let quRegex= /q(?=u)/;<br>let qRegex = /q(?!u)/;<br>quit.match(quRegex); // Returns ["q"]<br>noquit.match(qRegex); // Returns ["q"]</blockquote>
A more practical use of <code>lookaheads</code> is to check two or more patterns in one string. Here is a (naively) simple password checker that looks for between 3 and 6 characters and at least one number:
<blockquote>let password = "abc123";<br>let checkPass = /(?=\w{3,6})(?=\D*\d)/;<br>checkPass.test(password); // Returns true</blockquote>
</section>

## Instructions
<section id='instructions'>
Use <code>lookaheads</code> in the <code>pwRegex</code> to match passwords that are greater than 5 characters long, do not begin with numbers, and have two consecutive digits.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let sampleWord = "astronaut";
let pwRegex = /change/; // Change this line
let result = pwRegex.test(sampleWord);
```

</div>



</section>

## Solution
<section id='solution'>


```js
var pwRegex = /(?=\w{5})(?=\D*\d{2})/;
```

</section>
<hr>

# 30. Reuse Patterns Using Capture Groups

## Description
<section id='description'>
Some patterns you search for will occur multiple times in a string. It is wasteful to manually repeat that regex. There is a better way to specify when you have multiple repeat substrings in your string.
You can search for repeat substrings using <code>capture groups</code>. Parentheses, <code>(</code> and <code>)</code>, are used to find repeat substrings. You put the regex of the pattern that will repeat in between the parentheses.
To specify where that repeat string will appear, you use a backslash (<code>\</code>) and then a number. This number starts at 1 and increases with each additional capture group you use. An example would be <code>\1</code> to match the first group.
The example below matches any word that occurs twice separated by a space:
<blockquote>let repeatStr = "regex regex";<br>let repeatRegex = /(\w+)\s\1/;<br>repeatRegex.test(repeatStr); // Returns true<br>repeatStr.match(repeatRegex); // Returns ["regex regex", "regex"]</blockquote>
Using the <code>.match()</code> method on a string will return an array with the string it matches, along with its capture group.
</section>

## Instructions
<section id='instructions'>
Use <code>capture groups</code> in <code>reRegex</code> to match numbers that are repeated only three times in a string, each separated by a space.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let repeatNum = "42 42 42";
let reRegex = /change/; // Change this line
let result = reRegex.test(repeatNum);
```

</div>



</section>

## Solution
<section id='solution'>

```js
let repeatNum = "42 42 42";
let reRegex = /^(\d+)\s\1\s\1$/;
let result = reRegex.test(repeatNum);
```
</section>
<hr>

# 31. Use Capture Groups to Search and Replace

## Description
<section id='description'>
Searching is useful. However, you can make searching even more powerful when it also changes (or replaces) the text you match.
You can search and replace text in a string using <code>.replace()</code> on a string. The inputs for <code>.replace()</code> is first the regex pattern you want to search for. The second parameter is the string to replace the match or a function to do something.
<blockquote>let wrongText = "The sky is silver.";<br>let silverRegex = /silver/;<br>wrongText.replace(silverRegex, "blue");<br>// Returns "The sky is blue."</blockquote>
You can also access capture groups in the replacement string with dollar signs (<code>$</code>).
<blockquote>"Code Camp".replace(/(\w+)\s(\w+)/, '$2 $1');<br>// Returns "Camp Code"</blockquote>
</section>

## Instructions
<section id='instructions'>
Write a regex so that it will search for the string <code>"good"</code>. Then update the <code>replaceText</code> variable to replace <code>"good"</code> with <code>"okey-dokey"</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let huhText = "This sandwich is good.";
let fixRegex = /change/; // Change this line
let replaceText = ""; // Change this line
let result = huhText.replace(fixRegex, replaceText);
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

# 32. Remove Whitespace from Start and End

## Description
<section id='description'>
Sometimes whitespace characters around strings are not wanted but are there. Typical processing of strings is to remove the whitespace at the start and end of it.
</section>

## Instructions
<section id='instructions'>
Write a regex and use the appropriate string methods to remove whitespace at the beginning and end of strings.
<strong>Note</strong><br>The <code>.trim()</code> method would work here, but you'll need to complete this challenge using regular expressions.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let hello = "   Hello, World!  ";
let wsRegex = /change/; // Change this line
let result = hello; // Change this line
```

</div>



</section>

## Solution
<section id='solution'>

```js
let hello = "   Hello, World!  ";
let wsRegex = /^(\s+)(.+[^\s])(\s+)$/;
let result = hello.replace(wsRegex, '$2');
```
</section>
<hr>

# Debugging
# 1. Use the JavaScript Console to Check the Value of a Variable

## Description
<section id='description'>
Both Chrome and Firefox have excellent JavaScript consoles, also known as DevTools, for debugging your JavaScript.
You can find Developer tools in your Chrome's menu or Web Console in Firefox's menu. If you're using a different browser, or a mobile phone, we strongly recommend switching to desktop Firefox or Chrome.
The <code>console.log()</code> method, which "prints" the output of what's within its parentheses to the console, will likely be the most helpful debugging tool. Placing it at strategic points in your code can show you the intermediate values of variables. It's good practice to have an idea of what the output should be before looking at what it is. Having check points to see the status of your calculations throughout your code will help narrow down where the problem is.
Here's an example to print 'Hello world!' to the console:
<code>console.log('Hello world!');</code>
</section>

## Instructions
<section id='instructions'>
Use the <code>console.log()</code> method to print the value of the variable <code>a</code> where noted in the code.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let a = 5;
let b = 1;
a++;
// Add your code below this line


let sumAB = a + b;
console.log(sumAB);
```

</div>



</section>

## Solution
<section id='solution'>


```js
var a = 5; console.log(a);
```

</section>
<hr>

# 2. Understanding the Differences between the freeCodeCamp and Browser Console

## Description
<section id='description'>
You may have noticed that some freeCodeCamp JavaScript challenges include their own console.  This console behaves a little differently than the browser console you used in the last challenge.
The following challenge is meant to highlight some of the differences between the freeCodeCamp console and the browser console.
First, the browser console.  When you load and run an ordinary JavaScript file in your browser the <code>console.log()</code> statements will print exactly what you tell them to print to the browser console the exact number of times you requested. In your in-browser text editor the process is slightly different and can be confusing at first.
Values passed to <code>console.log()</code> in the text editor block run each set of tests as well as one more time for any function calls that you have in your code.
This lends itself to some interesting behavior and might trip you up in the beginning, because a logged value that you expect to see only once may print out many more times depending on the number of tests and the values being passed to those tests.
If you would like to see only your single output and not have to worry about running through the test cycles, you can use <code>console.clear()</code>.
</section>

## Instructions
<section id='instructions'>
Use <code>console.log()</code> to print the variables in the code where indicated.

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// Open your browser console
let outputTwo = "This will print to the browser console 2 times";
// Use console.log() to print the outputTwo variable


let outputOne = "Try to get this to log only once to the browser console";
// Use console.clear() in the next line to print the outputOne only once


// Use console.log() to print the outputOne variable


```

</div>



</section>

## Solution
<section id='solution'>


```js
let outputTwo = "This will print to the browser console 2 times"; console.log(outputTwo); let outputOne = "Try to get this to log only once to the browser console";
console.clear();
console.log(outputOne);
```

</section>
<hr>

# 3. Use typeof to Check the Type of a Variable

## Description
<section id='description'>
You can use <code>typeof</code> to check the data structure, or type, of a variable. This is useful in debugging when working with multiple data types. If you think you're adding two numbers, but one is actually a string, the results can be unexpected. Type errors can lurk in calculations or function calls. Be careful especially when you're accessing and working with external data in the form of a JavaScript Object Notation (JSON) object.
Here are some examples using <code>typeof</code>:
<blockquote>console.log(typeof ""); // outputs "string"<br>console.log(typeof 0); // outputs "number"<br>console.log(typeof []); // outputs "object"<br>console.log(typeof {}); // outputs "object"</blockquote>
JavaScript recognizes six primitive (immutable) data types: <code>Boolean</code>, <code>Null</code>, <code>Undefined</code>, <code>Number</code>, <code>String</code>, and <code>Symbol</code> (new with ES6) and one type for mutable items: <code>Object</code>. Note that in JavaScript, arrays are technically a type of object.
</section>

## Instructions
<section id='instructions'>
Add two <code>console.log()</code> statements to check the <code>typeof</code> each of the two variables <code>seven</code> and <code>three</code> in the code.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let seven = 7;
let three = "3";
console.log(seven + three);
// Add your code below this line

```

</div>



</section>

## Solution
<section id='solution'>


```js
let seven = 7;let three = "3";console.log(typeof seven);
console.log(typeof three);
```

</section>
<hr>

# 4. Catch Misspelled Variable and Function Names

## Description
<section id='description'>
The <code>console.log()</code> and <code>typeof</code> methods are the two primary ways to check intermediate values and types of program output. Now it's time to get into the common forms that bugs take. One syntax-level issue that fast typers can commiserate with is the humble spelling error.
Transposed, missing, or mis-capitalized characters in a variable or function name will have the browser looking for an object that doesn't exist - and complain in the form of a reference error. JavaScript variable and function names are case-sensitive.
</section>

## Instructions
<section id='instructions'>
Fix the two spelling errors in the code so the <code>netWorkingCapital</code> calculation works.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let receivables = 10;
let payables = 8;
let netWorkingCapital = recievables - payable;
console.log(`Net working capital is: ${netWorkingCapital}`);
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

# 5. Catch Unclosed Parentheses, Brackets, Braces and Quotes

## Description
<section id='description'>
Another syntax error to be aware of is that all opening parentheses, brackets, curly braces, and quotes have a closing pair. Forgetting a piece tends to happen when you're editing existing code and inserting items with one of the pair types. Also, take care when nesting code blocks into others, such as adding a callback function as an argument to a method.
One way to avoid this mistake is as soon as the opening character is typed, immediately include the closing match, then move the cursor back between them and continue coding. Fortunately, most modern code editors generate the second half of the pair automatically.
</section>

## Instructions
<section id='instructions'>
Fix the two pair errors in the code.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let myArray = [1, 2, 3;
let arraySum = myArray.reduce((previous, current =>  previous + current);
console.log(`Sum of array values is: ${arraySum}`);
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

# 6. Catch Mixed Usage of Single and Double Quotes

## Description
<section id='description'>
JavaScript allows the use of both single ('') and double ("") quotes to declare a string. Deciding which one to use generally comes down to personal preference, with some exceptions.
Having two choices is great when a string has contractions or another piece of text that's in quotes. Just be careful that you don't close the string too early, which causes a syntax error.
Here are some examples of mixing quotes:
<blockquote>// These are correct:<br>const grouchoContraction = "I've had a perfectly wonderful evening, but this wasn't it.";<br>const quoteInString = "Groucho Marx once said 'Quote me as saying I was mis-quoted.'";<br>// This is incorrect:<br>const uhOhGroucho = 'I've had a perfectly wonderful evening, but this wasn't it.';</blockquote>
Of course, it is okay to use only one style of quotes. You can escape the quotes inside the string by using the backslash (\) escape character:
<blockquote>// Correct use of same quotes:<br>const allSameQuotes = 'I\'ve had a perfectly wonderful evening, but this wasn\'t it.';</blockquote>
</section>

## Instructions
<section id='instructions'>
Fix the string so it either uses different quotes for the <code>href</code> value, or escape the existing ones. Keep the double quote marks around the entire string.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let innerHtml = "<p>Click here to <a href="#Home">return home</a></p>";
console.log(innerHtml);
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

# 7. Catch Use of Assignment Operator Instead of Equality Operator

## Description
<section id='description'>
Branching programs, i.e. ones that do different things if certain conditions are met, rely on <code>if</code>, <code>else if</code>, and <code>else</code> statements in JavaScript. The condition sometimes takes the form of testing whether a result is equal to a value.
This logic is spoken (in English, at least) as "if x equals y, then ..." which can literally translate into code using the <code>=</code>, or assignment operator. This leads to unexpected control flow in your program.
As covered in previous challenges, the assignment operator (<code>=</code>) in JavaScript assigns a value to a variable name. And the <code>==</code> and <code>===</code> operators check for equality (the triple <code>===</code> tests for strict equality, meaning both value and type are the same).
The code below assigns <code>x</code> to be 2, which evaluates as <code>true</code>. Almost every value on its own in JavaScript evaluates to <code>true</code>, except what are known as the "falsy" values: <code>false</code>, <code>0</code>, <code>""</code> (an empty string), <code>NaN</code>, <code>undefined</code>, and <code>null</code>.
<blockquote>let x = 1;<br>let y = 2;<br>if (x = y) {<br>&nbsp;&nbsp;// this code block will run for any value of y (unless y were originally set as a falsy)<br>} else {<br>&nbsp;&nbsp;// this code block is what should run (but won't) in this example<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Fix the condition so the program runs the right branch, and the appropriate value is assigned to <code>result</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let x = 7;
let y = 9;
let result = "to come";

if(x = y) {
  result = "Equal!";
} else {
  result = "Not equal!";
}

console.log(result);
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

# 8. Catch Missing Open and Closing Parenthesis After a Function Call

## Description
<section id='description'>
When a function or method doesn't take any arguments, you may forget to include the (empty) opening and closing parentheses when calling it. Often times the result of a function call is saved in a variable for other use in your code. This error can be detected by logging variable values (or their types) to the console and seeing that one is set to a function reference, instead of the expected value the function returns.
The variables in the following example are different:
<blockquote>function myFunction() {<br>&nbsp;&nbsp;return "You rock!";<br>}<br>let varOne = myFunction; // set to equal a function<br>let varTwo = myFunction(); // set to equal the string "You rock!"</blockquote>
</section>

## Instructions
<section id='instructions'>
Fix the code so the variable <code>result</code> is set to the value returned from calling the function <code>getNine</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function getNine() {
  let x = 6;
  let y = 3;
  return x + y;
}

let result = getNine;
console.log(result);
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

# 9. Catch Arguments Passed in the Wrong Order When Calling a Function

## Description
<section id='description'>
Continuing the discussion on calling functions, the next bug to watch out for is when a function's arguments are supplied in the incorrect order. If the arguments are different types, such as a function expecting an array and an integer, this will likely throw a runtime error. If the arguments are the same type (all integers, for example), then the logic of the code won't make sense. Make sure to supply all required arguments, in the proper order to avoid these issues.
</section>

## Instructions
<section id='instructions'>
The function <code>raiseToPower</code> raises a base to an exponent. Unfortunately, it's not called properly - fix the code so the value of <code>power</code> is the expected 8.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function raiseToPower(b, e) {
  return Math.pow(b, e);
}

let base = 2;
let exp = 3;
let power = raiseToPower(exp, base);
console.log(power);
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

# 10. Catch Off By One Errors When Using Indexing

## Description
<section id='description'>
<code>Off by one errors</code> (sometimes called OBOE) crop up when you're trying to target a specific index of a string or array (to slice or access a segment), or when looping over the indices of them. JavaScript indexing starts at zero, not one, which means the last index is always one less than the length of the item. If you try to access an index equal to the length, the program may throw an "index out of range" reference error or print <code>undefined</code>.
When you use string or array methods that take index ranges as arguments, it helps to read the documentation and understand if they are inclusive (the item at the given index is part of what's returned) or not. Here are some examples of off by one errors:
<blockquote>let alphabet = "abcdefghijklmnopqrstuvwxyz";<br>let len = alphabet.length;<br>for (let i = 0; i <= len; i++) {<br>&nbsp;&nbsp;// loops one too many times at the end<br>&nbsp;&nbsp;console.log(alphabet[i]);<br>}<br>for (let j = 1; j < len; j++) {<br>&nbsp;&nbsp;// loops one too few times and misses the first character at index 0<br>&nbsp;&nbsp;console.log(alphabet[j]);<br>}<br>for (let k = 0; k < len; k++) {<br>&nbsp;&nbsp;// Goldilocks approves - this is just right<br>&nbsp;&nbsp;console.log(alphabet[k]);<br>}</blockquote>
</section>

## Instructions
<section id='instructions'>
Fix the two indexing errors in the following function so all the numbers 1 through 5 are printed to the console.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function countToFive() {
  let firstFive = "12345";
  let len = firstFive.length;
  // Fix the line below
  for (let i = 1; i <= len; i++) {
  // Do not alter code below this line
    console.log(firstFive[i]);
  }
}

countToFive();
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

# 11. Use Caution When Reinitializing Variables Inside a Loop

## Description
<section id='description'>
Sometimes it's necessary to save information, increment counters, or re-set variables within a loop. A potential issue is when variables either should be reinitialized, and aren't, or vice versa. This is particularly dangerous if you accidentally reset the variable being used for the terminal condition, causing an infinite loop.
Printing variable values with each cycle of your loop by using <code>console.log()</code> can uncover buggy behavior related to resetting, or failing to reset a variable.
</section>

## Instructions
<section id='instructions'>
The following function is supposed to create a two-dimensional array with <code>m</code> rows and <code>n</code> columns of zeroes. Unfortunately, it's not producing the expected output because the <code>row</code> variable isn't being reinitialized (set back to an empty array) in the outer loop. Fix the code so it returns a correct 3x2 array of zeroes, which looks like <code>[[0, 0], [0, 0], [0, 0]]</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function zeroArray(m, n) {
  // Creates a 2-D array with m rows and n columns of zeroes
  let newArray = [];
  let row = [];
  for (let i = 0; i < m; i++) {
    // Adds the m-th row into newArray

    for (let j = 0; j < n; j++) {
      // Pushes n zeroes into the current row to create the columns
      row.push(0);
    }
    // Pushes the current row, which now has n zeroes in it, to the array
    newArray.push(row);
  }
  return newArray;
}

let matrix = zeroArray(3, 2);
console.log(matrix);
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

# 12. Prevent Infinite Loops with a Valid Terminal Condition

## Description
<section id='description'>
The final topic is the dreaded infinite loop. Loops are great tools when you need your program to run a code block a certain number of times or until a condition is met, but they need a terminal condition that ends the looping. Infinite loops are likely to freeze or crash the browser, and cause general program execution mayhem, which no one wants.
There was an example of an infinite loop in the introduction to this section - it had no terminal condition to break out of the <code>while</code> loop inside <code>loopy()</code>. Do NOT call this function!
<blockquote>function loopy() {<br>&nbsp;&nbsp;while(true) {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("Hello, world!");<br>&nbsp;&nbsp;}<br>}</blockquote>
It's the programmer's job to ensure that the terminal condition, which tells the program when to break out of the loop code, is eventually reached. One error is incrementing or decrementing a counter variable in the wrong direction from the terminal condition. Another one is accidentally resetting a counter or index variable within the loop code, instead of incrementing or decrementing it.
</section>

## Instructions
<section id='instructions'>
The <code>myFunc()</code> function contains an infinite loop because the terminal condition <code>i != 4</code> will never evaluate to <code>false</code> (and break the looping) - <code>i</code> will increment by 2 each pass, and jump right over 4 since <code>i</code> is odd to start. Fix the comparison operator in the terminal condition so the loop only runs for <code>i</code> less than or equal to 4.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function myFunc() {
  for (let i = 1; i != 4; i += 2) {
    console.log("Still going!");
  }
}
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

# Basic Data Structures
# 1. Use an Array to Store a Collection of Data

## Description
<section id='description'>
The below is an example of the simplest implementation of an array data structure. This is known as a <dfn>one-dimensional array</dfn>, meaning it only has one level, or that it does not have any other arrays nested within it. Notice it contains <dfn>booleans</dfn>, <dfn>strings</dfn>, and <dfn>numbers</dfn>, among other valid JavaScript data types:
<blockquote>let simpleArray = ['one', 2, 'three’, true, false, undefined, null];<br>console.log(simpleArray.length);<br>// logs 7</blockquote>
All arrays have a length property, which as shown above, can be very easily accessed with the syntax <code>Array.length</code>.
A more complex implementation of an array can be seen below. This is known as a <dfn>multi-dimensional array</dfn>, or an array that contains other arrays. Notice that this array also contains JavaScript <dfn>objects</dfn>, which we will examine very closely in our next section, but for now, all you need to know is that arrays are also capable of storing complex objects.
<blockquote>let complexArray = [<br>&nbsp;&nbsp;[<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;one: 1,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;two: 2<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;three: 3,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;four: 4<br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;],<br>&nbsp;&nbsp;[<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a: "a",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;b: "b"<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;c: "c",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;d: “d”<br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;]<br>];</blockquote>
</section>

## Instructions
<section id='instructions'>
We have defined a variable called <code>yourArray</code>. Complete the statement by assigning an array of at least 5 elements in length to the <code>yourArray</code> variable. Your array should contain at least one <dfn>string</dfn>, one <dfn>number</dfn>, and one <dfn>boolean</dfn>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let yourArray; // change this line
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

# 2. Access an Array's Contents Using Bracket Notation

## Description
<section id='description'>
The fundamental feature of any data structure is, of course, the ability to not only store data, but to be able to retrieve that data on command. So, now that we've learned how to create an array, let's begin to think about how we can access that array's information.
When we define a simple array as seen below, there are 3 items in it:
<blockquote>let ourArray = ["a", "b", "c"];</blockquote>
In an array, each array item has an <dfn>index</dfn>.  This index doubles as the position of that item in the array, and how you reference it. However, it is important to note, that JavaScript arrays are <dfn>zero-indexed</dfn>, meaning that the first element of an array is actually at the <em><strong>zeroth</strong></em> position, not the first.
In order to retrieve an element from an array we can enclose an index in brackets and append it to the end of an array, or more commonly, to a variable which references an array object. This is known as <dfn>bracket notation</dfn>.
For example, if we want to retrieve the <code>"a"</code> from <code>ourArray</code> and assign it to a variable, we can do so with the following code:
<blockquote>let ourVariable = ourArray[0];<br>// ourVariable equals "a"</blockquote>
In addition to accessing the value associated with an index, you can also <em>set</em> an index to a value using the same notation:
<blockquote>ourArray[1] = "not b anymore";<br>// ourArray now equals ["a", "not b anymore", "c"];</blockquote>
Using bracket notation, we have now reset the item at index 1 from <code>"b"</code>, to <code>"not b anymore"</code>.
</section>

## Instructions
<section id='instructions'>
In order to complete this challenge, set the 2nd position (index <code>1</code>) of <code>myArray</code> to anything you want, besides <code>"b"</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let myArray = ["a", "b", "c", "d"];
// change code below this line

//change code above this line
console.log(myArray);
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

# 3. Add Items to an Array with push() and unshift()

## Description
<section id='description'>
An array's length, like the data types it can contain, is not fixed. Arrays can be defined with a length of any number of elements, and elements can be added or removed over time; in other words, arrays are <dfn>mutable</dfn>. In this challenge, we will look at two methods with which we can programmatically modify an array: <code>Array.push()</code> and <code>Array.unshift()</code>.
Both methods take one or more elements as parameters and add those elements to the array the method is being called on; the <code>push()</code> method adds elements to the end of an array, and <code>unshift()</code> adds elements to the beginning. Consider the following:
<blockquote>let twentyThree = 'XXIII';<br>let romanNumerals = ['XXI', 'XXII'];<br><br>romanNumerals.unshift('XIX', 'XX');<br>// now equals ['XIX', 'XX', 'XXI', 'XXII']<br><br>romanNumerals.push(twentyThree);<br>// now equals ['XIX', 'XX', 'XXI', 'XXII', 'XXIII']
Notice that we can also pass variables, which allows us even greater flexibility in dynamically modifying our array's data.
</section>

## Instructions
<section id='instructions'>
We have defined a function, <code>mixedNumbers</code>, which we are passing an array as an argument. Modify the function by using <code>push()</code> and <code>unshift()</code> to add <code>'I', 2, 'three'</code> to the beginning of the array and <code>7, 'VIII', 9</code> to the end so that the returned array contains representations of the numbers 1-9 in order.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function mixedNumbers(arr) {
  // change code below this line

  // change code above this line
  return arr;
}

// do not change code below this line
console.log(mixedNumbers(['IV', 5, 'six']));
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

# 4. Remove Items from an Array with pop() and shift()

## Description
<section id='description'>
Both <code>push()</code> and <code>unshift()</code> have corresponding methods that are nearly functional opposites: <code>pop()</code> and <code>shift()</code>. As you may have guessed by now, instead of adding, <code>pop()</code> <em>removes</em> an element from the end of an array, while <code>shift()</code> removes an element from the beginning. The key difference between <code>pop()</code> and <code>shift()</code> and their cousins <code>push()</code> and <code>unshift()</code>, is that neither method takes parameters, and each only allows an array to be modified by a single element at a time.
Let's take a look:
<blockquote>let greetings = ['whats up?', 'hello', 'see ya!'];<br><br>greetings.pop();<br>// now equals ['whats up?', 'hello']<br><br>greetings.shift();<br>// now equals ['hello']</blockquote>
We can also return the value of the removed element with either method like this:
<blockquote>let popped = greetings.pop();<br>// returns 'hello'<br>// greetings now equals []</blockquote>
</section>

## Instructions
<section id='instructions'>
We have defined a function, <code>popShift</code>, which takes an array as an argument and returns a new array. Modify the function, using <code>pop()</code> and <code>shift()</code>, to remove the first and last elements of the argument array, and assign the removed elements to their corresponding variables, so that the returned array contains their values.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function popShift(arr) {
  let popped; // change this line
  let shifted; // change this line
  return [shifted, popped];
}

// do not change code below this line
console.log(popShift(['challenge', 'is', 'not', 'complete']));
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

# 5. Remove Items Using splice()

## Description
<section id='description'>
Ok, so we've learned how to remove elements from the beginning and end of arrays using <code>shift()</code> and <code>pop()</code>, but what if we want to remove an element from somewhere in the middle? Or remove more than one element at once? Well, that's where <code>splice()</code> comes in. <code>splice()</code> allows us to do just that: <strong>remove any number of consecutive elements</strong> from anywhere in an array.
<code>splice()</code> can take up to 3 parameters, but for now, we'll focus on just the first 2. The first two parameters of <code>splice()</code> are integers which represent indexes, or positions, of the array that <code>splice()</code> is being called upon. And remember, arrays are <em>zero-indexed</em>, so to indicate the first element of an array, we would use <code>0</code>. <code>splice()</code>'s first parameter represents the index on the array from which to begin removing elements, while the second parameter indicates the number of elements to delete. For example:
<blockquote>let array = ['today', 'was', 'not', 'so', 'great'];<br><br>array.splice(2, 2);<br>// remove 2 elements beginning with the 3rd element<br>// array now equals ['today', 'was', 'great']</blockquote>
<code>splice()</code> not only modifies the array it's being called on, but it also returns a new array containing the value of the removed elements:
<blockquote>let array = ['I', 'am', 'feeling', 'really', 'happy'];<br><br>let newArray = array.splice(3, 2);<br>// newArray equals ['really', 'happy']</blockquote>
</section>

## Instructions
<section id='instructions'>
We've defined a function, <code>sumOfTen</code>, which takes an array as an argument and returns the sum of that array's elements. Modify the function, using <code>splice()</code>, so that it returns a value of <code>10</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function sumOfTen(arr) {
  // change code below this line

  // change code above this line
  return arr.reduce((a, b) => a + b);
}

// do not change code below this line
console.log(sumOfTen([2, 5, 1, 5, 2, 1]));
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

# 6. Add Items Using splice()

## Description
<section id='description'>
Remember in the last challenge we mentioned that <code>splice()</code> can take up to three parameters? Well, we can go one step further with <code>splice()</code> &mdash; in addition to removing elements, we can use that third parameter, which represents one or more elements, to <em>add</em> them as well. This can be incredibly useful for quickly switching out an element, or a set of elements, for another. For instance, let's say you're storing a color scheme for a set of DOM elements in an array, and want to dynamically change a color based on some action:
<blockquote>function colorChange(arr, index, newColor) {<br>&nbsp;&nbsp;arr.splice(index, 1, newColor);<br>&nbsp;&nbsp;return arr;<br>}<br><br>let colorScheme = ['#878787', '#a08794', '#bb7e8c', '#c9b6be', '#d1becf'];<br><br>colorScheme = colorChange(colorScheme, 2, '#332327');<br>// we have removed '#bb7e8c' and added '#332327' in its place<br>// colorScheme now equals ['#878787', '#a08794', '#332327', '#c9b6be', '#d1becf']</blockquote>
This function takes an array of hex values, an index at which to remove an element, and the new color to replace the removed element with. The return value is an array containing a newly modified color scheme! While this example is a bit oversimplified, we can see the value that utilizing <code>splice()</code> to its maximum potential can have.
</section>

## Instructions
<section id='instructions'>
We have defined a function, <code>htmlColorNames</code>, which takes an array of HTML colors as an argument. Modify the function using <code>splice()</code> to remove the first two elements of the array and add <code>'DarkSalmon'</code> and <code>'BlanchedAlmond'</code> in their respective places.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function htmlColorNames(arr) {
  // change code below this line

  // change code above this line
  return arr;
}

// do not change code below this line
console.log(htmlColorNames(['DarkGoldenRod', 'WhiteSmoke', 'LavenderBlush', 'PaleTurqoise', 'FireBrick']));
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

# 7. Copy Array Items Using slice()

## Description
<section id='description'>
The next method we will cover is <code>slice()</code>. <code>slice()</code>, rather than modifying an array, copies, or <em>extracts</em>, a given number of elements to a new array, leaving the array it is called upon untouched. <code>slice()</code> takes only 2 parameters &mdash; the first is the index at which to begin extraction, and the second is the index at which to stop extraction (extraction will occur up to, but not including the element at this index). Consider this:
<blockquote>let weatherConditions = ['rain', 'snow', 'sleet', 'hail', 'clear'];<br><br>let todaysWeather = weatherConditions.slice(1, 3);<br>// todaysWeather equals ['snow', 'sleet'];<br>// weatherConditions still equals ['rain', 'snow', 'sleet', 'hail', 'clear']<br></blockquote>
In effect, we have created a new array by extracting elements from an existing array.
</section>

## Instructions
<section id='instructions'>
We have defined a function, <code>forecast</code>, that takes an array as an argument. Modify the function using <code>slice()</code> to extract information from the argument array and return a new array that contains the elements <code>'warm'</code> and <code>'sunny'</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function forecast(arr) {
  // change code below this line

  return arr;
}

// do not change code below this line
console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));
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

# 8. Copy an Array with the Spread Operator

## Description
<section id='description'>
While <code>slice()</code> allows us to be selective about what elements of an array to copy, among several other useful tasks, ES6's new <dfn>spread operator</dfn> allows us to easily copy <em>all</em> of an array's elements, in order, with a simple and highly readable syntax. The spread syntax simply looks like this: <code>...</code>
In practice, we can use the spread operator to copy an array like so:
<blockquote>let thisArray = [true, true, undefined, false, null];<br>let thatArray = [...thisArray];<br>// thatArray equals [true, true, undefined, false, null]<br>// thisArray remains unchanged, and is identical to thatArray</blockquote>
</section>

## Instructions
<section id='instructions'>
We have defined a function, <code>copyMachine</code> which takes <code>arr</code> (an array) and <code>num</code> (a number) as arguments. The function is supposed to return a new array made up of <code>num</code> copies of <code>arr</code>. We have done most of the work for you, but it doesn't work quite right yet. Modify the function using spread syntax so that it works correctly (hint: another method we have already covered might come in handy here!).
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function copyMachine(arr, num) {
  let newArr = [];
  while (num >= 1) {
    // change code below this line

    // change code above this line
    num--;
  }
  return newArr;
}

// change code here to test different cases:
console.log(copyMachine([true, false, true], 2));
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

# 9. Combine Arrays with the Spread Operator

## Description
<section id='description'>
Another huge advantage of the <dfn>spread</dfn> operator, is the ability to combine arrays, or to insert all the elements of one array into another, at any index. With more traditional syntaxes, we can concatenate arrays, but this only allows us to combine arrays at the end of one, and at the start of another. Spread syntax makes the following operation extremely simple:
<blockquote>let thisArray = ['sage', 'rosemary', 'parsley', 'thyme'];<br><br>let thatArray = ['basil', 'cilantro', ...thisArray, 'coriander'];<br>// thatArray now equals ['basil', 'cilantro', 'sage', 'rosemary', 'parsley', 'thyme', 'coriander']</blockquote>
Using spread syntax, we have just achieved an operation that would have been more complex and more verbose had we used traditional methods.
</section>

## Instructions
<section id='instructions'>
We have defined a function <code>spreadOut</code> that returns the variable <code>sentence</code>. Modify the function using the <dfn>spread</dfn> operator so that it returns the array <code>['learning', 'to', 'code', 'is', 'fun']</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function spreadOut() {
  let fragment = ['to', 'code'];
  let sentence; // change this line
  return sentence;
}

// do not change code below this line
console.log(spreadOut());
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

# 10. Check For The Presence of an Element With indexOf()

## Description
<section id='description'>
Since arrays can be changed, or <em>mutated</em>, at any time, there's no guarantee about where a particular piece of data will be on a given array, or if that element even still exists. Luckily, JavaScript provides us with another built-in method, <code>indexOf()</code>, that allows us to quickly and easily check for the presence of an element on an array. <code>indexOf()</code> takes an element as a parameter, and when called, it returns the position, or index, of that element, or <code>-1</code> if the element does not exist on the array.
For example:
<blockquote>let fruits = ['apples', 'pears', 'oranges', 'peaches', 'pears'];<br><br>fruits.indexOf('dates') // returns -1<br>fruits.indexOf('oranges') // returns 2<br>fruits.indexOf('pears') // returns 1, the first index at which the element exists</blockquote>
</section>

## Instructions
<section id='instructions'>
<code>indexOf()</code> can be incredibly useful for quickly checking for the presence of an element on an array. We have defined a function, <code>quickCheck</code>, that takes an array and an element as arguments. Modify the function using <code>indexOf()</code> so that it returns <code>true</code> if the passed element exists on the array, and <code>false</code> if it does not.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function quickCheck(arr, elem) {
  // change code below this line

  // change code above this line
}

// change code here to test different cases:
console.log(quickCheck(['squash', 'onions', 'shallots'], 'mushrooms'));
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

# 11. Iterate Through All an Array's Items Using For Loops

## Description
<section id='description'>
Sometimes when working with arrays, it is very handy to be able to iterate through each item to find one or more elements that we might need, or to manipulate an array based on which data items meet a certain set of criteria. JavaScript offers several built in methods that each iterate over arrays in slightly different ways to achieve different results (such as <code>every()</code>, <code>forEach()</code>, <code>map()</code>, etc.), however the technique which is most flexible and offers us the greatest amount of control is a simple <code>for</code> loop.
Consider the following:
<blockquote>function greaterThanTen(arr) {<br>&nbsp;&nbsp;let newArr = [];<br>&nbsp;&nbsp;for (let i = 0; i < arr.length; i++) {<br>&nbsp;&nbsp;&nbsp;&nbsp;if (arr[i] > 10) {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;newArr.push(arr[i]);<br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;}<br>&nbsp;&nbsp;return newArr;<br>}<br><br>greaterThanTen([2, 12, 8, 14, 80, 0, 1]);<br>// returns [12, 14, 80]</blockquote>
Using a <code>for</code> loop, this function iterates through and accesses each element of the array, and subjects it to a simple test that we have created. In this way, we have easily and programmatically determined which data items are greater than <code>10</code>, and returned a new array containing those items.
</section>

## Instructions
<section id='instructions'>
We have defined a function, <code>filteredArray</code>, which takes <code>arr</code>, a nested array, and <code>elem</code> as arguments, and returns a new array. <code>elem</code> represents an element that may or may not be present on one or more of the arrays nested within <code>arr</code>. Modify the function, using a <code>for</code> loop, to return a filtered version of the passed array such that any array nested within <code>arr</code> containing <code>elem</code> has been removed.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function filteredArray(arr, elem) {
  let newArr = [];
  // change code below this line

  // change code above this line
  return newArr;
}

// change code here to test different cases:
console.log(filteredArray([[3, 2, 3], [1, 6, 3], [3, 13, 26], [19, 3, 9]], 3));
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

# 12. Create complex multi-dimensional arrays

## Description
<section id='description'>
Awesome! You have just learned a ton about arrays! This has been a fairly high level overview, and there is plenty more to learn about working with arrays, much of which you will see in later sections. But before moving on to looking at <dfn>Objects</dfn>, lets take one more look, and see how arrays can become a bit more complex than what we have seen in previous challenges.
One of the most powerful features when thinking of arrays as data structures, is that arrays can contain, or even be completely made up of other arrays. We have seen arrays that contain arrays in previous challenges, but fairly simple ones. However, arrays can contain an infinite depth of arrays that can contain other arrays, each with their own arbitrary levels of depth, and so on. In this way, an array can very quickly become very complex data structure, known as a <dfn>multi-dimensional</dfn>, or nested array. Consider the following example:
<blockquote>let nestedArray = [ // top, or first level - the outer most array<br>&nbsp;&nbsp;['deep'], // an array within an array, 2 levels of depth<br>&nbsp;&nbsp;[<br>&nbsp;&nbsp;&nbsp;&nbsp;['deeper'], ['deeper'] // 2 arrays nested 3 levels deep<br>&nbsp;&nbsp;],<br>&nbsp;&nbsp;[<br>&nbsp;&nbsp;&nbsp;&nbsp;[<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;['deepest'], ['deepest'] // 2 arrays nested 4 levels deep<br>&nbsp;&nbsp;&nbsp;&nbsp;],<br>&nbsp;&nbsp;&nbsp;&nbsp;[<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;['deepest-est?'] // an array nested 5 levels deep<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;]<br>&nbsp;&nbsp;&nbsp;&nbsp;]<br>&nbsp;&nbsp;]<br>];</blockquote>
While this example may seem convoluted, this level of complexity is not unheard of, or even unusual, when dealing with large amounts of data.
However, we can still very easily access the deepest levels of an array this complex with bracket notation:
<blockquote>console.log(nestedArray[2][1][0][0][0]);<br>// logs: deepest-est?</blockquote>
And now that we know where that piece of data is, we can reset it if we need to:
<blockquote>nestedArray[2][1][0][0][0] = 'deeper still';<br><br>console.log(nestedArray[2][1][0][0][0]);<br>// now logs: deeper still</blockquote>
</section>

## Instructions
<section id='instructions'>
We have defined a variable, <code>myNestedArray</code>, set equal to an array. Modify <code>myNestedArray</code>, using any combination of <dfn>strings</dfn>, <dfn>numbers</dfn>, and <dfn>booleans</dfn> for data elements, so that it has exactly five levels of depth (remember, the outer-most array is level 1). Somewhere on the third level, include the string <code>'deep'</code>, on the fourth level, include the string <code>'deeper'</code>, and on the fifth level, include the string <code>'deepest'</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let myNestedArray = [
  // change code below this line
  ['unshift', false, 1, 2, 3, 'complex', 'nested'],
  ['loop', 'shift', 6, 7, 1000, 'method'],
  ['concat', false, true, 'spread', 'array'],
  ['mutate', 1327.98, 'splice', 'slice', 'push'],
  ['iterate', 1.3849, 7, '8.4876', 'arbitrary', 'depth']
  // change code above this line
];
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

# 13. Add Key-Value Pairs to JavaScript Objects

## Description
<section id='description'>
At their most basic, objects are just collections of <dfn>key-value pairs</dfn>, or in other words, pieces of data mapped to unique identifiers that we call <dfn>properties</dfn> or <dfn>keys</dfn>. Let's take a look at a very simple example:
<blockquote>let FCC_User = {<br>&nbsp;&nbsp;username: 'awesome_coder',<br>&nbsp;&nbsp;followers: 572,<br>&nbsp;&nbsp;points: 1741,<br>&nbsp;&nbsp;completedProjects: 15<br>};</blockquote>
The above code defines an object called <code>FCC_User</code> that has four <dfn>properties</dfn>, each of which map to a specific value. If we wanted to know the number of <code>followers</code> <code>FCC_User</code> has, we can access that property by writing:
<blockquote>let userData = FCC_User.followers;<br>// userData equals 572</blockquote>
This is called <dfn>dot notation</dfn>. Alternatively, we can also access the property with brackets, like so:
<blockquote>let userData = FCC_User['followers']<br>// userData equals 572</blockquote>
Notice that with <dfn>bracket notation</dfn>, we enclosed <code>followers</code> in quotes. This is because the brackets actually allow us to pass a variable in to be evaluated as a property name (hint: keep this in mind for later!). Had we passed <code>followers</code> in without the quotes, the JavaScript engine would have attempted to evaluate it as a variable, and a <code>ReferenceError: followers is not defined</code> would have been thrown.
</section>

## Instructions
<section id='instructions'>
Using the same syntax, we can also <em><strong>add new</strong></em> key-value pairs to objects. We've created a <code>foods</code> object with three entries. Add three more entries: <code>bananas</code> with a value of <code>13</code>, <code>grapes</code> with a value of <code>35</code>, and <code>strawberries</code> with a value of <code>27</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28
};

// change code below this line

// change code above this line

console.log(foods);
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

# 14. Modify an Object Nested Within an Object

## Description
<section id='description'>
Now let's take a look at a slightly more complex object. Object properties can be nested to an arbitrary depth, and their values can be any type of data supported by JavaScript, including arrays and even other objects. Consider the following:
<blockquote>let nestedObject = {<br>&nbsp;&nbsp;id: 28802695164,<br>&nbsp;&nbsp;date: 'December 31, 2016',<br>&nbsp;&nbsp;data: {<br>&nbsp;&nbsp;&nbsp;&nbsp;totalUsers: 99,<br>&nbsp;&nbsp;&nbsp;&nbsp;online: 80,<br>&nbsp;&nbsp;&nbsp;&nbsp;onlineStatus: {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;active: 67,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;away: 13<br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;}<br>};</blockquote>
<code>nestedObject</code> has three unique keys: <code>id</code>, whose value is a number, <code>date</code> whose value is a string, and <code>data</code>, whose value is an object which has yet another object nested within it. While structures can quickly become complex, we can still use the same notations to access the information we need.
</section>

## Instructions
<section id='instructions'>
Here we've defined an object, <code>userActivity</code>, which includes another object nested within it. You can modify properties on this nested object in the same way you modified properties in the last challenge. Set the value of the <code>online</code> key to <code>45</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let userActivity = {
  id: 23894201352,
  date: 'January 1, 2017',
  data: {
    totalUsers: 51,
    online: 42
  }
};

// change code below this line

// change code above this line

console.log(userActivity);
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

# 15. Access Property Names with Bracket Notation

## Description
<section id='description'>
In the first object challenge we mentioned the use of bracket notation as a way to access property values using the evaluation of a variable. For instance, imagine that our <code>foods</code> object is being used in a program for a supermarket cash register. We have some function that sets the <code>selectedFood</code> and we want to check our <code>foods</code> object for the presence of that food. This might look like:
<blockquote>let selectedFood = getCurrentFood(scannedItem);<br>let inventory = foods[selectedFood];</blockquote>
This code will evaluate the value stored in the <code>selectedFood</code> variable and return the value of that key in the <code>foods</code> object, or <code>undefined</code> if it is not present. Bracket notation is very useful because sometimes object properties are not known before runtime or we need to access them in a more dynamic way.
</section>

## Instructions
<section id='instructions'>
We've defined a function, <code>checkInventory</code>, which receives a scanned item as an argument. Return the current value of the <code>scannedItem</code> key in the <code>foods</code> object. You can assume that only valid keys will be provided as an argument to <code>checkInventory</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
};
// do not change code above this line

function checkInventory(scannedItem) {
  // change code below this line

}

// change code below this line to test different cases:
console.log(checkInventory("apples"));
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

# 16. Use the delete Keyword to Remove Object Properties

## Description
<section id='description'>
Now you know what objects are and their basic features and advantages. In short, they are key-value stores which provide a flexible, intuitive way to structure data, <strong><em>and</em></strong>, they provide very fast lookup time. Throughout the rest of these challenges, we will describe several common operations you can perform on objects so you can become comfortable applying these useful data structures in your programs.
In earlier challenges, we have both added to and modified an object's key-value pairs. Here we will see how we can <em>remove</em> a key-value pair from an object.
Let's revisit our <code>foods</code> object example one last time. If we wanted to remove the <code>apples</code> key, we can remove it by using the <code>delete</code> keyword like this:
<blockquote>delete foods.apples;</blockquote>
</section>

## Instructions
<section id='instructions'>
Use the delete keyword to remove the <code>oranges</code>, <code>plums</code>, and <code>strawberries</code> keys from the <code>foods</code> object.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
};

// change code below this line

// change code above this line

console.log(foods);
```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
let foods = {
  apples: 25,
  oranges: 32,
  plums: 28,
  bananas: 13,
  grapes: 35,
  strawberries: 27
};

delete foods.oranges;
delete foods.plums;
delete foods.strawberries;

console.log(foods);
```
</section>
<hr>

# 17. Check if an Object has a Property

## Description
<section id='description'>
Now we can add, modify, and remove keys from objects. But what if we just wanted to know if an object has a specific property? JavaScript provides us with two different ways to do this. One uses the <code>hasOwnProperty()</code> method and the other uses the <code>in</code> keyword. If we have an object <code>users</code> with a property of <code>Alan</code>, we could check for its presence in either of the following ways:
<blockquote>users.hasOwnProperty('Alan');<br>'Alan' in users;<br>// both return true</blockquote>
</section>

## Instructions
<section id='instructions'>
We've created an object, <code>users</code>, with some users in it and a function <code>isEveryoneHere</code>, which we pass the <code>users</code> object to as an argument. Finish writing this function so that it returns <code>true</code> only if the <code>users</code> object contains all four names, <code>Alan</code>, <code>Jeff</code>, <code>Sarah</code>, and <code>Ryan</code>, as keys, and <code>false</code> otherwise.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let users = {
  Alan: {
    age: 27,
    online: true
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: true
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function isEveryoneHere(obj) {
  // change code below this line

  // change code above this line
}

console.log(isEveryoneHere(users));
```

</div>



</section>

## Solution
<section id='solution'>

```js
let users = {
  Alan: {
    age: 27,
    online: true
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: true
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function isEveryoneHere(obj) {
  return [
    'Alan',
    'Jeff',
    'Sarah',
    'Ryan'
  ].every(i => obj.hasOwnProperty(i));
}

console.log(isEveryoneHere(users));
```
</section>
<hr>

# 18.  Iterate Through the Keys of an Object with a for...in Statement

## Description
<section id='description'>
Sometimes you may need to iterate through all the keys within an object. This requires a specific syntax in JavaScript called a <dfn>for...in</dfn> statement. For our <code>users</code> object, this could look like:
<blockquote>for (let user in users) {<br>&nbsp;&nbsp;console.log(user);<br>}<br><br>// logs:<br>Alan<br>Jeff<br>Sarah<br>Ryan</blockquote>
In this statement, we defined a variable <code>user</code>, and as you can see, this variable was reset during each iteration to each of the object's keys as the statement looped through the object, resulting in each user's name being printed to the console.
<strong>NOTE:</strong><br>Objects do not maintain an ordering to stored keys like arrays do; thus a key's position on an object, or the relative order in which it appears, is irrelevant when referencing or accessing that key.
</section>

## Instructions
<section id='instructions'>
We've defined a function, <code>countOnline</code>; use a <dfn>for...in</dfn> statement within this function to loop through the users in the <code>users</code> object and return the number of users whose <code>online</code> property is set to <code>true</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function countOnline(obj) {
  // change code below this line

  // change code above this line
}

console.log(countOnline(users));
```

</div>



</section>

## Solution
<section id='solution'>

```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function countOnline(obj) {
  let online = 0;
  for(let user in obj){
    if(obj[user].online == true) {
      online += 1;
    }
  }
  return online;
}

console.log(countOnline(users));
```
</section>
<hr>

# 19. Generate an Array of All Object Keys with Object.keys()

## Description
<section id='description'>
We can also generate an array which contains all the keys stored in an object using the <code>Object.keys()</code> method and passing in an object as the argument. This will return an array with strings representing each property in the object. Again, there will be no specific order to the entries in the array.
</section>

## Instructions
<section id='instructions'>
Finish writing the <code>getArrayOfUsers</code> function so that it returns an array containing all the properties in the object it receives as an argument.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function getArrayOfUsers(obj) {
  // change code below this line

  // change code above this line
}

console.log(getArrayOfUsers(users));
```

</div>



</section>

## Solution
<section id='solution'>

```js
let users = {
  Alan: {
    age: 27,
    online: false
  },
  Jeff: {
    age: 32,
    online: true
  },
  Sarah: {
    age: 48,
    online: false
  },
  Ryan: {
    age: 19,
    online: true
  }
};

function getArrayOfUsers(obj) {
  return Object.keys(users);
}

console.log(getArrayOfUsers(users));
```
</section>
<hr>

# 20. Modify an Array Stored in an Object

## Description
<section id='description'>
Now you've seen all the basic operations for JavaScript objects. You can add, modify, and remove key-value pairs, check if keys exist, and iterate over all the keys in an object. As you continue learning JavaScript you will see even more versatile applications of objects. Additionally, the optional Advanced Data Structures lessons later in the curriculum also cover the ES6 <dfn>Map</dfn> and <dfn>Set</dfn> objects, both of which are similar to ordinary objects but provide some additional features. Now that you've learned the basics of arrays and objects, you're fully prepared to begin tackling more complex problems using JavaScript!
</section>

## Instructions
<section id='instructions'>
Take a look at the object we've provided in the code editor. The <code>user</code> object contains three keys. The <code>data</code> key contains five keys, one of which contains an array of <code>friends</code>. From this, you can see how flexible objects are as data structures. We've started writing a function <code>addFriend</code>. Finish writing it so that it takes a <code>user</code> object and adds the name of the <code>friend</code> argument to the array stored in <code>user.data.friends</code> and returns that array.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let user = {
  name: 'Kenneth',
  age: 28,
  data: {
    username: 'kennethCodesAllDay',
    joinDate: 'March 26, 2016',
    organization: 'freeCodeCamp',
    friends: [
      'Sam',
      'Kira',
      'Tomo'
    ],
    location: {
      city: 'San Francisco',
      state: 'CA',
      country: 'USA'
    }
  }
};

function addFriend(userObj, friend) {
  // change code below this line

  // change code above this line
}

console.log(addFriend(user, 'Pete'));
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

# Basic Algorithm Scripting
# 1. Convert Celsius to Fahrenheit

## Description
<section id='description'>
The algorithm to convert from Celsius to Fahrenheit is the temperature in Celsius times <code>9/5</code>, plus <code>32</code>.
You are given a variable <code>celsius</code> representing a temperature in Celsius. Use the variable <code>fahrenheit</code> already defined and assign it the Fahrenheit temperature equivalent to the given Celsius temperature. Use the algorithm mentioned above to help convert the Celsius temperature to Fahrenheit.
Don't worry too much about the function and return statements as they will be covered in future challenges. For now, only use operators that you have already learned.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function convertToF(celsius) {
  let fahrenheit;
  return fahrenheit;
}

convertToF(30);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function convertToF(celsius) {
  let fahrenheit = celsius *9/5 + 32;

  return fahrenheit;
}

convertToF(30);

```

</section>
<hr>

# 2. Reverse a String

## Description
<section id='description'>
Reverse the provided string.
You may need to turn the string into an array before you can reverse it.
Your result must be a string.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function reverseString(str) {
  return str;
}

reverseString("hello");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function reverseString(str) {
  return str.split('').reverse().join('');
}

reverseString("hello");

```

</section>
<hr>

# 3. Factorialize a Number

## Description
<section id='description'>
Return the factorial of the provided integer.
If the integer is represented with the letter n, a factorial is the product of all positive integers less than or equal to n.
Factorials are often represented with the shorthand notation <code>n!</code>
For example: <code>5! = 1 *2 *3 *4 *5 = 120</code>
Only integers greater than or equal to zero will be supplied to the function.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function factorialize(num) {
  return num;
}

factorialize(5);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function factorialize(num) {
  return num < 1 ? 1 : num *factorialize(num - 1);
}

factorialize(5);

```

</section>
<hr>

# 4. Find the Longest Word in a String

## Description
<section id='description'>
Return the length of the longest word in the provided sentence.
Your response should be a number.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function findLongestWordLength(str) {
  return str.length;
}

findLongestWordLength("The quick brown fox jumped over the lazy dog");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function findLongestWordLength(str) {
  return str.split(' ').sort((a, b) => b.length - a.length)[0].length;
}

findLongestWordLength("The quick brown fox jumped over the lazy dog");

```

</section>
<hr>

# 5. Return Largest Numbers in Arrays

## Description
<section id='description'>
Return an array consisting of the largest number from each provided sub-array. For simplicity, the provided array will contain exactly 4 sub-arrays.
Remember, you can iterate through an array with a simple for loop, and access each member with array syntax <code>arr[i]</code>.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function largestOfFour(arr) {
  // You can do this!
  return arr;
}

largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function largestOfFour(arr) {
  return arr.map(subArr => Math.max.apply(null, subArr));
}

largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]);

```

</section>
<hr>

# 6. Confirm the Ending

## Description
<section id='description'>
Check if a string (first argument, <code>str</code>) ends with the given target string (second argument, <code>target</code>).
This challenge <em>can</em> be solved with the <code>.endsWith()</code> method, which was introduced in ES2015. But for the purpose of this challenge, we would like you to use one of the JavaScript substring methods instead.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function confirmEnding(str, target) {
  // "Never give up and good luck will find you."
  // -- Falcor
  return str;
}

confirmEnding("Bastian", "n");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function confirmEnding(str, target) {
  return str.substring(str.length - target.length) === target;
}

confirmEnding("Bastian", "n");

```

</section>
<hr>

# 7. Repeat a String Repeat a String

## Description
<section id='description'>
Repeat a given string <code>str</code> (first argument) for <code>num</code> times (second argument). Return an empty string if <code>num</code> is not a positive number.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function repeatStringNumTimes(str, num) {
  // repeat after me
  return str;
}

repeatStringNumTimes("abc", 3);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function repeatStringNumTimes(str, num) {
  if (num < 0) return '';
  return num === 1 ? str : str + repeatStringNumTimes(str, num-1);
}

repeatStringNumTimes("abc", 3);

```

</section>
<hr>

# 8. Truncate a String

## Description
<section id='description'>
Truncate a string (first argument) if it is longer than the given maximum string length (second argument). Return the truncated string with a <code>...</code> ending.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function truncateString(str, num) {
  // Clear out that junk in your trunk
  return str;
}

truncateString("A-tisket a-tasket A green and yellow basket", 8);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function truncateString(str, num) {
  if (num >= str.length) {
    return str;
  }

  return str.slice(0, num) + '...';
}

truncateString("A-tisket a-tasket A green and yellow basket", 8);

```

</section>
<hr>

# 9. Finders Keepers

## Description
<section id='description'>
Create a function that looks through an array (first argument) and returns the first element in the array that passes a truth test (second argument). If no element passes the test, return undefined.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function findElement(arr, func) {
  let num = 0;
  return num;
}

findElement([1, 2, 3, 4], num => num % 2 === 0);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function findElement(arr, func) {
  return arr.filter(func)[0];
}

findElement([1, 2, 3, 4], num => num % 2 === 0);

```

</section>
<hr>

# 10. Boo who

## Description
<section id='description'>
Check if a value is classified as a boolean primitive. Return true or false.
Boolean primitives are true and false.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function booWho(bool) {
  // What is the new fad diet for ghost developers? The Boolean.
  return bool;
}

booWho(null);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function booWho(bool) {
  return typeof bool === "boolean";
}

booWho(null);
```

</section>
<hr>

# 11. Title Case a Sentence

## Description
<section id='description'>
Return the provided string with the first letter of each word capitalized. Make sure the rest of the word is in lower case.
For the purpose of this exercise, you should also capitalize connecting words like "the" and "of".
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function titleCase(str) {
  return str;
}

titleCase("I'm a little tea pot");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function titleCase(str) {
  return str.split(' ').map(word => word.charAt(0).toUpperCase() + word.substring(1).toLowerCase()).join(' ');
}

titleCase("I'm a little tea pot");

```

</section>
<hr>

# 12. Slice and Splice

## Description
<section id='description'>
You are given two arrays and an index.
Use the array methods <code>slice</code> and <code>splice</code> to copy each element of the first array into the second array, in order.
Begin inserting elements at index <code>n</code> of the second array.
Return the resulting array. The input arrays should remain the same after the function runs.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function frankenSplice(arr1, arr2, n) {
  // It's alive. It's alive!
  return arr2;
}

frankenSplice([1, 2, 3], [4, 5, 6], 1);
```

</div>


### After Test
<div id='js-teardown'>

```js
let testArr1 = [1, 2];
let testArr2 = ["a", "b"];
```

</div>

</section>

## Solution
<section id='solution'>


```js
function frankenSplice(arr1, arr2, n) {
  // It's alive. It's alive!
  let result = arr2.slice();
  for (let i = 0; i < arr1.length; i++) {
    result.splice(n+i, 0, arr1[i]);
  }
  return result;
}

frankenSplice([1, 2, 3], [4, 5], 1);

```

</section>
<hr>

# 13. Falsy Bouncer

## Description
<section id='description'>
Remove all falsy values from an array.
Falsy values in JavaScript are <code>false</code>, <code>null</code>, <code>0</code>, <code>""</code>, <code>undefined</code>, and <code>NaN</code>.
Hint: Try converting each value to a Boolean.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function bouncer(arr) {
  // Don't show a false ID to this bouncer.
  return arr;
}

bouncer([7, "ate", "", false, 9]);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function bouncer(arr) {
  return arr.filter(e => e);
}

bouncer([7, "ate", "", false, 9]);

```

</section>
<hr>

# 14. Where do I Belong

## Description
<section id='description'>
Return the lowest index at which a value (second argument) should be inserted into an array (first argument) once it has been sorted. The returned value should be a number.
For example, <code>getIndexToIns([1,2,3,4], 1.5)</code> should return <code>1</code> because it is greater than <code>1</code> (index 0), but less than <code>2</code> (index 1).
Likewise, <code>getIndexToIns([20,3,5], 19)</code> should return <code>2</code> because once the array has been sorted it will look like <code>[3,5,20]</code> and <code>19</code> is less than <code>20</code> (index 2) and greater than <code>5</code> (index 1).
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function getIndexToIns(arr, num) {
  // Find my place in this sorted array.
  return num;
}

getIndexToIns([40, 60], 50);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function getIndexToIns(arr, num) {
  arr = arr.sort((a, b) => a - b);

  for (let i = 0; i < arr.length; i++) {
    if (arr[i] >= num) {
      return i;
    }
  }

  return arr.length;
}

getIndexToIns([40, 60], 50);

```

</section>
<hr>

# 15. Mutations

## Description
<section id='description'>
Return true if the string in the first element of the array contains all of the letters of the string in the second element of the array.
For example, <code>["hello", "Hello"]</code>, should return true because all of the letters in the second string are present in the first, ignoring case.
The arguments <code>["hello", "hey"]</code> should return false because the string "hello" does not contain a "y".
Lastly, <code>["Alien", "line"]</code>, should return true because all of the letters in "line" are present in "Alien".
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function mutation(arr) {
  return arr;
}

mutation(["hello", "hey"]);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function mutation(arr) {
  let hash = Object.create(null);

  arr[0].toLowerCase().split('').forEach(c => hash[c] = true);

  return !arr[1].toLowerCase().split('').filter(c => !hash[c]).length;
}

mutation(["hello", "hey"]);

```

</section>
<hr>

# 16. Chunky Monkey

## Description
<section id='description'>
Write a function that splits an array (first argument) into groups the length of <code>size</code> (second argument) and returns them as a two-dimensional array.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function chunkArrayInGroups(arr, size) {
  // Break it up.
  return arr;
}

chunkArrayInGroups(["a", "b", "c", "d"], 2);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function chunkArrayInGroups(arr, size) {
  let out = [];

  for (let i = 0; i < arr.length; i += size) {
    out.push(arr.slice(i, i + size));
  }

  return out;
}

chunkArrayInGroups(["a", "b", "c", "d"], 2);

```

</section>
<hr>

# Object Oriented Programming
# 1. Create a Basic JavaScript Object

## Description
<section id='description'>
Think about things people see everyday, like cars, shops, and birds. These are all <code>objects</code>: tangible things people can observe and interact with.
What are some qualities of these <code>objects</code>? A car has wheels. Shops sell items. Birds have wings.
These qualities, or <code>properties</code>, define what makes up an <code>object</code>. Note that similar <code>objects</code> share the same <code>properties</code>, but may have different values for those <code>properties</code>. For example, all cars have wheels, but not all cars have the same number of wheels.
<code>Objects</code> in JavaScript are used to model real-world objects, giving them <code>properties</code> and behavior just like their real-world counterparts. Here's an example using these concepts to create a <code>duck</code> <code>object</code>:
<blockquote>let duck = {<br>&nbsp;&nbsp;name: "Aflac",<br>&nbsp;&nbsp;numLegs: 2<br>};</blockquote>
This <code>duck</code> <code>object</code> has two property/value pairs: a <code>name</code> of "Aflac" and a <code>numLegs</code> of 2.
</section>

## Instructions
<section id='instructions'>
Create a <code>dog</code> <code>object</code> with <code>name</code> and <code>numLegs</code> properties, and set them to a string and a number, respectively.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let dog = {

};
```

</div>



</section>

## Solution
<section id='solution'>


```js
let dog = {
  name: '',
  numLegs: 4
};
```

</section>
<hr>

# 2. Use Dot Notation to Access the Properties of an Object

## Description
<section id='description'>
The last challenge created an <code>object</code> with various <code>properties</code>, now you'll see how to access the values of those <code>properties</code>. Here's an example:
<blockquote>let duck = {<br>&nbsp;&nbsp;name: "Aflac",<br>&nbsp;&nbsp;numLegs: 2<br>};<br>console.log(duck.name);<br>// This prints "Aflac" to the console</blockquote>
Dot notation is used on the <code>object</code> name, <code>duck</code>, followed by the name of the <code>property</code>, <code>name</code>, to access the value of "Aflac".
</section>

## Instructions
<section id='instructions'>
Print both <code>properties</code> of the <code>dog</code> object below to your console.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let dog = {
  name: "Spot",
  numLegs: 4
};
// Add your code below this line


```

</div>



</section>

## Solution
<section id='solution'>


```js
let dog = {
  name: "Spot",
  numLegs: 4
};
console.log(dog.name);
console.log(dog.numLegs);
```

</section>
<hr>

# 3. Create a Method on an Object

## Description
<section id='description'>
<code>Objects</code> can have a special type of <code>property</code>, called a <code>method</code>.
<code>Methods</code> are <code>properties</code> that are functions. This adds different behavior to an <code>object</code>. Here is the <code>duck</code> example with a method:
<blockquote>let duck = {<br>&nbsp;&nbsp;name: "Aflac",<br>&nbsp;&nbsp;numLegs: 2,<br>&nbsp;&nbsp;sayName: function() {return "The name of this duck is " + duck.name + ".";}<br>};<br>duck.sayName();<br>// Returns "The name of this duck is Aflac."</blockquote>
The example adds the <code>sayName</code> <code>method</code>, which is a function that returns a sentence giving the name of the <code>duck</code>.
Notice that the <code>method</code> accessed the <code>name</code> property in the return statement using <code>duck.name</code>. The next challenge will cover another way to do this.
</section>

## Instructions
<section id='instructions'>
Using the <code>dog</code> <code>object</code>, give it a method called <code>sayLegs</code>. The method should return the sentence "This dog has 4 legs."
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let dog = {
  name: "Spot",
  numLegs: 4,

};

dog.sayLegs();
```

</div>



</section>

## Solution
<section id='solution'>


```js
let dog = {
  name: "Spot",
  numLegs: 4,
  sayLegs () {
    return 'This dog has ' + this.numLegs + ' legs.';
  }
};

dog.sayLegs();
```

</section>
<hr>

# 4. Make Code More Reusable with the this Keyword

## Description
<section id='description'>
The last challenge introduced a <code>method</code> to the <code>duck</code> object. It used <code>duck.name</code> dot notation to access the value for the <code>name</code> property within the return statement:
<code>sayName: function() {return "The name of this duck is " + duck.name + ".";}</code>
While this is a valid way to access the object's property, there is a pitfall here. If the variable name changes, any code referencing the original name would need to be updated as well. In a short object definition, it isn't a problem, but if an object has many references to its properties there is a greater chance for error.
A way to avoid these issues is with the <code>this</code> keyword:
<blockquote>let duck = {<br>&nbsp;&nbsp;name: "Aflac",<br>&nbsp;&nbsp;numLegs: 2,<br>&nbsp;&nbsp;sayName: function() {return "The name of this duck is " + this.name + ".";}<br>};</blockquote>
<code>this</code> is a deep topic, and the above example is only one way to use it. In the current context, <code>this</code> refers to the object that the method is associated with: <code>duck</code>.
If the object's name is changed to <code>mallard</code>, it is not necessary to find all the references to <code>duck</code> in the code. It makes the code reusable and easier to read.
</section>

## Instructions
<section id='instructions'>
Modify the <code>dog.sayLegs</code> method to remove any references to <code>dog</code>. Use the <code>duck</code> example for guidance.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let dog = {
  name: "Spot",
  numLegs: 4,
  sayLegs: function() {return "This dog has " + dog.numLegs + " legs.";}
};

dog.sayLegs();
```

</div>



</section>

## Solution
<section id='solution'>


```js
let dog = {
  name: "Spot",
  numLegs: 4,
  sayLegs () {
    return 'This dog has ' + this.numLegs + ' legs.';
  }
};

dog.sayLegs();
```

</section>
<hr>

# 5. Define a Constructor Function

## Description
<section id='description'>
<code>Constructors</code> are functions that create new objects. They define properties and behaviors that will belong to the new object. Think of them as a blueprint for the creation of new objects.
Here is an example of a <code>constructor</code>:
<blockquote>function Bird() {<br>&nbsp;&nbsp;this.name = "Albert";<br>&nbsp;&nbsp;this.color = "blue";<br>&nbsp;&nbsp;this.numLegs = 2;<br>}</blockquote>
This <code>constructor</code> defines a <code>Bird</code> object with properties <code>name</code>, <code>color</code>, and <code>numLegs</code> set to Albert, blue, and 2, respectively.
<code>Constructors</code> follow a few conventions:
<ul><li><code>Constructors</code> are defined with a capitalized name to distinguish them from other functions that are not <code>constructors</code>.</li><li><code>Constructors</code> use the keyword <code>this</code> to set properties of the object they will create. Inside the <code>constructor</code>, <code>this</code> refers to the new object it will create.</li><li><code>Constructors</code> define properties and behaviors instead of returning a value as other functions might.</li></ul>
</section>

## Instructions
<section id='instructions'>
Create a <code>constructor</code>, <code>Dog</code>, with properties <code>name</code>, <code>color</code>, and <code>numLegs</code> that are set to a string, a string, and a number, respectively.
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
function Dog (name, color, numLegs) {
  this.name = 'name';
  this.color = 'color';
  this.numLegs = 4;
}
```

</section>
<hr>

# 6. Use a Constructor to Create Objects

## Description
<section id='description'>
Here's the <code>Bird</code> constructor from the previous challenge:
<blockquote>function Bird() {<br>&nbsp;&nbsp;this.name = "Albert";<br>&nbsp;&nbsp;this.color  = "blue";<br>&nbsp;&nbsp;this.numLegs = 2;<br>&nbsp;&nbsp;// "this" inside the constructor always refers to the object being created<br>}<br><br>let blueBird = new Bird();</blockquote>
Notice that the <code>new</code> operator is used when calling a constructor. This tells JavaScript to create a new <code>instance</code> of <code>Bird</code> called <code>blueBird</code>. Without the <code>new</code> operator, <code>this</code> inside the constructor would not point to the newly created object, giving unexpected results.
Now <code>blueBird</code> has all the properties defined inside the <code>Bird</code> constructor:
<blockquote>blueBird.name; // => Albert<br>blueBird.color; // => blue<br>blueBird.numLegs; // => 2</blockquote>
Just like any other object, its properties can be accessed and modified:
<blockquote>blueBird.name = 'Elvira';<br>blueBird.name; // => Elvira</blockquote>
</section>

## Instructions
<section id='instructions'>
Use the <code>Dog</code> constructor from the last lesson to create a new instance of <code>Dog</code>, assigning it to a variable <code>hound</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Dog() {
  this.name = "Rupert";
  this.color = "brown";
  this.numLegs = 4;
}
// Add your code below this line


```

</div>



</section>

## Solution
<section id='solution'>


```js
function Dog() {
  this.name = "Rupert";
  this.color = "brown";
  this.numLegs = 4;
}
const hound = new Dog();
```

</section>
<hr>

# 7. Extend Constructors to Receive Arguments

## Description
<section id='description'>
The <code>Bird</code> and <code>Dog</code> constructors from last challenge worked well. However, notice that all <code>Birds</code> that are created with the <code>Bird</code> constructor are automatically named Albert, are blue in color, and have two legs. What if you want birds with different values for name and color? It's possible to change the properties of each bird manually but that would be a lot of work:
<blockquote>let swan = new Bird();<br>swan.name = "Carlos";<br>swan.color = "white";</blockquote>
Suppose you were writing a program to keep track of hundreds or even thousands of different birds in an aviary. It would take a lot of time to create all the birds, then change the properties to different values for every one.
To more easily create different <code>Bird</code> objects, you can design your Bird constructor to accept parameters:
<blockquote>function Bird(name, color) {<br>&nbsp;&nbsp;this.name = name;<br>&nbsp;&nbsp;this.color = color;<br>&nbsp;&nbsp;this.numLegs = 2;<br>}</blockquote>
Then pass in the values as arguments to define each unique bird into the <code>Bird</code> constructor:
<code>let cardinal = new Bird("Bruce", "red");</code>
This gives a new instance of <code>Bird</code> with name and color properties set to Bruce and red, respectively. The <code>numLegs</code> property is still set to 2.
The <code>cardinal</code> has these properties:
<blockquote>cardinal.name // => Bruce<br>cardinal.color // => red<br>cardinal.numLegs // => 2</blockquote>
The constructor is more flexible. It's now possible to define the properties for each <code>Bird</code> at the time it is created, which is one way that JavaScript constructors are so useful. They group objects together based on shared characteristics and behavior and define a blueprint that automates their creation.
</section>

## Instructions
<section id='instructions'>
Create another <code>Dog</code> constructor. This time, set it up to take the parameters <code>name</code> and <code>color</code>, and have the property <code>numLegs</code> fixed at 4. Then create a new <code>Dog</code> saved in a variable <code>terrier</code>. Pass it two strings as arguments for the <code>name</code> and <code>color</code> properties.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Dog() {

}


```

</div>



</section>

## Solution
<section id='solution'>


```js
function Dog (name, color) {
  this.numLegs = 4;
  this.name = name;
  this.color = color;
}

const terrier = new Dog();
```

</section>
<hr>

# 8. Verify an Object's Constructor with instanceof

## Description
<section id='description'>
Anytime a constructor function creates a new object, that object is said to be an <code>instance</code> of its constructor. JavaScript gives a convenient way to verify this with the <code>instanceof</code> operator. <code>instanceof</code> allows you to compare an object to a constructor, returning <code>true</code> or <code>false</code> based on whether or not that object was created with the constructor. Here's an example:
<blockquote>let Bird = function(name, color) {<br>&nbsp;&nbsp;this.name = name;<br>&nbsp;&nbsp;this.color = color;<br>&nbsp;&nbsp;this.numLegs = 2;<br>}<br><br>let crow = new Bird("Alexis", "black");<br><br>crow instanceof Bird; // => true</blockquote>
If an object is created without using a constructor, <code>instanceof</code> will verify that it is not an instance of that constructor:
<blockquote>let canary = {<br>&nbsp;&nbsp;name: "Mildred",<br>&nbsp;&nbsp;color: "Yellow",<br>&nbsp;&nbsp;numLegs: 2<br>};<br><br>canary instanceof Bird; // => false</blockquote>
</section>

## Instructions
<section id='instructions'>
Create a new instance of the <code>House</code> constructor, calling it <code>myHouse</code> and passing a number of bedrooms. Then, use <code>instanceof</code> to verify that it is an instance of <code>House</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
/*jshint expr: true */

function House(numBedrooms) {
  this.numBedrooms = numBedrooms;
}

// Add your code below this line



```

</div>



</section>

## Solution
<section id='solution'>


```js
function House(numBedrooms) {
  this.numBedrooms = numBedrooms;
}
const myHouse = new House(4);
console.log(myHouse instanceof House);
```

</section>
<hr>

# 9. Understand Own Properties

## Description
<section id='description'>
In the following example, the <code>Bird</code> constructor defines two properties: <code>name</code> and <code>numLegs</code>:
<blockquote>function Bird(name) {<br>&nbsp;&nbsp;this.name  = name;<br>&nbsp;&nbsp;this.numLegs = 2;<br>}<br><br>let duck = new Bird("Donald");<br>let canary = new Bird("Tweety");</blockquote>
<code>name</code> and <code>numLegs</code> are called <code>own</code> properties, because they are defined directly on the instance object. That means that <code>duck</code> and <code>canary</code> each has its own separate copy of these properties.
In fact every instance of <code>Bird</code> will have its own copy of these properties.
The following code adds all of the <code>own</code> properties of <code>duck</code> to the array <code>ownProps</code>:
<blockquote>let ownProps = [];<br><br>for (let property in duck) {<br>&nbsp;&nbsp;if(duck.hasOwnProperty(property)) {<br>&nbsp;&nbsp;&nbsp;&nbsp;ownProps.push(property);<br>&nbsp;&nbsp;}<br>}<br><br>console.log(ownProps); // prints [ "name", "numLegs" ]</blockquote>
</section>

## Instructions
<section id='instructions'>
Add the <code>own</code> properties of <code>canary</code> to the array <code>ownProps</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Bird(name) {
  this.name = name;
  this.numLegs = 2;
}

let canary = new Bird("Tweety");
let ownProps = [];
// Add your code below this line



```

</div>



</section>

## Solution
<section id='solution'>


```js
function Bird(name) {
  this.name = name;
  this.numLegs = 2;
}

let canary = new Bird("Tweety");
function getOwnProps (obj) {
  const props = [];

  for (let prop in obj) {
    if (obj.hasOwnProperty(prop)) {
      props.push(prop);
    }
  }

  return props;
}

const ownProps = getOwnProps(canary);
```

</section>
<hr>

# 10. Use Prototype Properties to Reduce Duplicate Code

## Description
<section id='description'>
Since <code>numLegs</code> will probably have the same value for all instances of <code>Bird</code>, you essentially have a duplicated variable <code>numLegs</code> inside each <code>Bird</code> instance.
This may not be an issue when there are only two instances, but imagine if there are millions of instances. That would be a lot of duplicated variables.
A better way is to use <code>Bird’s</code> <code>prototype</code>. The <code>prototype</code> is an object that is shared among ALL instances of <code>Bird</code>. Here's how to add <code>numLegs</code> to the <code>Bird prototype</code>:
<blockquote>Bird.prototype.numLegs = 2;</blockquote>
Now all instances of <code>Bird</code> have the <code>numLegs</code> property.
<blockquote>console.log(duck.numLegs);  // prints 2<br>console.log(canary.numLegs);  // prints 2</blockquote>
Since all instances automatically have the properties on the <code>prototype</code>, think of a <code>prototype</code> as a "recipe" for creating objects.
Note that the <code>prototype</code> for <code>duck</code> and <code>canary</code> is part of the <code>Bird</code> constructor as <code>Bird.prototype</code>. Nearly every object in JavaScript has a <code>prototype</code> property which is part of the constructor function that created it.
</section>

## Instructions
<section id='instructions'>
Add a <code>numLegs</code> property to the <code>prototype</code> of <code>Dog</code>
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Dog(name) {
  this.name = name;
}



// Add your code above this line
let beagle = new Dog("Snoopy");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function Dog (name) {
  this.name = name;
}
Dog.prototype.numLegs = 4;
let beagle = new Dog("Snoopy");
```

</section>
<hr>

# 11. Iterate Over All Properties﻿

## Description
<section id='description'>
You have now seen two kinds of properties: <code>own</code> properties and <code>prototype</code> properties. <code>Own</code> properties are defined directly on the object instance itself. And <code>prototype</code> properties are defined on the <code>prototype</code>.
<blockquote>function Bird(name) {<br>&nbsp;&nbsp;this.name = name;  //own property<br>}<br><br>Bird.prototype.numLegs = 2; // prototype property<br><br>let duck = new Bird("Donald");</blockquote>
Here is how you add <code>duck</code>'s <code>own</code> properties to the array <code>ownProps</code> and <code>prototype</code> properties to the array <code>prototypeProps</code>:
<blockquote>let ownProps = [];<br>let prototypeProps = [];<br><br>for (let property in duck) {<br>&nbsp;&nbsp;if(duck.hasOwnProperty(property)) {<br>&nbsp;&nbsp;&nbsp;&nbsp;ownProps.push(property);<br>&nbsp;&nbsp;} else {<br>&nbsp;&nbsp;&nbsp;&nbsp;prototypeProps.push(property);<br>&nbsp;&nbsp;}<br>}<br><br>console.log(ownProps); // prints ["name"]<br>console.log(prototypeProps); // prints ["numLegs"]</blockquote>
</section>

## Instructions
<section id='instructions'>
Add all of the <code>own</code> properties of <code>beagle</code> to the array <code>ownProps</code>. Add all of the <code>prototype</code> properties of <code>Dog</code> to the array <code>prototypeProps</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Dog(name) {
  this.name = name;
}

Dog.prototype.numLegs = 4;

let beagle = new Dog("Snoopy");

let ownProps = [];
let prototypeProps = [];

// Add your code below this line



```

</div>



</section>

## Solution
<section id='solution'>


```js
function Dog(name) {
  this.name = name;
}

Dog.prototype.numLegs = 4;

let beagle = new Dog("Snoopy");

let ownProps = [];
let prototypeProps = [];
for (let prop in beagle) {
  if (beagle.hasOwnProperty(prop)) {
    ownProps.push(prop);
  } else {
    prototypeProps.push(prop);
  }
}
```

</section>
<hr>

# 12. Understand the Constructor Property

## Description
<section id='description'>
There is a special <code>constructor</code> property located on the object instances <code>duck</code> and <code>beagle</code> that were created in the previous challenges:
<blockquote>let duck = new Bird();<br>let beagle = new Dog();<br><br>console.log(duck.constructor === Bird);  //prints true<br>console.log(beagle.constructor === Dog);  //prints true</blockquote>
Note that the <code>constructor</code> property is a reference to the constructor function that created the instance.
The advantage of the <code>constructor</code> property is that it's possible to check for this property to find out what kind of object it is. Here's an example of how this could be used:
<blockquote>function joinBirdFraternity(candidate) {<br>&nbsp;&nbsp;if (candidate.constructor === Bird) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return true;<br>&nbsp;&nbsp;} else {<br>&nbsp;&nbsp;&nbsp;&nbsp;return false;<br>&nbsp;&nbsp;}<br>}</blockquote>
<strong>Note</strong><br>Since the <code>constructor</code> property can be overwritten (which will be covered in the next two challenges) it’s generally better to use the <code>instanceof</code> method to check the type of an object.
</section>

## Instructions
<section id='instructions'>
Write a <code>joinDogFraternity</code> function that takes a <code>candidate</code> parameter and, using the <code>constructor</code> property, return <code>true</code> if the candidate is a <code>Dog</code>, otherwise return <code>false</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Dog(name) {
  this.name = name;
}

// Add your code below this line
function joinDogFraternity(candidate) {

}

```

</div>



</section>

## Solution
<section id='solution'>


```js
function Dog(name) {
  this.name = name;
}
function joinDogFraternity(candidate) {
  return candidate.constructor === Dog;
}
```

</section>
<hr>

# 13. Change the Prototype to a New Object

## Description
<section id='description'>
Up until now you have been adding properties to the <code>prototype</code> individually:
<blockquote>Bird.prototype.numLegs = 2;</blockquote>
This becomes tedious after more than a few properties.
<blockquote>Bird.prototype.eat = function() {<br>&nbsp;&nbsp;console.log("nom nom nom");<br>}<br><br>Bird.prototype.describe = function() {<br>&nbsp;&nbsp;console.log("My name is " + this.name);<br>}</blockquote>
A more efficient way is to set the <code>prototype</code> to a new object that already contains the properties. This way, the properties are added all at once:
<blockquote>Bird.prototype = {<br>&nbsp;&nbsp;numLegs: 2, <br>&nbsp;&nbsp;eat: function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("nom nom nom");<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;describe: function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("My name is " + this.name);<br>&nbsp;&nbsp;}<br>};</blockquote>
</section>

## Instructions
<section id='instructions'>
Add the property <code>numLegs</code> and the two methods <code>eat()</code> and <code>describe()</code> to the <code>prototype</code> of <code>Dog</code> by setting the <code>prototype</code> to a new object.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Dog(name) {
  this.name = name;
}

Dog.prototype = {
  // Add your code below this line

};
```

</div>



</section>

## Solution
<section id='solution'>


```js
function Dog(name) {
  this.name = name;
}
Dog.prototype = {
numLegs: 4,
  eat () {
    console.log('nom nom nom');
  },
  describe () {
    console.log('My name is ' + this.name);
  }
};
```

</section>
<hr>

# 14. Remember to Set the Constructor Property when Changing the Prototype

## Description
<section id='description'>
There is one crucial side effect of manually setting the prototype to a new object. It erases the <code>constructor</code> property! This property can be used to check which constructor function created the instance, but since the property has been overwritten, it now gives false results:
<blockquote>duck.constructor === Bird; // false -- Oops <br> duck.constructor === Object; // true, all objects inherit from Object.prototype <br> duck instanceof Bird; // true, still works</blockquote>
To fix this, whenever a prototype is manually set to a new object, remember to define the <code>constructor</code> property:
<blockquote>Bird.prototype = {<br>&nbsp;&nbsp;constructor: Bird, // define the constructor property<br>&nbsp;&nbsp;numLegs: 2,<br>&nbsp;&nbsp;eat: function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("nom nom nom");<br>&nbsp;&nbsp;},<br>&nbsp;&nbsp;describe: function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("My name is " + this.name); <br>&nbsp;&nbsp;}<br>};</blockquote>
</section>

## Instructions
<section id='instructions'>
Define the <code>constructor</code> property on the <code>Dog</code> <code>prototype</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Dog(name) {
  this.name = name;
}

// Modify the code below this line
Dog.prototype = {

  numLegs: 4,
  eat: function() {
    console.log("nom nom nom");
  },
  describe: function() {
    console.log("My name is " + this.name);
  }
};
```

</div>



</section>

## Solution
<section id='solution'>


```js
function Dog(name) {
  this.name = name;
}
Dog.prototype = {
  constructor: Dog,
  numLegs: 4,
  eat: function() {
    console.log("nom nom nom");
  },
  describe: function() {
    console.log("My name is " + this.name);
  }
};
```

</section>
<hr>

# 15. Understand Where an Object’s Prototype Comes From

## Description
<section id='description'>
Just like people inherit genes from their parents, an object inherits its <code>prototype</code> directly from the constructor function that created it. For example, here the <code>Bird</code> constructor creates the <code>duck</code> object:
<blockquote>function Bird(name) {<br>&nbsp;&nbsp;this.name = name;<br>}<br><br>let duck = new Bird("Donald");</blockquote>
<code>duck</code> inherits its <code>prototype</code> from the <code>Bird</code> constructor function. You can show this relationship with the <code>isPrototypeOf</code> method:
<blockquote>Bird.prototype.isPrototypeOf(duck);<br>// returns true</blockquote>
</section>

## Instructions
<section id='instructions'>
Use <code>isPrototypeOf</code> to check the <code>prototype</code> of <code>beagle</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Dog(name) {
  this.name = name;
}

let beagle = new Dog("Snoopy");

// Add your code below this line


```

</div>



</section>

## Solution
<section id='solution'>


```js
function Dog(name) {
  this.name = name;
}
let beagle = new Dog("Snoopy");
Dog.prototype.isPrototypeOf(beagle);
```

</section>
<hr>

# 16. Understand the Prototype Chain

## Description
<section id='description'>
All objects in JavaScript (with a few exceptions) have a <code>prototype</code>. Also, an object’s <code>prototype</code> itself is an object.
<blockquote>function Bird(name) {<br>&nbsp;&nbsp;this.name = name;<br>}<br><br>typeof Bird.prototype; // => object</blockquote>
Because a <code>prototype</code> is an object, a <code>prototype</code> can have its own <code>prototype</code>! In this case, the <code>prototype</code> of <code>Bird.prototype</code> is <code>Object.prototype</code>:
<blockquote>Object.prototype.isPrototypeOf(Bird.prototype);<br>// returns true</blockquote>
How is this useful? You may recall the <code>hasOwnProperty</code> method from a previous challenge:
<blockquote>let duck = new Bird("Donald");<br>duck.hasOwnProperty("name"); // => true</blockquote>
The <code>hasOwnProperty</code> method is defined in <code>Object.prototype</code>, which can be accessed by <code>Bird.prototype</code>, which can then be accessed by <code>duck</code>. This is an example of the <code>prototype</code> chain.
In this <code>prototype</code> chain, <code>Bird</code> is the <code>supertype</code> for <code>duck</code>, while <code>duck</code> is the <code>subtype</code>. <code>Object</code> is a <code>supertype</code> for both <code>Bird</code> and <code>duck</code>.
<code>Object</code> is a <code>supertype</code> for all objects in JavaScript. Therefore, any object can use the <code>hasOwnProperty</code> method.
</section>

## Instructions
<section id='instructions'>
Modify the code to show the correct prototype chain.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Dog(name) {
  this.name = name;
}

let beagle = new Dog("Snoopy");

Dog.prototype.isPrototypeOf(beagle);  // => true

// Fix the code below so that it evaluates to true
???.isPrototypeOf(Dog.prototype);

```

</div>



</section>

## Solution
<section id='solution'>


```js
function Dog(name) {
  this.name = name;
}
let beagle = new Dog("Snoopy");
Dog.prototype.isPrototypeOf(beagle);
Object.prototype.isPrototypeOf(Dog.prototype);
```

</section>
<hr>

# 17. Use Inheritance So You Don't Repeat Yourself

## Description
<section id='description'>
There's a principle in programming called <code>Don't Repeat Yourself (DRY)</code>. The reason repeated code is a problem is because any change requires fixing code in multiple places. This usually means more work for programmers and more room for errors.
Notice in the example below that the <code>describe</code> method is shared by <code>Bird</code> and <code>Dog</code>:
<blockquote>Bird.prototype = {<br>&nbsp;&nbsp;constructor: Bird,<br>&nbsp;&nbsp;describe: function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("My name is " + this.name);<br>&nbsp;&nbsp;}<br>};<br><br>Dog.prototype = {<br>&nbsp;&nbsp;constructor: Dog,<br>&nbsp;&nbsp;describe: function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("My name is " + this.name);<br>&nbsp;&nbsp;}<br>};</blockquote>
The <code>describe</code> method is repeated in two places. The code can be edited to follow the <code>DRY</code> principle by creating a <code>supertype</code> (or parent) called <code>Animal</code>:
<blockquote>function Animal() { };<br><br>Animal.prototype = {<br>&nbsp;&nbsp;constructor: Animal, <br>&nbsp;&nbsp;describe: function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("My name is " + this.name);<br>&nbsp;&nbsp;}<br>};</blockquote>
Since <code>Animal</code> includes the <code>describe</code> method, you can remove it from <code>Bird</code> and <code>Dog</code>:
<blockquote>Bird.prototype = {<br>&nbsp;&nbsp;constructor: Bird<br>};<br><br>Dog.prototype = {<br>&nbsp;&nbsp;constructor: Dog<br>};</blockquote>
</section>

## Instructions
<section id='instructions'>
The <code>eat</code> method is repeated in both <code>Cat</code> and <code>Bear</code>. Edit the code in the spirit of <code>DRY</code> by moving the <code>eat</code> method to the <code>Animal</code> <code>supertype</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Cat(name) {
  this.name = name;
}

Cat.prototype = {
  constructor: Cat,
  eat: function() {
    console.log("nom nom nom");
  }
};

function Bear(name) {
  this.name = name;
}

Bear.prototype = {
  constructor: Bear,
  eat: function() {
    console.log("nom nom nom");
  }
};

function Animal() { }

Animal.prototype = {
  constructor: Animal,

};
```

</div>



</section>

## Solution
<section id='solution'>


```js
function Cat(name) {
  this.name = name;
}

Cat.prototype = {
  constructor: Cat
};

function Bear(name) {
  this.name = name;
}

Bear.prototype = {
  constructor: Bear
};

function Animal() { }

Animal.prototype = {
  constructor: Animal,
  eat: function() {
    console.log("nom nom nom");
  }
};
```

</section>
<hr>

# 18. Inherit Behaviors from a Supertype

## Description
<section id='description'>
In the previous challenge, you created a <code>supertype</code> called <code>Animal</code> that defined behaviors shared by all animals:
<blockquote>function Animal() { }<br>Animal.prototype.eat = function() {<br>&nbsp;&nbsp;console.log("nom nom nom");<br>};</blockquote>
This and the next challenge will cover how to reuse <code>Animal's</code> methods inside <code>Bird</code> and <code>Dog</code> without defining them again. It uses a technique called <code>inheritance</code>.
This challenge covers the first step: make an instance of the <code>supertype</code> (or parent).
You already know one way to create an instance of <code>Animal</code> using the <code>new</code> operator:
<blockquote>let animal = new Animal();</blockquote>
There are some disadvantages when using this syntax for <code>inheritance</code>, which are too complex for the scope of this challenge. Instead, here's an alternative approach without those disadvantages:
<blockquote>let animal = Object.create(Animal.prototype);</blockquote>
<code>Object.create(obj)</code> creates a new object, and sets <code>obj</code> as the new object's <code>prototype</code>. Recall that the <code>prototype</code> is like the "recipe" for creating an object. By setting the <code>prototype</code> of <code>animal</code> to be <code>Animal's</code> <code>prototype</code>, you are effectively giving the <code>animal</code> instance the same "recipe" as any other instance of <code>Animal</code>.
<blockquote>animal.eat(); // prints "nom nom nom"<br>animal instanceof Animal; // => true</blockquote>
</section>

## Instructions
<section id='instructions'>
Use <code>Object.create</code> to make two instances of <code>Animal</code> named <code>duck</code> and <code>beagle</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Animal() { }

Animal.prototype = {
  constructor: Animal,
  eat: function() {
    console.log("nom nom nom");
  }
};

// Add your code below this line

let duck; // Change this line
let beagle; // Change this line

duck.eat(); // Should print "nom nom nom"
beagle.eat(); // Should print "nom nom nom"
```

</div>



</section>

## Solution
<section id='solution'>


```js
function Animal() { }

Animal.prototype = {
  constructor: Animal,
  eat: function() {
    console.log("nom nom nom");
  }
};
let duck = Object.create(Animal.prototype);
let beagle = Object.create(Animal.prototype);

duck.eat();
beagle.eat();
```

</section>
<hr>

# 19. Set the Child's Prototype to an Instance of the Parent

## Description
<section id='description'>
In the previous challenge you saw the first step for inheriting behavior from the <code>supertype</code> (or parent) <code>Animal</code>: making a new instance of <code>Animal</code>.
This challenge covers the next step: set the <code>prototype</code> of the <code>subtype</code> (or child)&mdash;in this case, <code>Bird</code>&mdash;to be an instance of <code>Animal</code>.
<blockquote>Bird.prototype = Object.create(Animal.prototype);</blockquote>
Remember that the <code>prototype</code> is like the "recipe" for creating an object. In a way, the recipe for <code>Bird</code> now includes all the key "ingredients" from <code>Animal</code>.
<blockquote>let duck = new Bird("Donald");<br>duck.eat(); // prints "nom nom nom"</blockquote>
<code>duck</code> inherits all of <code>Animal</code>'s properties, including the <code>eat</code> method.
</section>

## Instructions
<section id='instructions'>
Modify the code so that instances of <code>Dog</code> inherit from <code>Animal</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Animal() { }

Animal.prototype = {
  constructor: Animal,
  eat: function() {
    console.log("nom nom nom");
  }
};

function Dog() { }

// Add your code below this line


let beagle = new Dog();
beagle.eat();  // Should print "nom nom nom"
```

</div>



</section>

## Solution
<section id='solution'>


```js
function Animal() { }

Animal.prototype = {
  constructor: Animal,
  eat: function() {
    console.log("nom nom nom");
  }
};

function Dog() { }
Dog.prototype = Object.create(Animal.prototype);

let beagle = new Dog();
beagle.eat();
```

</section>
<hr>

# 20. Reset an Inherited Constructor Property

## Description
<section id='description'>
When an object inherits its <code>prototype</code> from another object, it also inherits the <code>supertype</code>'s constructor property.
Here's an example:
<blockquote>function Bird() { }<br>Bird.prototype = Object.create(Animal.prototype);<br>let duck = new Bird();<br>duck.constructor // function Animal(){...}</blockquote>
But <code>duck</code> and all instances of <code>Bird</code> should show that they were constructed by <code>Bird</code> and not <code>Animal</code>. To do so, you can manually set <code>Bird's</code> constructor property to the <code>Bird</code> object:
<blockquote>Bird.prototype.constructor = Bird;<br>duck.constructor // function Bird(){...}</blockquote>
</section>

## Instructions
<section id='instructions'>
Fix the code so <code>duck.constructor</code> and <code>beagle.constructor</code> return their respective constructors.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Animal() { }
function Bird() { }
function Dog() { }

Bird.prototype = Object.create(Animal.prototype);
Dog.prototype = Object.create(Animal.prototype);

// Add your code below this line



let duck = new Bird();
let beagle = new Dog();
```

</div>



</section>

## Solution
<section id='solution'>


```js
function Animal() { }
function Bird() { }
function Dog() { }
Bird.prototype = Object.create(Animal.prototype);
Dog.prototype = Object.create(Animal.prototype);
Dog.prototype.constructor = Dog;
Bird.prototype.constructor = Bird;
let duck = new Bird();
let beagle = new Dog();
```

</section>
<hr>

# 21. Add Methods After Inheritance

## Description
<section id='description'>
A constructor function that inherits its <code>prototype</code> object from a <code>supertype</code> constructor function can still have its own methods in addition to inherited methods.
For example, <code>Bird</code> is a constructor that inherits its <code>prototype</code> from <code>Animal</code>:
<blockquote>function Animal() { }<br>Animal.prototype.eat = function() {<br>&nbsp;&nbsp;console.log("nom nom nom");<br>};<br>function Bird() { }<br>Bird.prototype = Object.create(Animal.prototype);<br>Bird.prototype.constructor = Bird;</blockquote>
In addition to what is inherited from <code>Animal</code>, you want to add behavior that is unique to <code>Bird</code> objects. Here, <code>Bird</code> will get a <code>fly()</code> function. Functions are added to <code>Bird's</code> <code>prototype</code> the same way as any constructor function:
<blockquote>Bird.prototype.fly = function() {<br>&nbsp;&nbsp;console.log("I'm flying!");<br>};</blockquote>
Now instances of <code>Bird</code> will have both <code>eat()</code> and <code>fly()</code> methods:
<blockquote>let duck = new Bird();<br>duck.eat(); // prints "nom nom nom"<br>duck.fly(); // prints "I'm flying!"</blockquote>
</section>

## Instructions
<section id='instructions'>
Add all necessary code so the <code>Dog</code> object inherits from <code>Animal</code> and the <code>Dog's</code> <code>prototype</code> constructor is set to Dog. Then add a <code>bark()</code> method to the <code>Dog</code> object so that <code>beagle</code> can both <code>eat()</code> and <code>bark()</code>. The <code>bark()</code> method should print "Woof!" to the console.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Animal() { }
Animal.prototype.eat = function() { console.log("nom nom nom"); };

function Dog() { }

// Add your code below this line




// Add your code above this line

let beagle = new Dog();

beagle.eat(); // Should print "nom nom nom"
beagle.bark(); // Should print "Woof!"
```

</div>



</section>

## Solution
<section id='solution'>


```js
function Animal() { }
Animal.prototype.eat = function() { console.log("nom nom nom"); };

function Dog() { }
Dog.prototype = Object.create(Animal.prototype);
Dog.prototype.constructor = Dog;
Dog.prototype.bark = function () {
  console.log('Woof!');
};
let beagle = new Dog();

beagle.eat();
beagle.bark();
```

</section>
<hr>

# 22. Override Inherited Methods

## Description
<section id='description'>
In previous lessons, you learned that an object can inherit its behavior (methods) from another object by cloning its <code>prototype</code> object:
<blockquote>ChildObject.prototype = Object.create(ParentObject.prototype);</blockquote>
Then the <code>ChildObject</code> received its own methods by chaining them onto its <code>prototype</code>:
<blockquote>ChildObject.prototype.methodName = function() {...};</blockquote>
It's possible to override an inherited method. It's done the same way - by adding a method to <code>ChildObject.prototype</code> using the same method name as the one to override.
Here's an example of <code>Bird</code> overriding the <code>eat()</code> method inherited from <code>Animal</code>:
<blockquote>function Animal() { }<br>Animal.prototype.eat = function() {<br>&nbsp;&nbsp;return "nom nom nom";<br>};<br>function Bird() { }<br><br>// Inherit all methods from Animal<br>Bird.prototype = Object.create(Animal.prototype);<br><br>// Bird.eat() overrides Animal.eat()<br>Bird.prototype.eat = function() {<br>&nbsp;&nbsp;return "peck peck peck";<br>};</blockquote>
If you have an instance <code>let duck = new Bird();</code> and you call <code>duck.eat()</code>, this is how JavaScript looks for the method on <code>duck’s</code> <code>prototype</code> chain:
1. duck => Is eat() defined here? No.
2. Bird => Is eat() defined here? => Yes. Execute it and stop searching.
3. Animal => eat() is also defined, but JavaScript stopped searching before reaching this level.
4. Object => JavaScript stopped searching before reaching this level.
</section>

## Instructions
<section id='instructions'>
Override the <code>fly()</code> method for <code>Penguin</code> so that it returns "Alas, this is a flightless bird."
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Bird() { }

Bird.prototype.fly = function() { return "I am flying!"; };

function Penguin() { }
Penguin.prototype = Object.create(Bird.prototype);
Penguin.prototype.constructor = Penguin;

// Add your code below this line



// Add your code above this line

let penguin = new Penguin();
console.log(penguin.fly());
```

</div>



</section>

## Solution
<section id='solution'>


```js
function Bird() { }

Bird.prototype.fly = function() { return "I am flying!"; };

function Penguin() { }
Penguin.prototype = Object.create(Bird.prototype);
Penguin.prototype.constructor = Penguin;
Penguin.prototype.fly = () => 'Alas, this is a flightless bird.';
let penguin = new Penguin();
console.log(penguin.fly());
```

</section>
<hr>

# 23. Use a Mixin to Add Common Behavior Between Unrelated Objects

## Description
<section id='description'>
As you have seen, behavior is shared through inheritance. However, there are cases when inheritance is not the best solution. Inheritance does not work well for unrelated objects like <code>Bird</code> and <code>Airplane</code>. They can both fly, but a <code>Bird</code> is not a type of <code>Airplane</code> and vice versa.
For unrelated objects, it's better to use <code>mixins</code>. A <code>mixin</code> allows other objects to use a collection of functions.
<blockquote>let flyMixin = function(obj) {<br>&nbsp;&nbsp;obj.fly = function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("Flying, wooosh!");<br>&nbsp;&nbsp;}<br>};</blockquote>
The <code>flyMixin</code> takes any object and gives it the <code>fly</code> method.
<blockquote>let bird = {<br>&nbsp;&nbsp;name: "Donald",<br>&nbsp;&nbsp;numLegs: 2<br>};<br><br>let plane = {<br>&nbsp;&nbsp;model: "777",<br>&nbsp;&nbsp;numPassengers: 524<br>};<br><br>flyMixin(bird);<br>flyMixin(plane);</blockquote>
Here <code>bird</code> and <code>plane</code> are passed into <code>flyMixin</code>, which then assigns the <code>fly</code> function to each object. Now <code>bird</code> and <code>plane</code> can both fly:
<blockquote>bird.fly(); // prints "Flying, wooosh!"<br>plane.fly(); // prints "Flying, wooosh!"</blockquote>
Note how the <code>mixin</code> allows for the same <code>fly</code> method to be reused by unrelated objects <code>bird</code> and <code>plane</code>.
</section>

## Instructions
<section id='instructions'>
Create a <code>mixin</code> named <code>glideMixin</code> that defines a method named <code>glide</code>. Then use the <code>glideMixin</code> to give both <code>bird</code> and <code>boat</code> the ability to glide.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let bird = {
  name: "Donald",
  numLegs: 2
};

let boat = {
  name: "Warrior",
  type: "race-boat"
};

// Add your code below this line






```

</div>



</section>

## Solution
<section id='solution'>


```js
let bird = {
  name: "Donald",
  numLegs: 2
};

let boat = {
  name: "Warrior",
  type: "race-boat"
};
function glideMixin (obj) {
  obj.glide = () => 'Gliding!';
}

glideMixin(bird);
glideMixin(boat);
```

</section>
<hr>

# 24. Use Closure to Protect Properties Within an Object from Being Modified Externally

## Description
<section id='description'>

In the previous challenge, <code>bird</code> had a public property <code>name</code>. It is considered public because it can be accessed and changed outside of <code>bird</code>'s definition.

<blockquote>bird.name = "Duffy";</blockquote>

Therefore, any part of your code can easily change the name of <code>bird</code> to any value. Think about things like passwords and bank accounts being easily changeable by any part of your codebase. That could cause a lot of issues.

The simplest way to make this public property private is by creating a variable within the constructor function. This changes the scope of that variable to be within the constructor function versus available globally. This way, the variable can only be accessed and changed by methods also within the constructor function.
<blockquote>function Bird() {<br>&nbsp;&nbsp;let hatchedEgg = 10; // private variable<br><br>&nbsp;&nbsp;/*publicly available method that a bird object can use */<br>&nbsp;&nbsp;this.getHatchedEggCount = function() { <br>&nbsp;&nbsp;&nbsp;&nbsp;return hatchedEgg;<br>&nbsp;&nbsp;};<br>}<br>let ducky = new Bird();<br>ducky.getHatchedEggCount(); // returns 10</blockquote>
Here <code>getHachedEggCount</code> is a privileged method, because it has access to the private variable <code>hatchedEgg</code>. This is possible because <code>hatchedEgg</code> is declared in the same context as <code>getHachedEggCount</code>. In JavaScript, a function always has access to the context in which it was created. This is called <code>closure</code>.

</section>

## Instructions
<section id='instructions'>
Change how <code>weight</code> is declared in the <code>Bird</code> function so it is a private variable. Then, create a method <code>getWeight</code> that returns the value of <code>weight</code> 15.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function Bird() {
  this.weight = 15;


}

```

</div>



</section>

## Solution
<section id='solution'>


```js
function Bird() {
  let weight = 15;

  this.getWeight = () => weight;
}
```

</section>
<hr>

# 25. Understand the Immediately Invoked Function Expression (IIFE)

## Description
<section id='description'>
A common pattern in JavaScript is to execute a function as soon as it is declared:
<blockquote>(function () {<br>&nbsp;&nbsp;console.log("Chirp, chirp!");<br>})(); // this is an anonymous function expression that executes right away<br>// Outputs "Chirp, chirp!" immediately</blockquote>
Note that the function has no name and is not stored in a variable. The two parentheses () at the end of the function expression cause it to be immediately executed or invoked. This pattern is known as an <code>immediately invoked function expression</code> or <code>IIFE</code>.
</section>

## Instructions
<section id='instructions'>
Rewrite the function <code>makeNest</code> and remove its call so instead it's an anonymous <code>immediately invoked function expression</code> (<code>IIFE</code>).
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function makeNest() {
  console.log("A cozy nest is ready");
}

makeNest();
```

</div>



</section>

## Solution
<section id='solution'>


```js
(function () {
  console.log("A cozy nest is ready");
})();
```

</section>
<hr>

# 26. Use an IIFE to Create a Module

## Description
<section id='description'>
An <code>immediately invoked function expression</code> (<code>IIFE</code>) is often used to group related functionality into a single object or <code>module</code>. For example, an earlier challenge defined two mixins:
<blockquote>function glideMixin(obj) {<br>&nbsp;&nbsp;obj.glide = function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("Gliding on the water");<br>&nbsp;&nbsp;};<br>}<br>function flyMixin(obj) {<br>&nbsp;&nbsp;obj.fly = function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;console.log("Flying, wooosh!");<br>&nbsp;&nbsp;};<br>}</blockquote>
We can group these <code>mixins</code> into a module as follows:
<blockquote>let motionModule = (function () {<br>&nbsp;&nbsp;return {<br>&nbsp;&nbsp;&nbsp;&nbsp;glideMixin: function (obj) {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;obj.glide = function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;console.log("Gliding on the water");<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;};<br>&nbsp;&nbsp;&nbsp;&nbsp;},<br>&nbsp;&nbsp;&nbsp;&nbsp;flyMixin: function(obj) {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;obj.fly = function() {<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;console.log("Flying, wooosh!");<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;};<br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>&nbsp;&nbsp;}<br>}) (); // The two parentheses cause the function to be immediately invoked</blockquote>
Note that you have an <code>immediately invoked function expression</code> (<code>IIFE</code>) that returns an object <code>motionModule</code>. This returned object contains all of the <code>mixin</code> behaviors as properties of the object.
The advantage of the <code>module</code> pattern is that all of the motion behaviors can be packaged into a single object that can then be used by other parts of your code. Here is an example using it:
<blockquote>motionModule.glideMixin(duck);<br>duck.glide();</blockquote>
</section>

## Instructions
<section id='instructions'>
Create a <code>module</code> named <code>funModule</code> to wrap the two <code>mixins</code> <code>isCuteMixin</code> and <code>singMixin</code>. <code>funModule</code> should return an object.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
let isCuteMixin = function(obj) {
  obj.isCute = function() {
    return true;
  };
};
let singMixin = function(obj) {
  obj.sing = function() {
    console.log("Singing to an awesome tune");
  };
};
```

</div>



</section>

## Solution
<section id='solution'>


```js
const funModule = (function () {
  return {
    isCuteMixin: obj => {
      obj.isCute = () => true;
    },
    singMixin: obj => {
      obj.sing = () => console.log("Singing to an awesome tune");
    }
  };
})();
```

</section>
<hr>

# Functional Programming
# 1. Learn About Functional Programming

## Description
<section id='description'>
Functional programming is a style of programming where solutions are simple, isolated functions, without any side effects outside of the function scope.
<code>INPUT -> PROCESS -> OUTPUT</code>
Functional programming is about:
1) Isolated functions - there is no dependence on the state of the program, which includes global variables that are subject to change
2) Pure functions - the same input always gives the same output
3) Functions with limited side effects - any changes, or mutations, to the state of the program outside the function are carefully controlled
</section>

## Instructions
<section id='instructions'>
The members of freeCodeCamp happen to love tea.
In the code editor, the <code>prepareTea</code> and <code>getTea</code> functions are already defined for you. Call the <code>getTea</code> function to get 40 cups of tea for the team, and store them in the <code>tea4TeamFCC</code> variable.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
/** *A long process to prepare tea.
 *@return {string} A cup of tea.
 **/
const prepareTea = () => 'greenTea';

/** *Get given number of cups of tea.
 *@param {number} numOfCups Number of required cups of tea.
 *@return {Array<string>} Given amount of tea cups.
 **/
const getTea = (numOfCups) => {
  const teaCups = [];

  for(let cups = 1; cups <= numOfCups; cups += 1) {
    const teaCup = prepareTea();
    teaCups.push(teaCup);
  }

  return teaCups;
};

// Add your code below this line

const tea4TeamFCC = null; // :(

// Add your code above this line

console.log(tea4TeamFCC);
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

# 2. Understand Functional Programming Terminology

## Description
<section id='description'>
The FCC Team had a mood swing and now wants two types of tea: green tea and black tea. General Fact: Client mood swings are pretty common.
With that information, we'll need to revisit the <code>getTea</code> function from last challenge to handle various tea requests. We can modify <code>getTea</code> to accept a function as a parameter to be able to change the type of tea it prepares. This makes <code>getTea</code> more flexible, and gives the programmer more control when client requests change.
But first, let's cover some functional terminology:
<code>Callbacks</code> are the functions that are slipped or passed into another function to decide the invocation of that function. You may have seen them passed to other methods, for example in <code>filter</code>, the callback function tells JavaScript the criteria for how to filter an array.
Functions that can be assigned to a variable, passed into another function, or returned from another function just like any other normal value, are called <code>first class</code> functions. In JavaScript, all functions are <code>first class</code> functions.
The functions that take a function as an argument, or return a function as a return value are called <code>higher order</code> functions.
When the functions are passed in to another function or returned from another function, then those functions which gets passed in or returned can be called a <code>lambda</code>.
</section>

## Instructions
<section id='instructions'>
Prepare 27 cups of green tea and 13 cups of black tea and store them in <code>tea4GreenTeamFCC</code> and <code>tea4BlackTeamFCC</code> variables, respectively. Note that the <code>getTea</code> function has been modified so it now takes a function as the first argument.
Note: The data (the number of cups of tea) is supplied as the last argument. We'll discuss this more in later lessons.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
/** *A long process to prepare green tea.
 *@return {string} A cup of green tea.
 **/
const prepareGreenTea = () => 'greenTea';

/** *A long process to prepare black tea.
 *@return {string} A cup of black tea.
 **/
const prepareBlackTea = () => 'blackTea';

/** *Get given number of cups of tea.
 *@param {function():string} prepareTea The type of tea preparing function.
 *@param {number} numOfCups Number of required cups of tea.
 *@return {Array<string>} Given amount of tea cups.
 **/
const getTea = (prepareTea, numOfCups) => {
  const teaCups = [];

  for(let cups = 1; cups <= numOfCups; cups += 1) {
    const teaCup = prepareTea();
    teaCups.push(teaCup);
  }

  return teaCups;
};

// Add your code below this line

const tea4GreenTeamFCC = null; // :(
const tea4BlackTeamFCC = null; // :(

// Add your code above this line

console.log(
  tea4GreenTeamFCC,
  tea4BlackTeamFCC
);
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

# 3. Understand the Hazards of Using Imperative Code

## Description
<section id='description'>
Functional programming is a good habit. It keeps your code easy to manage, and saves you from sneaky bugs. But before we get there, let's look at an imperative approach to programming to highlight where you may have issues.
In English (and many other languages), the imperative tense is used to give commands. Similarly, an imperative style in programming is one that gives the computer a set of statements to perform a task.
Often the statements change the state of the program, like updating global variables. A classic example is writing a <code>for</code> loop that gives exact directions to iterate over the indices of an array.
In contrast, functional programming is a form of declarative programming. You tell the computer what you want done by calling a method or function.
JavaScript offers many predefined methods that handle common tasks so you don't need to write out how the computer should perform them. For example, instead of using the <code>for</code> loop mentioned above, you could call the <code>map</code> method which handles the details of iterating over an array. This helps to avoid semantic errors, like the "Off By One Errors" that were covered in the Debugging section.
Consider the scenario: you are browsing the web in your browser, and want to track the tabs you have opened. Let's try to model this using some simple object-oriented code.
A Window object is made up of tabs, and you usually have more than one Window open. The titles of each open site in each Window object is held in an array. After working in the browser (opening new tabs, merging windows, and closing tabs), you want to print the tabs that are still open. Closed tabs are removed from the array and new tabs (for simplicity) get added to the end of it.
The code editor shows an implementation of this functionality with functions for <code>tabOpen()</code>, <code>tabClose()</code>, and <code>join()</code>. The array <code>tabs</code> is part of the Window object that stores the name of the open pages.
<h4>Instructions<h4>
Run the code in the editor. It's using a method that has side effects in the program, causing incorrect output. The final list of open tabs should be <code>['FB', 'Gitter', 'Reddit', 'Twitter', 'Medium', 'new tab', 'Netflix', 'YouTube', 'Vine', 'GMail', 'Work mail', 'Docs', 'freeCodeCamp', 'new tab']</code> but the output will be slightly different.
Work through the code and see if you can figure out the problem, then advance to the next challenge to learn more.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// tabs is an array of titles of each site open within the window
var Window = function(tabs) {
  this.tabs = tabs; // we keep a record of the array inside the object
};

// When you join two windows into one window
Window.prototype.join = function (otherWindow) {
  this.tabs = this.tabs.concat(otherWindow.tabs);
  return this;
};

// When you open a new tab at the end
Window.prototype.tabOpen = function (tab) {
  this.tabs.push('new tab'); // let's open a new tab for now
  return this;
};

// When you close a tab
Window.prototype.tabClose = function (index) {
  var tabsBeforeIndex = this.tabs.splice(0, index); // get the tabs before the tab
  var tabsAfterIndex = this.tabs.splice(index); // get the tabs after the tab

  this.tabs = tabsBeforeIndex.concat(tabsAfterIndex); // join them together
  return this;
 };

// Let's create three browser windows
var workWindow = new Window(['GMail', 'Inbox', 'Work mail', 'Docs', 'freeCodeCamp']); // Your mailbox, drive, and other work sites
var socialWindow = new Window(['FB', 'Gitter', 'Reddit', 'Twitter', 'Medium']); // Social sites
var videoWindow = new Window(['Netflix', 'YouTube', 'Vimeo', 'Vine']); //  Entertainment sites

// Now perform the tab opening, closing, and other operations
var finalTabs = socialWindow
                    .tabOpen() // Open a new tab for cat memes
                    .join(videoWindow.tabClose(2)) // Close third tab in video window, and join
                    .join(workWindow.tabClose(1).tabOpen());

alert(finalTabs.tabs);
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

# 4. Avoid Mutations and Side Effects Using Functional Programming

## Description
<section id='description'>
If you haven't already figured it out, the issue in the previous challenge was with the <code>splice</code> call in the <code>tabClose()</code> function. Unfortunately, <code>splice</code> changes the original array it is called on, so the second call to it used a modified array, and gave unexpected results.
This is a small example of a much larger pattern - you call a function on a variable, array, or an object, and the function changes the variable or something in the object.
One of the core principles of functional programming is to not change things. Changes lead to bugs. It's easier to prevent bugs knowing that your functions don't change anything, including the function arguments or any global variable.
The previous example didn't have any complicated operations but the <code>splice</code> method changed the original array, and resulted in a bug.
Recall that in functional programming, changing or altering things is called <code>mutation</code>, and the outcome is called a <code>side effect</code>. A function, ideally, should be a <code>pure function</code>, meaning that it does not cause any side effects.
Let's try to master this discipline and not alter any variable or object in our code.
</section>

## Instructions
<section id='instructions'>
Fill in the code for the function <code>incrementer</code> so it returns the value of the global variable <code>fixedValue</code> increased by one.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// the global variable
var fixedValue = 4;

function incrementer () {
  // Add your code below this line


  // Add your code above this line
}

var newValue = incrementer(); // Should equal 5
console.log(fixedValue); // Should print 4
```

</div>



</section>

## Solution
<section id='solution'>

```js
var fixedValue = 4

function incrementer() {
  return fixedValue + 1
}

var newValue = incrementer(); // Should equal 5
```
</section>
<hr>

# 5. Pass Arguments to Avoid External Dependence in a Function

## Description
<section id='description'>
The last challenge was a step closer to functional programming principles, but there is still something missing.
We didn't alter the global variable value, but the function <code>incrementer</code> would not work without the global variable <code>fixedValue</code> being there.
Another principle of functional programming is to always declare your dependencies explicitly. This means if a function depends on a variable or object being present, then pass that variable or object directly into the function as an argument.
There are several good consequences from this principle. The function is easier to test, you know exactly what input it takes, and it won't depend on anything else in your program.
This can give you more confidence when you alter, remove, or add new code. You would know what you can or cannot change and you can see where the potential traps are.
Finally, the function would always produce the same output for the same set of inputs, no matter what part of the code executes it.
</section>

## Instructions
<section id='instructions'>
Let's update the <code>incrementer</code> function to clearly declare its dependencies.
Write the <code>incrementer</code> function so it takes an argument, and then increases the value by one.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// the global variable
var fixedValue = 4;

// Add your code below this line
function incrementer () {


  // Add your code above this line
}

var newValue = incrementer(fixedValue); // Should equal 5
console.log(fixedValue); // Should print 4
```

</div>



</section>

## Solution
<section id='solution'>

```js
// the global variable
var fixedValue = 4;

const incrementer = val => val + 1;

var newValue = incrementer(fixedValue); // Should equal 5
console.log(fixedValue); // Should print 4
```
</section>
<hr>

# 6. Refactor Global Variables Out of Functions

## Description
<section id='description'>
So far, we have seen two distinct principles for functional programming:
1) Don't alter a variable or object - create new variables and objects and return them if need be from a function.
2) Declare function arguments - any computation inside a function depends only on the arguments, and not on any global object or variable.
Adding one to a number is not very exciting, but we can apply these principles when working with arrays or more complex objects.
</section>

## Instructions
<section id='instructions'>
Rewrite the code so the global array <code>bookList</code> is not changed inside either function. The <code>add</code> function should add the given <code>bookName</code> to the end of an array. The <code>remove</code> function should remove the given <code>bookName</code> from an array. Both functions should return an array, and any new parameters should be added before the <code>bookName</code> parameter.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// the global variable
var bookList = ["The Hound of the Baskervilles", "On The Electrodynamics of Moving Bodies", "Philosophiæ Naturalis Principia Mathematica", "Disquisitiones Arithmeticae"];

/*This function should add a book to the list and return the list */
// New parameters should come before bookName

// Add your code below this line
function add (bookName) {

  bookList.push(bookName);
  return bookList;
  
  // Add your code above this line
}

/*This function should remove a book from the list and return the list */
// New parameters should come before the bookName one

// Add your code below this line
function remove (bookName) {
  var book_index = bookList.indexOf(bookName);
  if (book_index >= 0) {

    bookList.splice(book_index, 1);
    return bookList;

    // Add your code above this line
    }
}

var newBookList = add(bookList, 'A Brief History of Time');
var newerBookList = remove(bookList, 'On The Electrodynamics of Moving Bodies');
var newestBookList = remove(add(bookList, 'A Brief History of Time'), 'On The Electrodynamics of Moving Bodies');

console.log(bookList);
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

# 7. Use the map Method to Extract Data from an Array

## Description
<section id='description'>
So far we have learned to use pure functions to avoid side effects in a program. Also, we have seen the value in having a function only depend on its input arguments.
This is only the beginning. As its name suggests, functional programming is centered around a theory of functions.
It would make sense to be able to pass them as arguments to other functions, and return a function from another function. Functions are considered <code>First Class Objects</code> in JavaScript, which means they can be used like any other object. They can be saved in variables, stored in an object, or passed as function arguments.
Let's start with some simple array functions, which are methods on the array object prototype. In this exercise we are looking at <code>Array.prototype.map()</code>, or more simply <code>map</code>.
Remember that the <code>map</code> method is a way to iterate over each item in an array. It creates a new array (without changing the original one) after applying a callback function to every element.
</section>

## Instructions
<section id='instructions'>
The <code>watchList</code> array holds objects with information on several movies. Use <code>map</code> to pull the title and rating from <code>watchList</code> and save the new array in the <code>rating</code> variable. The code in the editor currently uses a <code>for</code> loop to do this, replace the loop functionality with your <code>map</code> expression.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// the global variable
var watchList = [
                 {
                   "Title": "Inception",
                   "Year": "2010",
                   "Rated": "PG-13",
                   "Released": "16 Jul 2010",
                   "Runtime": "148 min",
                   "Genre": "Action, Adventure, Crime",
                   "Director": "Christopher Nolan",
                   "Writer": "Christopher Nolan",
                   "Actors": "Leonardo DiCaprio, Joseph Gordon-Levitt, Ellen Page, Tom Hardy",
                   "Plot": "A thief, who steals corporate secrets through use of dream-sharing technology, is given the inverse task of planting an idea into the mind of a CEO.",
                   "Language": "English, Japanese, French",
                   "Country": "USA, UK",
                   "Awards": "Won 4 Oscars. Another 143 wins & 198 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMjAxMzY3NjcxNF5BMl5BanBnXkFtZTcwNTI5OTM0Mw@@._V1_SX300.jpg",
                   "Metascore": "74",
                   "imdbRating": "8.8",
                   "imdbVotes": "1,446,708",
                   "imdbID": "tt1375666",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Interstellar",
                   "Year": "2014",
                   "Rated": "PG-13",
                   "Released": "07 Nov 2014",
                   "Runtime": "169 min",
                   "Genre": "Adventure, Drama, Sci-Fi",
                   "Director": "Christopher Nolan",
                   "Writer": "Jonathan Nolan, Christopher Nolan",
                   "Actors": "Ellen Burstyn, Matthew McConaughey, Mackenzie Foy, John Lithgow",
                   "Plot": "A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival.",
                   "Language": "English",
                   "Country": "USA, UK",
                   "Awards": "Won 1 Oscar. Another 39 wins & 132 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMjIxNTU4MzY4MF5BMl5BanBnXkFtZTgwMzM4ODI3MjE@._V1_SX300.jpg",
                   "Metascore": "74",
                   "imdbRating": "8.6",
                   "imdbVotes": "910,366",
                   "imdbID": "tt0816692",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "The Dark Knight",
                   "Year": "2008",
                   "Rated": "PG-13",
                   "Released": "18 Jul 2008",
                   "Runtime": "152 min",
                   "Genre": "Action, Adventure, Crime",
                   "Director": "Christopher Nolan",
                   "Writer": "Jonathan Nolan (screenplay), Christopher Nolan (screenplay), Christopher Nolan (story), David S. Goyer (story), Bob Kane (characters)",
                   "Actors": "Christian Bale, Heath Ledger, Aaron Eckhart, Michael Caine",
                   "Plot": "When the menace known as the Joker wreaks havoc and chaos on the people of Gotham, the caped crusader must come to terms with one of the greatest psychological tests of his ability to fight injustice.",
                   "Language": "English, Mandarin",
                   "Country": "USA, UK",
                   "Awards": "Won 2 Oscars. Another 146 wins & 142 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMTMxNTMwODM0NF5BMl5BanBnXkFtZTcwODAyMTk2Mw@@._V1_SX300.jpg",
                   "Metascore": "82",
                   "imdbRating": "9.0",
                   "imdbVotes": "1,652,832",
                   "imdbID": "tt0468569",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Batman Begins",
                   "Year": "2005",
                   "Rated": "PG-13",
                   "Released": "15 Jun 2005",
                   "Runtime": "140 min",
                   "Genre": "Action, Adventure",
                   "Director": "Christopher Nolan",
                   "Writer": "Bob Kane (characters), David S. Goyer (story), Christopher Nolan (screenplay), David S. Goyer (screenplay)",
                   "Actors": "Christian Bale, Michael Caine, Liam Neeson, Katie Holmes",
                   "Plot": "After training with his mentor, Batman begins his fight to free crime-ridden Gotham City from the corruption that Scarecrow and the League of Shadows have cast upon it.",
                   "Language": "English, Urdu, Mandarin",
                   "Country": "USA, UK",
                   "Awards": "Nominated for 1 Oscar. Another 15 wins & 66 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BNTM3OTc0MzM2OV5BMl5BanBnXkFtZTYwNzUwMTI3._V1_SX300.jpg",
                   "Metascore": "70",
                   "imdbRating": "8.3",
                   "imdbVotes": "972,584",
                   "imdbID": "tt0372784",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Avatar",
                   "Year": "2009",
                   "Rated": "PG-13",
                   "Released": "18 Dec 2009",
                   "Runtime": "162 min",
                   "Genre": "Action, Adventure, Fantasy",
                   "Director": "James Cameron",
                   "Writer": "James Cameron",
                   "Actors": "Sam Worthington, Zoe Saldana, Sigourney Weaver, Stephen Lang",
                   "Plot": "A paraplegic marine dispatched to the moon Pandora on a unique mission becomes torn between following his orders and protecting the world he feels is his home.",
                   "Language": "English, Spanish",
                   "Country": "USA, UK",
                   "Awards": "Won 3 Oscars. Another 80 wins & 121 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMTYwOTEwNjAzMl5BMl5BanBnXkFtZTcwODc5MTUwMw@@._V1_SX300.jpg",
                   "Metascore": "83",
                   "imdbRating": "7.9",
                   "imdbVotes": "876,575",
                   "imdbID": "tt0499549",
                   "Type": "movie",
                   "Response": "True"
                }
];

// Add your code below this line

var rating = [];
for(var i=0; i < watchList.length; i++){
  rating.push({title: watchList[i]["Title"],  rating: watchList[i]["imdbRating"]});
}

// Add your code above this line

console.log(JSON.stringify(rating));
```

</div>



</section>

## Solution
<section id='solution'>

```js
// the global variable
var watchList = [
                 {
                   "Title": "Inception",
                   "Year": "2010",
                   "Rated": "PG-13",
                   "Released": "16 Jul 2010",
                   "Runtime": "148 min",
                   "Genre": "Action, Adventure, Crime",
                   "Director": "Christopher Nolan",
                   "Writer": "Christopher Nolan",
                   "Actors": "Leonardo DiCaprio, Joseph Gordon-Levitt, Ellen Page, Tom Hardy",
                   "Plot": "A thief, who steals corporate secrets through use of dream-sharing technology, is given the inverse task of planting an idea into the mind of a CEO.",
                   "Language": "English, Japanese, French",
                   "Country": "USA, UK",
                   "Awards": "Won 4 Oscars. Another 143 wins & 198 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMjAxMzY3NjcxNF5BMl5BanBnXkFtZTcwNTI5OTM0Mw@@._V1_SX300.jpg",
                   "Metascore": "74",
                   "imdbRating": "8.8",
                   "imdbVotes": "1,446,708",
                   "imdbID": "tt1375666",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Interstellar",
                   "Year": "2014",
                   "Rated": "PG-13",
                   "Released": "07 Nov 2014",
                   "Runtime": "169 min",
                   "Genre": "Adventure, Drama, Sci-Fi",
                   "Director": "Christopher Nolan",
                   "Writer": "Jonathan Nolan, Christopher Nolan",
                   "Actors": "Ellen Burstyn, Matthew McConaughey, Mackenzie Foy, John Lithgow",
                   "Plot": "A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival.",
                   "Language": "English",
                   "Country": "USA, UK",
                   "Awards": "Won 1 Oscar. Another 39 wins & 132 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMjIxNTU4MzY4MF5BMl5BanBnXkFtZTgwMzM4ODI3MjE@._V1_SX300.jpg",
                   "Metascore": "74",
                   "imdbRating": "8.6",
                   "imdbVotes": "910,366",
                   "imdbID": "tt0816692",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "The Dark Knight",
                   "Year": "2008",
                   "Rated": "PG-13",
                   "Released": "18 Jul 2008",
                   "Runtime": "152 min",
                   "Genre": "Action, Adventure, Crime",
                   "Director": "Christopher Nolan",
                   "Writer": "Jonathan Nolan (screenplay), Christopher Nolan (screenplay), Christopher Nolan (story), David S. Goyer (story), Bob Kane (characters)",
                   "Actors": "Christian Bale, Heath Ledger, Aaron Eckhart, Michael Caine",
                   "Plot": "When the menace known as the Joker wreaks havoc and chaos on the people of Gotham, the caped crusader must come to terms with one of the greatest psychological tests of his ability to fight injustice.",
                   "Language": "English, Mandarin",
                   "Country": "USA, UK",
                   "Awards": "Won 2 Oscars. Another 146 wins & 142 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMTMxNTMwODM0NF5BMl5BanBnXkFtZTcwODAyMTk2Mw@@._V1_SX300.jpg",
                   "Metascore": "82",
                   "imdbRating": "9.0",
                   "imdbVotes": "1,652,832",
                   "imdbID": "tt0468569",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Batman Begins",
                   "Year": "2005",
                   "Rated": "PG-13",
                   "Released": "15 Jun 2005",
                   "Runtime": "140 min",
                   "Genre": "Action, Adventure",
                   "Director": "Christopher Nolan",
                   "Writer": "Bob Kane (characters), David S. Goyer (story), Christopher Nolan (screenplay), David S. Goyer (screenplay)",
                   "Actors": "Christian Bale, Michael Caine, Liam Neeson, Katie Holmes",
                   "Plot": "After training with his mentor, Batman begins his fight to free crime-ridden Gotham City from the corruption that Scarecrow and the League of Shadows have cast upon it.",
                   "Language": "English, Urdu, Mandarin",
                   "Country": "USA, UK",
                   "Awards": "Nominated for 1 Oscar. Another 15 wins & 66 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BNTM3OTc0MzM2OV5BMl5BanBnXkFtZTYwNzUwMTI3._V1_SX300.jpg",
                   "Metascore": "70",
                   "imdbRating": "8.3",
                   "imdbVotes": "972,584",
                   "imdbID": "tt0372784",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Avatar",
                   "Year": "2009",
                   "Rated": "PG-13",
                   "Released": "18 Dec 2009",
                   "Runtime": "162 min",
                   "Genre": "Action, Adventure, Fantasy",
                   "Director": "James Cameron",
                   "Writer": "James Cameron",
                   "Actors": "Sam Worthington, Zoe Saldana, Sigourney Weaver, Stephen Lang",
                   "Plot": "A paraplegic marine dispatched to the moon Pandora on a unique mission becomes torn between following his orders and protecting the world he feels is his home.",
                   "Language": "English, Spanish",
                   "Country": "USA, UK",
                   "Awards": "Won 3 Oscars. Another 80 wins & 121 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMTYwOTEwNjAzMl5BMl5BanBnXkFtZTcwODc5MTUwMw@@._V1_SX300.jpg",
                   "Metascore": "83",
                   "imdbRating": "7.9",
                   "imdbVotes": "876,575",
                   "imdbID": "tt0499549",
                   "Type": "movie",
                   "Response": "True"
                }
];

var rating = watchList.map(function(movie) {
  return {
    title: movie["Title"],
    rating: movie["imdbRating"]
  }
});
```
</section>
<hr>

# 8. Implement map on a Prototype

## Description
<section id='description'>
As you have seen from applying <code>Array.prototype.map()</code>, or simply <code>map()</code> earlier, the <code>map</code> method returns an array of the same length as the one it was called on. It also doesn't alter the original array, as long as its callback function doesn't.
In other words, <code>map</code> is a pure function, and its output depends solely on its inputs. Plus, it takes another function as its argument.
It would teach us a lot about <code>map</code> to try to implement a version of it that behaves exactly like the <code>Array.prototype.map()</code> with a <code>for</code> loop or <code>Array.prototype.forEach()</code>.
Note: A pure function is allowed to alter local variables defined within its scope, although, it's preferable to avoid that as well.
</section>

## Instructions
<section id='instructions'>
Write your own <code>Array.prototype.myMap()</code>, which should behave exactly like <code>Array.prototype.map()</code>. You may use a <code>for</code> loop or the <code>forEach</code> method.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// the global Array
var s = [23, 65, 98, 5];

Array.prototype.myMap = function(callback){
  var newArray = [];
  // Add your code below this line

  // Add your code above this line
  return newArray;

};

var new_s = s.myMap(function(item){
  return item *2;
});
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

# 9. Use the filter Method to Extract Data from an Array

## Description
<section id='description'>
Another useful array function is <code>Array.prototype.filter()</code>, or simply <code>filter()</code>. The <code>filter</code> method returns a new array which is at most as long as the original array, but usually has fewer items.
<code>Filter</code> doesn't alter the original array, just like <code>map</code>. It takes a callback function that applies the logic inside the callback on each element of the array. If an element returns true based on the criteria in the callback function, then it is included in the new array.
</section>

## Instructions
<section id='instructions'>
The variable <code>watchList</code> holds an array of objects with information on several movies. Use a combination of <code>filter</code> and <code>map</code> to return a new array of objects with only <code>title</code> and <code>rating</code> keys, but where <code>imdbRating</code> is greater than or equal to 8.0. Note that the rating values are saved as strings in the object and you may want to convert them into numbers to perform mathematical operations on them.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// the global variable
var watchList = [
                 {
                   "Title": "Inception",
                   "Year": "2010",
                   "Rated": "PG-13",
                   "Released": "16 Jul 2010",
                   "Runtime": "148 min",
                   "Genre": "Action, Adventure, Crime",
                   "Director": "Christopher Nolan",
                   "Writer": "Christopher Nolan",
                   "Actors": "Leonardo DiCaprio, Joseph Gordon-Levitt, Ellen Page, Tom Hardy",
                   "Plot": "A thief, who steals corporate secrets through use of dream-sharing technology, is given the inverse task of planting an idea into the mind of a CEO.",
                   "Language": "English, Japanese, French",
                   "Country": "USA, UK",
                   "Awards": "Won 4 Oscars. Another 143 wins & 198 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMjAxMzY3NjcxNF5BMl5BanBnXkFtZTcwNTI5OTM0Mw@@._V1_SX300.jpg",
                   "Metascore": "74",
                   "imdbRating": "8.8",
                   "imdbVotes": "1,446,708",
                   "imdbID": "tt1375666",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Interstellar",
                   "Year": "2014",
                   "Rated": "PG-13",
                   "Released": "07 Nov 2014",
                   "Runtime": "169 min",
                   "Genre": "Adventure, Drama, Sci-Fi",
                   "Director": "Christopher Nolan",
                   "Writer": "Jonathan Nolan, Christopher Nolan",
                   "Actors": "Ellen Burstyn, Matthew McConaughey, Mackenzie Foy, John Lithgow",
                   "Plot": "A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival.",
                   "Language": "English",
                   "Country": "USA, UK",
                   "Awards": "Won 1 Oscar. Another 39 wins & 132 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMjIxNTU4MzY4MF5BMl5BanBnXkFtZTgwMzM4ODI3MjE@._V1_SX300.jpg",
                   "Metascore": "74",
                   "imdbRating": "8.6",
                   "imdbVotes": "910,366",
                   "imdbID": "tt0816692",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "The Dark Knight",
                   "Year": "2008",
                   "Rated": "PG-13",
                   "Released": "18 Jul 2008",
                   "Runtime": "152 min",
                   "Genre": "Action, Adventure, Crime",
                   "Director": "Christopher Nolan",
                   "Writer": "Jonathan Nolan (screenplay), Christopher Nolan (screenplay), Christopher Nolan (story), David S. Goyer (story), Bob Kane (characters)",
                   "Actors": "Christian Bale, Heath Ledger, Aaron Eckhart, Michael Caine",
                   "Plot": "When the menace known as the Joker wreaks havoc and chaos on the people of Gotham, the caped crusader must come to terms with one of the greatest psychological tests of his ability to fight injustice.",
                   "Language": "English, Mandarin",
                   "Country": "USA, UK",
                   "Awards": "Won 2 Oscars. Another 146 wins & 142 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMTMxNTMwODM0NF5BMl5BanBnXkFtZTcwODAyMTk2Mw@@._V1_SX300.jpg",
                   "Metascore": "82",
                   "imdbRating": "9.0",
                   "imdbVotes": "1,652,832",
                   "imdbID": "tt0468569",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Batman Begins",
                   "Year": "2005",
                   "Rated": "PG-13",
                   "Released": "15 Jun 2005",
                   "Runtime": "140 min",
                   "Genre": "Action, Adventure",
                   "Director": "Christopher Nolan",
                   "Writer": "Bob Kane (characters), David S. Goyer (story), Christopher Nolan (screenplay), David S. Goyer (screenplay)",
                   "Actors": "Christian Bale, Michael Caine, Liam Neeson, Katie Holmes",
                   "Plot": "After training with his mentor, Batman begins his fight to free crime-ridden Gotham City from the corruption that Scarecrow and the League of Shadows have cast upon it.",
                   "Language": "English, Urdu, Mandarin",
                   "Country": "USA, UK",
                   "Awards": "Nominated for 1 Oscar. Another 15 wins & 66 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BNTM3OTc0MzM2OV5BMl5BanBnXkFtZTYwNzUwMTI3._V1_SX300.jpg",
                   "Metascore": "70",
                   "imdbRating": "8.3",
                   "imdbVotes": "972,584",
                   "imdbID": "tt0372784",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Avatar",
                   "Year": "2009",
                   "Rated": "PG-13",
                   "Released": "18 Dec 2009",
                   "Runtime": "162 min",
                   "Genre": "Action, Adventure, Fantasy",
                   "Director": "James Cameron",
                   "Writer": "James Cameron",
                   "Actors": "Sam Worthington, Zoe Saldana, Sigourney Weaver, Stephen Lang",
                   "Plot": "A paraplegic marine dispatched to the moon Pandora on a unique mission becomes torn between following his orders and protecting the world he feels is his home.",
                   "Language": "English, Spanish",
                   "Country": "USA, UK",
                   "Awards": "Won 3 Oscars. Another 80 wins & 121 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMTYwOTEwNjAzMl5BMl5BanBnXkFtZTcwODc5MTUwMw@@._V1_SX300.jpg",
                   "Metascore": "83",
                   "imdbRating": "7.9",
                   "imdbVotes": "876,575",
                   "imdbID": "tt0499549",
                   "Type": "movie",
                   "Response": "True"
                }
];

// Add your code below this line

var filteredList;

// Add your code above this line

console.log(filteredList);
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

# 10. Implement the filter Method on a Prototype

## Description
<section id='description'>
It would teach us a lot about the <code>filter</code> method if we try to implement a version of it that behaves exactly like <code>Array.prototype.filter()</code>. It can use either a <code>for</code> loop or <code>Array.prototype.forEach()</code>.
Note: A pure function is allowed to alter local variables defined within its scope, although, it's preferable to avoid that as well.
</section>

## Instructions
<section id='instructions'>
Write your own <code>Array.prototype.myFilter()</code>, which should behave exactly like <code>Array.prototype.filter()</code>. You may use a <code>for</code> loop or the <code>Array.prototype.forEach()</code> method.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// the global Array
var s = [23, 65, 98, 5];

Array.prototype.myFilter = function(callback){
  var newArray = [];
  // Add your code below this line

  // Add your code above this line
  return newArray;

};

var new_s = s.myFilter(function(item){
  return item % 2 === 1;
});
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

# 11. Return Part of an Array Using the slice Method

## Description
<section id='description'>
The <code>slice</code> method returns a copy of certain elements of an array. It can take two arguments, the first gives the index of where to begin the slice, the second is the index for where to end the slice (and it's non-inclusive). If the arguments are not provided, the default is to start at the beginning of the array through the end, which is an easy way to make a copy of the entire array. The <code>slice</code> method does not mutate the original array, but returns a new one.
Here's an example:
<blockquote>var arr = ["Cat", "Dog", "Tiger", "Zebra"];<br>var newArray = arr.slice(1, 3);<br>// Sets newArray to ["Dog", "Tiger"]</blockquote>
</section>

## Instructions
<section id='instructions'>
Use the <code>slice</code> method in the <code>sliceArray</code> function to return part of the <code>anim</code> array given the provided <code>beginSlice</code> and <code>endSlice</code> indices. The function should return an array.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function sliceArray(anim, beginSlice, endSlice) {
  // Add your code below this line


  // Add your code above this line
}
var inputAnim = ["Cat", "Dog", "Tiger", "Zebra", "Ant"];
sliceArray(inputAnim, 1, 3);
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

# 12. Remove Elements from an Array Using slice Instead of splice

## Description
<section id='description'>
A common pattern while working with arrays is when you want to remove items and keep the rest of the array. JavaScript offers the <code>splice</code> method for this, which takes arguments for the index of where to start removing items, then the number of items to remove. If the second argument is not provided, the default is to remove items through the end. However, the <code>splice</code> method mutates the original array it is called on. Here's an example:
<blockquote>var cities = ["Chicago", "Delhi", "Islamabad", "London", "Berlin"];<br>cities.splice(3, 1); // Returns "London" and deletes it from the cities array<br>// cities is now ["Chicago", "Delhi", "Islamabad", "Berlin"]</blockquote>
As we saw in the last challenge, the <code>slice</code> method does not mutate the original array, but returns a new one which can be saved into a variable. Recall that the <code>slice</code> method takes two arguments for the indices to begin and end the slice (the end is non-inclusive), and returns those items in a new array. Using the <code>slice</code> method instead of <code>splice</code> helps to avoid any array-mutating side effects.
</section>

## Instructions
<section id='instructions'>
Rewrite the function <code>nonMutatingSplice</code> by using <code>slice</code> instead of <code>splice</code>. It should limit the provided <code>cities</code> array to a length of 3, and return a new array with only the first three items.
Do not mutate the original array provided to the function.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function nonMutatingSplice(cities) {
  // Add your code below this line
  return cities.splice(3);

  // Add your code above this line
}
var inputCities = ["Chicago", "Delhi", "Islamabad", "London", "Berlin"];
nonMutatingSplice(inputCities);
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

# 13. Combine Two Arrays Using the concat Method

## Description
<section id='description'>
<code>Concatenation</code> means to join items end to end. JavaScript offers the <code>concat</code> method for both strings and arrays that work in the same way. For arrays, the method is called on one, then another array is provided as the argument to <code>concat</code>, which is added to the end of the first array. It returns a new array and does not mutate either of the original arrays. Here's an example:
<blockquote>[1, 2, 3].concat([4, 5, 6]);<br>// Returns a new array [1, 2, 3, 4, 5, 6]</blockquote>
</section>

## Instructions
<section id='instructions'>
Use the <code>concat</code> method in the <code>nonMutatingConcat</code> function to concatenate <code>attach</code> to the end of <code>original</code>. The function should return the concatenated array.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function nonMutatingConcat(original, attach) {
  // Add your code below this line


  // Add your code above this line
}
var first = [1, 2, 3];
var second = [4, 5];
nonMutatingConcat(first, second);
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

# 14. Add Elements to the End of an Array Using concat Instead of push

## Description
<section id='description'>
Functional programming is all about creating and using non-mutating functions.
The last challenge introduced the <code>concat</code> method as a way to combine arrays into a new one without mutating the original arrays. Compare <code>concat</code> to the <code>push</code> method. <code>Push</code> adds an item to the end of the same array it is called on, which mutates that array. Here's an example:
<blockquote>var arr = [1, 2, 3];<br>arr.push([4, 5, 6]);<br>// arr is changed to [1, 2, 3, [4, 5, 6]]<br>// Not the functional programming way</blockquote>
<code>Concat</code> offers a way to add new items to the end of an array without any mutating side effects.
</section>

## Instructions
<section id='instructions'>
Change the <code>nonMutatingPush</code> function so it uses <code>concat</code> to add <code>newItem</code> to the end of <code>original</code> instead of <code>push</code>. The function should return an array.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function nonMutatingPush(original, newItem) {
  // Add your code below this line
  return original.push(newItem);

  // Add your code above this line
}
var first = [1, 2, 3];
var second = [4, 5];
nonMutatingPush(first, second);
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

# 15. Use the reduce Method to Analyze Data

## Description
<section id='description'>
<code>Array.prototype.reduce()</code>, or simply <code>reduce()</code>, is the most general of all array operations in JavaScript. You can solve almost any array processing problem using the <code>reduce</code> method.
This is not the case with the <code>filter</code> and <code>map</code> methods since they do not allow interaction between two different elements of the array. For example, if you want to compare elements of the array, or add them together, <code>filter</code> or <code>map</code> could not process that.
The <code>reduce</code> method allows for more general forms of array processing, and it's possible to show that both <code>filter</code> and <code>map</code> can be derived as a special application of <code>reduce</code>.
However, before we get there, let's practice using <code>reduce</code> first.
</section>

## Instructions
<section id='instructions'>
The variable <code>watchList</code> holds an array of objects with information on several movies. Use <code>reduce</code> to find the average IMDB rating of the movies <strong>directed by Christopher Nolan</strong>. Recall from prior challenges how to <code>filter</code> data and <code>map</code> over it to pull what you need. You may need to create other variables, and return the average rating from <code>getRating</code> function. Note that the rating values are saved as strings in the object and need to be converted into numbers before they are used in any mathematical operations.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// the global variable
var watchList = [
                 {
                   "Title": "Inception",
                   "Year": "2010",
                   "Rated": "PG-13",
                   "Released": "16 Jul 2010",
                   "Runtime": "148 min",
                   "Genre": "Action, Adventure, Crime",
                   "Director": "Christopher Nolan",
                   "Writer": "Christopher Nolan",
                   "Actors": "Leonardo DiCaprio, Joseph Gordon-Levitt, Ellen Page, Tom Hardy",
                   "Plot": "A thief, who steals corporate secrets through use of dream-sharing technology, is given the inverse task of planting an idea into the mind of a CEO.",
                   "Language": "English, Japanese, French",
                   "Country": "USA, UK",
                   "Awards": "Won 4 Oscars. Another 143 wins & 198 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMjAxMzY3NjcxNF5BMl5BanBnXkFtZTcwNTI5OTM0Mw@@._V1_SX300.jpg",
                   "Metascore": "74",
                   "imdbRating": "8.8",
                   "imdbVotes": "1,446,708",
                   "imdbID": "tt1375666",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Interstellar",
                   "Year": "2014",
                   "Rated": "PG-13",
                   "Released": "07 Nov 2014",
                   "Runtime": "169 min",
                   "Genre": "Adventure, Drama, Sci-Fi",
                   "Director": "Christopher Nolan",
                   "Writer": "Jonathan Nolan, Christopher Nolan",
                   "Actors": "Ellen Burstyn, Matthew McConaughey, Mackenzie Foy, John Lithgow",
                   "Plot": "A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival.",
                   "Language": "English",
                   "Country": "USA, UK",
                   "Awards": "Won 1 Oscar. Another 39 wins & 132 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMjIxNTU4MzY4MF5BMl5BanBnXkFtZTgwMzM4ODI3MjE@._V1_SX300.jpg",
                   "Metascore": "74",
                   "imdbRating": "8.6",
                   "imdbVotes": "910,366",
                   "imdbID": "tt0816692",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "The Dark Knight",
                   "Year": "2008",
                   "Rated": "PG-13",
                   "Released": "18 Jul 2008",
                   "Runtime": "152 min",
                   "Genre": "Action, Adventure, Crime",
                   "Director": "Christopher Nolan",
                   "Writer": "Jonathan Nolan (screenplay), Christopher Nolan (screenplay), Christopher Nolan (story), David S. Goyer (story), Bob Kane (characters)",
                   "Actors": "Christian Bale, Heath Ledger, Aaron Eckhart, Michael Caine",
                   "Plot": "When the menace known as the Joker wreaks havoc and chaos on the people of Gotham, the caped crusader must come to terms with one of the greatest psychological tests of his ability to fight injustice.",
                   "Language": "English, Mandarin",
                   "Country": "USA, UK",
                   "Awards": "Won 2 Oscars. Another 146 wins & 142 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMTMxNTMwODM0NF5BMl5BanBnXkFtZTcwODAyMTk2Mw@@._V1_SX300.jpg",
                   "Metascore": "82",
                   "imdbRating": "9.0",
                   "imdbVotes": "1,652,832",
                   "imdbID": "tt0468569",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Batman Begins",
                   "Year": "2005",
                   "Rated": "PG-13",
                   "Released": "15 Jun 2005",
                   "Runtime": "140 min",
                   "Genre": "Action, Adventure",
                   "Director": "Christopher Nolan",
                   "Writer": "Bob Kane (characters), David S. Goyer (story), Christopher Nolan (screenplay), David S. Goyer (screenplay)",
                   "Actors": "Christian Bale, Michael Caine, Liam Neeson, Katie Holmes",
                   "Plot": "After training with his mentor, Batman begins his fight to free crime-ridden Gotham City from the corruption that Scarecrow and the League of Shadows have cast upon it.",
                   "Language": "English, Urdu, Mandarin",
                   "Country": "USA, UK",
                   "Awards": "Nominated for 1 Oscar. Another 15 wins & 66 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BNTM3OTc0MzM2OV5BMl5BanBnXkFtZTYwNzUwMTI3._V1_SX300.jpg",
                   "Metascore": "70",
                   "imdbRating": "8.3",
                   "imdbVotes": "972,584",
                   "imdbID": "tt0372784",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Avatar",
                   "Year": "2009",
                   "Rated": "PG-13",
                   "Released": "18 Dec 2009",
                   "Runtime": "162 min",
                   "Genre": "Action, Adventure, Fantasy",
                   "Director": "James Cameron",
                   "Writer": "James Cameron",
                   "Actors": "Sam Worthington, Zoe Saldana, Sigourney Weaver, Stephen Lang",
                   "Plot": "A paraplegic marine dispatched to the moon Pandora on a unique mission becomes torn between following his orders and protecting the world he feels is his home.",
                   "Language": "English, Spanish",
                   "Country": "USA, UK",
                   "Awards": "Won 3 Oscars. Another 80 wins & 121 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMTYwOTEwNjAzMl5BMl5BanBnXkFtZTcwODc5MTUwMw@@._V1_SX300.jpg",
                   "Metascore": "83",
                   "imdbRating": "7.9",
                   "imdbVotes": "876,575",
                   "imdbID": "tt0499549",
                   "Type": "movie",
                   "Response": "True"
                }
];

function getRating(watchList){
  // Add your code below this line
  var averageRating;


  // Add your code above this line
  return averageRating;
}
console.log(getRating(watchList));
```

</div>



</section>

## Solution
<section id='solution'>

```js
// the global variable
var watchList = [
                 {
                   "Title": "Inception",
                   "Year": "2010",
                   "Rated": "PG-13",
                   "Released": "16 Jul 2010",
                   "Runtime": "148 min",
                   "Genre": "Action, Adventure, Crime",
                   "Director": "Christopher Nolan",
                   "Writer": "Christopher Nolan",
                   "Actors": "Leonardo DiCaprio, Joseph Gordon-Levitt, Ellen Page, Tom Hardy",
                   "Plot": "A thief, who steals corporate secrets through use of dream-sharing technology, is given the inverse task of planting an idea into the mind of a CEO.",
                   "Language": "English, Japanese, French",
                   "Country": "USA, UK",
                   "Awards": "Won 4 Oscars. Another 143 wins & 198 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMjAxMzY3NjcxNF5BMl5BanBnXkFtZTcwNTI5OTM0Mw@@._V1_SX300.jpg",
                   "Metascore": "74",
                   "imdbRating": "8.8",
                   "imdbVotes": "1,446,708",
                   "imdbID": "tt1375666",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Interstellar",
                   "Year": "2014",
                   "Rated": "PG-13",
                   "Released": "07 Nov 2014",
                   "Runtime": "169 min",
                   "Genre": "Adventure, Drama, Sci-Fi",
                   "Director": "Christopher Nolan",
                   "Writer": "Jonathan Nolan, Christopher Nolan",
                   "Actors": "Ellen Burstyn, Matthew McConaughey, Mackenzie Foy, John Lithgow",
                   "Plot": "A team of explorers travel through a wormhole in space in an attempt to ensure humanity's survival.",
                   "Language": "English",
                   "Country": "USA, UK",
                   "Awards": "Won 1 Oscar. Another 39 wins & 132 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMjIxNTU4MzY4MF5BMl5BanBnXkFtZTgwMzM4ODI3MjE@._V1_SX300.jpg",
                   "Metascore": "74",
                   "imdbRating": "8.6",
                   "imdbVotes": "910,366",
                   "imdbID": "tt0816692",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "The Dark Knight",
                   "Year": "2008",
                   "Rated": "PG-13",
                   "Released": "18 Jul 2008",
                   "Runtime": "152 min",
                   "Genre": "Action, Adventure, Crime",
                   "Director": "Christopher Nolan",
                   "Writer": "Jonathan Nolan (screenplay), Christopher Nolan (screenplay), Christopher Nolan (story), David S. Goyer (story), Bob Kane (characters)",
                   "Actors": "Christian Bale, Heath Ledger, Aaron Eckhart, Michael Caine",
                   "Plot": "When the menace known as the Joker wreaks havoc and chaos on the people of Gotham, the caped crusader must come to terms with one of the greatest psychological tests of his ability to fight injustice.",
                   "Language": "English, Mandarin",
                   "Country": "USA, UK",
                   "Awards": "Won 2 Oscars. Another 146 wins & 142 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMTMxNTMwODM0NF5BMl5BanBnXkFtZTcwODAyMTk2Mw@@._V1_SX300.jpg",
                   "Metascore": "82",
                   "imdbRating": "9.0",
                   "imdbVotes": "1,652,832",
                   "imdbID": "tt0468569",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Batman Begins",
                   "Year": "2005",
                   "Rated": "PG-13",
                   "Released": "15 Jun 2005",
                   "Runtime": "140 min",
                   "Genre": "Action, Adventure",
                   "Director": "Christopher Nolan",
                   "Writer": "Bob Kane (characters), David S. Goyer (story), Christopher Nolan (screenplay), David S. Goyer (screenplay)",
                   "Actors": "Christian Bale, Michael Caine, Liam Neeson, Katie Holmes",
                   "Plot": "After training with his mentor, Batman begins his fight to free crime-ridden Gotham City from the corruption that Scarecrow and the League of Shadows have cast upon it.",
                   "Language": "English, Urdu, Mandarin",
                   "Country": "USA, UK",
                   "Awards": "Nominated for 1 Oscar. Another 15 wins & 66 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BNTM3OTc0MzM2OV5BMl5BanBnXkFtZTYwNzUwMTI3._V1_SX300.jpg",
                   "Metascore": "70",
                   "imdbRating": "8.3",
                   "imdbVotes": "972,584",
                   "imdbID": "tt0372784",
                   "Type": "movie",
                   "Response": "True"
                },
                {
                   "Title": "Avatar",
                   "Year": "2009",
                   "Rated": "PG-13",
                   "Released": "18 Dec 2009",
                   "Runtime": "162 min",
                   "Genre": "Action, Adventure, Fantasy",
                   "Director": "James Cameron",
                   "Writer": "James Cameron",
                   "Actors": "Sam Worthington, Zoe Saldana, Sigourney Weaver, Stephen Lang",
                   "Plot": "A paraplegic marine dispatched to the moon Pandora on a unique mission becomes torn between following his orders and protecting the world he feels is his home.",
                   "Language": "English, Spanish",
                   "Country": "USA, UK",
                   "Awards": "Won 3 Oscars. Another 80 wins & 121 nominations.",
                   "Poster": "http://ia.media-imdb.com/images/M/MV5BMTYwOTEwNjAzMl5BMl5BanBnXkFtZTcwODc5MTUwMw@@._V1_SX300.jpg",
                   "Metascore": "83",
                   "imdbRating": "7.9",
                   "imdbVotes": "876,575",
                   "imdbID": "tt0499549",
                   "Type": "movie",
                   "Response": "True"
                }
];

function getRating(watchList){
  var averageRating;
  const rating = watchList
                  .filter(obj => obj.Director === "Christopher Nolan")
                  .map(obj => Number(obj.imdbRating));
  averageRating = rating.reduce((accum, curr) => accum + curr)/rating.length;
  return averageRating;
}

```
</section>
<hr>

# 16. Sort an Array Alphabetically using the sort Method

## Description
<section id='description'>
The <code>sort</code> method sorts the elements of an array according to the callback function.
For example:
<blockquote>function ascendingOrder(arr) {<br>&nbsp;&nbsp;return arr.sort(function(a, b) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return a - b;<br>&nbsp;&nbsp;});<br>}<br>ascendingOrder([1, 5, 2, 3, 4]);<br>// Returns [1, 2, 3, 4, 5]<br><br>function reverseAlpha(arr) {<br>&nbsp;&nbsp;return arr.sort(function(a, b) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return a === b ? 0 : a < b ? 1 : -1;<br>&nbsp;&nbsp;});<br>}<br>reverseAlpha(['l', 'h', 'z', 'b', 's']);<br>// Returns ['z', 's', 'l', 'h', 'b']</blockquote>
Note: It's encouraged to provide a callback function to specify how to sort the array items. JavaScript's default sorting method is by string Unicode point value, which may return unexpected results.
</section>

## Instructions
<section id='instructions'>
Use the <code>sort</code> method in the <code>alphabeticalOrder</code> function to sort the elements of <code>arr</code> in alphabetical order.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function alphabeticalOrder(arr) {
  // Add your code below this line


  // Add your code above this line
}
alphabeticalOrder(["a", "d", "c", "a", "z", "g"]);
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

# 17. Return a Sorted Array Without Changing the Original Array

## Description
<section id='description'>
A side effect of the <code>sort</code> method is that it changes the order of the elements in the original array. In other words, it mutates the array in place. One way to avoid this is to first concatenate an empty array to the one being sorted (remember that <code>concat</code> returns a new array), then run the <code>sort</code> method.
</section>

## Instructions
<section id='instructions'>
Use the <code>sort</code> method in the <code>nonMutatingSort</code> function to sort the elements of an array in ascending order. The function should return a new array, and not mutate the <code>globalArray</code> variable.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var globalArray = [5, 6, 3, 2, 9];
function nonMutatingSort(arr) {
  // Add your code below this line


  // Add your code above this line
}
nonMutatingSort(globalArray);
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

# 18. Split a String into an Array Using the split Method

## Description
<section id='description'>
The <code>split</code> method splits a string into an array of strings. It takes an argument for the delimiter, which can be a character to use to break up the string or a regular expression. For example, if the delimiter is a space, you get an array of words, and if the delimiter is an empty string, you get an array of each character in the string.
Here are two examples that split one string by spaces, then another by digits using a regular expression:
<blockquote>var str = "Hello World";<br>var bySpace = str.split(" ");<br>// Sets bySpace to ["Hello", "World"]<br><br>var otherString = "How9are7you2today";<br>var byDigits = otherString.split(/\d/);<br>// Sets byDigits to ["How", "are", "you", "today"]</blockquote>
Since strings are immutable, the <code>split</code> method makes it easier to work with them.
</section>

## Instructions
<section id='instructions'>
Use the <code>split</code> method inside the <code>splitify</code> function to split <code>str</code> into an array of words. The function should return the array. Note that the words are not always separated by spaces, and the array should not contain punctuation.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function splitify(str) {
  // Add your code below this line


  // Add your code above this line
}
splitify("Hello World,I-am code");
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

# 19. Combine an Array into a String Using the join Method

## Description
<section id='description'>
The <code>join</code> method is used to join the elements of an array together to create a string. It takes an argument for the delimiter that is used to separate the array elements in the string.
Here's an example:
<blockquote>var arr = ["Hello", "World"];<br>var str = arr.join(" ");<br>// Sets str to "Hello World"</blockquote>
</section>

## Instructions
<section id='instructions'>
Use the <code>join</code> method (among others) inside the <code>sentensify</code> function to make a sentence from the words in the string <code>str</code>. The function should return a string. For example, "I-like-Star-Wars" would be converted to "I like Star Wars". For this challenge, do not use the <code>replace</code> method.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function sentensify(str) {
  // Add your code below this line


  // Add your code above this line
}
sentensify("May-the-force-be-with-you");
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

# 20. Apply Functional Programming to Convert Strings to URL Slugs

## Description
<section id='description'>
The last several challenges covered a number of useful array and string methods that follow functional programming principles. We've also learned about <code>reduce</code>, which is a powerful method used to reduce problems to simpler forms. From computing averages to sorting, any array operation can be achieved by applying it. Recall that <code>map</code> and <code>filter</code> are special cases of <code>reduce</code>.
Let's combine what we've learned to solve a practical problem.
Many content management sites (CMS) have the titles of a post added to part of the URL for simple bookmarking purposes. For example, if you write a Medium post titled "Stop Using Reduce", it's likely the URL would have some form of the title string in it (".../stop-using-reduce"). You may have already noticed this on the freeCodeCamp site.
</section>

## Instructions
<section id='instructions'>
Fill in the <code>urlSlug</code> function so it converts a string <code>title</code> and returns the hyphenated version for the URL. You can use any of the methods covered in this section, and don't use <code>replace</code>. Here are the requirements:
The input is a string with spaces and title-cased words
The output is a string with the spaces between words replaced by a hyphen (<code>-</code>)
The output should be all lower-cased letters
The output should not have any spaces
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
// the global variable
var globalTitle = "Winter Is Coming";

// Add your code below this line
function urlSlug(title) {


}
// Add your code above this line

var winterComing = urlSlug(globalTitle); // Should be "winter-is-coming"
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

# 21. Use the every Method to Check that Every Element in an Array Meets a Criteria

## Description
<section id='description'>
The <code>every</code> method works with arrays to check if <em>every</em> element passes a particular test. It returns a Boolean value - <code>true</code> if all values meet the criteria, <code>false</code> if not.
For example, the following code would check if every element in the <code>numbers</code> array is less than 10:
<blockquote>var numbers = [1, 5, 8, 0, 10, 11];<br>numbers.every(function(currentValue) {<br>&nbsp;&nbsp;return currentValue < 10;<br>});<br>// Returns false</blockquote>
</section>

## Instructions
<section id='instructions'>
Use the <code>every</code> method inside the <code>checkPositive</code> function to check if every element in <code>arr</code> is positive. The function should return a Boolean value.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function checkPositive(arr) {
  // Add your code below this line


  // Add your code above this line
}
checkPositive([1, 2, 3, -4, 5]);
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

# 22. Use the some Method to Check that Any Elements in an Array Meet a Criteria

## Description
<section id='description'>
The <code>some</code> method works with arrays to check if <em>any</em> element passes a particular test. It returns a Boolean value - <code>true</code> if any of the values meet the criteria, <code>false</code> if not.
For example, the following code would check if any element in the <code>numbers</code> array is less than 10:
<blockquote>var numbers = [10, 50, 8, 220, 110, 11];<br>numbers.some(function(currentValue) {<br>&nbsp;&nbsp;return currentValue < 10;<br>});<br>// Returns true</blockquote>
</section>

## Instructions
<section id='instructions'>
Use the <code>some</code> method inside the <code>checkPositive</code> function to check if any element in <code>arr</code> is positive. The function should return a Boolean value.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function checkPositive(arr) {
  // Add your code below this line


  // Add your code above this line
}
checkPositive([1, 2, 3, -4, 5]);
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

# 23. Introduction to Currying and Partial Application

## Description
<section id='description'>
The <code>arity</code> of a function is the number of arguments it requires. <code>Currying</code> a function means to convert a function of N <code>arity</code> into N functions of <code>arity</code> 1.
In other words, it restructures a function so it takes one argument, then returns another function that takes the next argument, and so on.
Here's an example:
<blockquote>//Un-curried function<br>function unCurried(x, y) {<br>&nbsp;&nbsp;return x + y;<br>}<br><br>//Curried function<br>function curried(x) {<br>&nbsp;&nbsp;return function(y) {<br>&nbsp;&nbsp;&nbsp;&nbsp;return x + y;<br>&nbsp;&nbsp;}<br>}
<br>//Alternative using ES6
<br>const curried = x => y => x + y
<br>
<br>curried(1)(2) // Returns 3</blockquote>
This is useful in your program if you can't supply all the arguments to a function at one time. You can save each function call into a variable, which will hold the returned function reference that takes the next argument when it's available. Here's an example using the <code>curried</code> function in the example above:
<blockquote>// Call a curried function in parts:<br>var funcForY = curried(1);<br>console.log(funcForY(2)); // Prints 3</blockquote>
Similarly, <code>partial application</code> can be described as applying a few arguments to a function at a time and returning another function that is applied to more arguments.
Here's an example:
<blockquote>//Impartial function<br>function impartial(x, y, z) {<br>&nbsp;&nbsp;return x + y + z;<br>}<br>var partialFn = impartial.bind(this, 1, 2);<br>partialFn(10); // Returns 13</blockquote>
</section>

## Instructions
<section id='instructions'>
Fill in the body of the <code>add</code> function so it uses currying to add parameters <code>x</code>, <code>y</code>, and <code>z</code>.
</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function add(x) {
  // Add your code below this line


  // Add your code above this line
}
add(10)(20)(30);
```

</div>



</section>

## Solution
<section id='solution'>

```js
const add = x => y => z => x + y + z
```
</section>
<hr>

# Intermediate Algorithm Scripting
# 1. Sum All Numbers in a Range

## Description
<section id='description'>
We'll pass you an array of two numbers. Return the sum of those two numbers plus the sum of all the numbers between them.
The lowest number will not always come first.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function sumAll(arr) {
  return 1;
}

sumAll([1, 4]);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function sumAll(arr) {
  var sum = 0;
  arr.sort(function(a,b) {return a-b;});
  for (var i = arr[0]; i <= arr[1]; i++) {
    sum += i;
  }
  return sum;
}
```

</section>
<hr>

# 2. Diff Two Arrays

## Description
<section id='description'>
Compare two arrays and return a new array with any items only found in one of the two given arrays, but not both. In other words, return the symmetric difference of the two arrays.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
<strong>Note</strong><br>You can return the array with its elements in any order.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function diffArray(arr1, arr2) {
  var newArr = [];
  // Same, same; but different.
  return newArr;
}

diffArray([1, 2, 3, 5], [1, 2, 3, 4, 5]);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function diffArray(arr1, arr2) {
  var newArr = [];
  var h1 = Object.create(null);
  arr1.forEach(function(e) {
    h1[e] = e;
  });

  var h2 = Object.create(null);
  arr2.forEach(function(e) {
    h2[e] = e;
  });

  Object.keys(h1).forEach(function(e) {
     if (!(e in h2)) newArr.push(h1[e]);
  });
  Object.keys(h2).forEach(function(e) {
     if (!(e in h1)) newArr.push(h2[e]);
  });
  // Same, same; but different.
  return newArr;
}
```

</section>
<hr>

# 3. Seek and Destroy

## Description
<section id='description'>
You will be provided with an initial array (the first argument in the destroyer function), followed by one or more arguments. Remove all elements from the initial array that are of the same value as these arguments.
<strong>Note</strong><br> You have to use the <code>arguments</code> object.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function destroyer(arr) {
  // Remove all the values
  return arr;
}

destroyer([1, 2, 3, 1, 2, 3], 2, 3);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function destroyer(arr) {
  var hash = Object.create(null);
  [].slice.call(arguments, 1).forEach(function(e) {
    hash[e] = true;
  });
  // Remove all the values
  return arr.filter(function(e) { return !(e in hash);});
}

destroyer([1, 2, 3, 1, 2, 3], 2, 3);

```

</section>
<hr>

# 4. Wherefore art thou

## Description
<section id='description'>
Make a function that looks through an array of objects (first argument) and returns an array of all objects that have matching name and value pairs (second argument). Each name and value pair of the source object has to be present in the object from the collection if it is to be included in the returned array.
For example, if the first argument is <code>[{ first: "Romeo", last: "Montague" }, { first: "Mercutio", last: null }, { first: "Tybalt", last: "Capulet" }]</code>, and the second argument is <code>{ last: "Capulet" }</code>, then you must return the third object from the array (the first argument), because it contains the name and its value, that was passed on as the second argument.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function whatIsInAName(collection, source) {
  // What's in a name?
  var arr = [];
  // Only change code below this line


  // Only change code above this line
  return arr;
}

whatIsInAName([{ first: "Romeo", last: "Montague" }, { first: "Mercutio", last: null }, { first: "Tybalt", last: "Capulet" }], { last: "Capulet" });
```

</div>



</section>

## Solution
<section id='solution'>


```js
function whatIsInAName(collection, source) {
  var arr = [];
  var keys = Object.keys(source);
  collection.forEach(function(e) {
    if(keys.every(function(key) {return e[key] === source[key];})) {
      arr.push(e);
    }
  });
  return arr;
}
```

</section>
<hr>

# 5. Spinal Tap Case

## Description
<section id='description'>
Convert a string to spinal case. Spinal case is all-lowercase-words-joined-by-dashes.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function spinalCase(str) {
  // "It's such a fine line between stupid, and clever."
  // --David St. Hubbins
  return str;
}

spinalCase('This Is Spinal Tap');
```

</div>



</section>

## Solution
<section id='solution'>


```js
function spinalCase(str) {
  // "It's such a fine line between stupid, and clever."
  // --David St. Hubbins
  str = str.replace(/([a-z](?=[A-Z]))/g, '$1 ');
  return str.toLowerCase().replace(/\ |\_/g, '-');
}
```

</section>
<hr>

# 6. Pig Latin

## Description
<section id='description'>
Translate the provided string to pig latin.
<a href="http://en.wikipedia.org/wiki/Pig_Latin" target="_blank">Pig Latin</a> takes the first consonant (or consonant cluster) of an English word, moves it to the end of the word and suffixes an "ay".
If a word begins with a vowel you just add "way" to the end.
If a word does not contain a vowel, just add "ay" to the end.
Input strings are guaranteed to be English words in all lowercase.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function translatePigLatin(str) {
  return str;
}

translatePigLatin("consonant");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function translatePigLatin(str) {
  if (isVowel(str.charAt(0))) return str + "way";
  var front = [];
  str = str.split('');
  while (str.length && !isVowel(str[0])) {
    front.push(str.shift());
  }
  return [].concat(str, front).join('') + 'ay';
}

function isVowel(c) {
  return ['a', 'e', 'i', 'o', 'u'].indexOf(c.toLowerCase()) !== -1;
}
```

</section>
<hr>

# 7. Search and Replace

## Description
<section id='description'>
Perform a search and replace on the sentence using the arguments provided and return the new sentence.
First argument is the sentence to perform the search and replace on.
Second argument is the word that you will be replacing (before).
Third argument is what you will be replacing the second argument with (after).
<strong>Note</strong><br> Preserve the case of the first character in the original word when you are replacing it. For example if you mean to replace the word "Book" with the word "dog", it should be replaced as "Dog"
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function myReplace(str, before, after) {
  return str;
}

myReplace("A quick brown fox jumped over the lazy dog", "jumped", "leaped");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function myReplace(str, before, after) {
  if (before.charAt(0) === before.charAt(0).toUpperCase()) {
    after = after.charAt(0).toUpperCase() + after.substring(1);
  } else {
    after = after.charAt(0).toLowerCase() + after.substring(1);
  }
  return str.replace(before, after);
}
```

</section>
<hr>

# 8. DNA Pairing

## Description
<section id='description'>
The DNA strand is missing the pairing element. Take each character, get its pair, and return the results as a 2d array.
<a href="http://en.wikipedia.org/wiki/Base_pair" target="_blank">Base pairs</a> are a pair of AT and CG. Match the missing element to the provided character.
Return the provided character as the first element in each array.
For example, for the input GCG, return [["G", "C"], ["C","G"],["G", "C"]]
The character and its pair are paired up in an array, and all the arrays are grouped into one encapsulating array.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function pairElement(str) {
  return str;
}

pairElement("GCG");
```

</div>



</section>

## Solution
<section id='solution'>


```js
var lookup = Object.create(null);
lookup.A = 'T';
lookup.T = 'A';
lookup.C = 'G';
lookup.G = 'C';

function pairElement(str) {
 return str.split('').map(function(p) {return [p, lookup[p]];});
}
```

</section>
<hr>

# 9. Missing letters

## Description
<section id='description'>
Find the missing letter in the passed letter range and return it.
If all letters are present in the range, return undefined.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function fearNotLetter(str) {
  return str;
}

fearNotLetter("abce");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function fearNotLetter (str) {
  for (var i = str.charCodeAt(0); i <= str.charCodeAt(str.length - 1); i++) {
    var letter = String.fromCharCode(i);
    if (str.indexOf(letter) === -1) {
      return letter;
    }
  }

  return undefined;
}
```

</section>
<hr>

# 10. Sorted Union

## Description
<section id='description'>
Write a function that takes two or more arrays and returns a new array of unique values in the order of the original provided arrays.
In other words, all values present from all arrays should be included in their original order, but with no duplicates in the final array.
The unique numbers should be sorted by their original order, but the final array should not be sorted in numerical order.
Check the assertion tests for examples.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function uniteUnique(arr) {
  return arr;
}

uniteUnique([1, 3, 2], [5, 2, 1, 4], [2, 1]);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function uniteUnique(arr) {
  return [].slice.call(arguments).reduce(function(a, b) {
    return [].concat(a, b.filter(function(e) {return a.indexOf(e) === -1;}));
  }, []);
}
```

</section>
<hr>

# 11. Convert HTML Entities

## Description
<section id='description'>
Convert the characters <code>&</code>, <code><</code>, <code>></code>, <code>"</code> (double quote), and <code>'</code> (apostrophe), in a string to their corresponding HTML entities.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function convertHTML(str) {
  // &colon;&rpar;
  return str;
}

convertHTML("Dolce & Gabbana");
```

</div>



</section>

## Solution
<section id='solution'>


```js
var MAP = { '&': '&amp;',
            '<': '&lt;',
            '>': '&gt;',
            '"': '&quot;',
            "'": '&apos;'};

function convertHTML(str) {
  return str.replace(/[&<>"']/g, function(c) {
    return MAP[c];
  });
}
```

</section>
<hr>

# 12. Sum All Odd Fibonacci Numbers

## Description
<section id='description'>
Given a positive integer <code>num</code>, return the sum of all odd Fibonacci numbers that are less than or equal to <code>num</code>.
The first two numbers in the Fibonacci sequence are 1 and 1. Every additional number in the sequence is the sum of the two previous numbers. The first six numbers of the Fibonacci sequence are 1, 1, 2, 3, 5 and 8.
For example, <code>sumFibs(10)</code> should return <code>10</code> because all odd Fibonacci numbers less than or equal to <code>10</code> are 1, 1, 3, and 5.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function sumFibs(num) {
  return num;
}

sumFibs(4);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function sumFibs(num) {
  var a = 1;
  var b = 1;
  var s = 0;
  while (a <= num) {
    if (a % 2 !== 0) {
      s += a;
    }
    a = [b, b=b+a][0];
  }
  return s;
}
```

</section>
<hr>

# 13. Sum All Primes

## Description
<section id='description'>
Sum all the prime numbers up to and including the provided number.
A prime number is defined as a number greater than one and having only two divisors, one and itself. For example, 2 is a prime number because it's only divisible by one and two.
The provided number may not be a prime.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function sumPrimes(num) {
  return num;
}

sumPrimes(10);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function eratosthenesArray(n) {
    var primes = [];
    if (n > 2) {
        var half = n>>1;
        var sieve = Array(half);
        for (var i = 1, limit = Math.sqrt(n)>>1; i <= limit; i++) {
            if (!sieve[i]) {
                for (var step = 2*i+1, j = (step*step)>>1; j < half; j+=step) {
                    sieve[j] = true;
                }
            }
        }
        primes.push(2);
        for (var p = 1; p < half; p++) {
            if (!sieve[p]) primes.push(2*p+1);
        }
    }
    return primes;
}

function sumPrimes(num) {
  return eratosthenesArray(num+1).reduce(function(a,b) {return a+b;}, 0);
}

sumPrimes(10);
```

</section>
<hr>

# 14. Smallest Common Multiple

## Description
<section id='description'>
Find the smallest common multiple of the provided parameters that can be evenly divided by both, as well as by all sequential numbers in the range between these parameters.
The range will be an array of two numbers that will not necessarily be in numerical order.
For example, if given 1 and 3, find the smallest common multiple of both 1 and 3 that is also evenly divisible by all numbers <em>between</em> 1 and 3. The answer here would be 6.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function smallestCommons(arr) {
  return arr;
}


smallestCommons([1,5]);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function gcd(a, b) {
    while (b !== 0) {
        a = [b, b = a % b][0];
    }
    return a;
}

function lcm(a, b) {
    return (a *b) / gcd(a, b);
}

function smallestCommons(arr) {
  arr.sort(function(a,b) {return a-b;});
  var rng = [];
  for (var i = arr[0]; i <= arr[1]; i++) {
    rng.push(i);
  }
  return rng.reduce(lcm);
}
```

</section>
<hr>

# 15. Drop it

## Description
<section id='description'>
Given the array <code>arr</code>, iterate through and remove each element starting from the first element (the 0 index) until the function <code>func</code> returns <code>true</code> when the iterated element is passed through it.
Then return the rest of the array once the condition is satisfied, otherwise, <code>arr</code> should be returned as an empty array.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function dropElements(arr, func) {
  // Drop them elements.
  return arr;
}

dropElements([1, 2, 3], function(n) {return n < 3; });
```

</div>



</section>

## Solution
<section id='solution'>


```js
function dropElements(arr, func) {
  // Drop them elements.
  while (arr.length && !func(arr[0])) {
    arr.shift();
  }
  return arr;
}
```

</section>
<hr>

# 16. Steamroller

## Description
<section id='description'>
Flatten a nested array. You must account for varying levels of nesting.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function steamrollArray(arr) {
  // I'm a steamroller, baby
  return arr;
}

steamrollArray([1, [2], [3, [[4]]]]);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function steamrollArray(arr) {
  if (!Array.isArray(arr)) {
    return [arr];
  }
  var out = [];
  arr.forEach(function(e) {
    steamrollArray(e).forEach(function(v) {
      out.push(v);
    });
  });
  return out;
}
```

</section>
<hr>

# 17. Binary Agents

## Description
<section id='description'>
Return an English translated sentence of the passed binary string.
The binary string will be space separated.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function binaryAgent(str) {
  return str;
}

binaryAgent("01000001 01110010 01100101 01101110 00100111 01110100 00100000 01100010 01101111 01101110 01100110 01101001 01110010 01100101 01110011 00100000 01100110 01110101 01101110 00100001 00111111");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function binaryAgent(str) {
  return str.split(' ').map(function(s) { return parseInt(s, 2); }).map(function(b) { return String.fromCharCode(b);}).join('');
}
```

</section>
<hr>

# 18. Everything Be True

## Description
<section id='description'>
Check if the predicate (second argument) is <dfn>truthy</dfn> on all elements of a collection (first argument).
In other words, you are given an array collection of objects. The predicate <code>pre</code> will be an object property and you need to return <code>true</code> if its value is <code>truthy</code>. Otherwise, return <code>false</code>.
In JavaScript, <code>truthy</code> values are values that translate to <code>true</code> when evaluated in a Boolean context.
Remember, you can access object properties through either dot notation or <code>[]</code> notation.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function truthCheck(collection, pre) {
  // Is everyone being true?
  return pre;
}

truthCheck([{"user": "Tinky-Winky", "sex": "male"}, {"user": "Dipsy", "sex": "male"}, {"user": "Laa-Laa", "sex": "female"}, {"user": "Po", "sex": "female"}], "sex");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function truthCheck(collection, pre) {
  // Does everyone have one of these?
  return collection.every(function(e) { return e[pre]; });
}
```

</section>
<hr>

# 19. Arguments Optional

## Description
<section id='description'>
Create a function that sums two arguments together. If only one argument is provided, then return a function that expects one argument and returns the sum.
For example, <code>addTogether(2, 3)</code> should return <code>5</code>, and <code>addTogether(2)</code> should return a function.
Calling this returned function with a single argument will then return the sum:
<code>var sumTwoAnd = addTogether(2);</code>
<code>sumTwoAnd(3)</code> returns <code>5</code>.
If either argument isn't a valid number, return undefined.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function addTogether() {
  return false;
}

addTogether(2,3);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function addTogether() {
  var a = arguments[0];
  if (toString.call(a) !== '[object Number]') return;
  if (arguments.length === 1) {
    return function(b) {
      if (toString.call(b) !== '[object Number]') return;
      return a + b;
    };
  }
  var b = arguments[1];
  if (toString.call(b) !== '[object Number]') return;
  return a + arguments[1];
}
```

</section>
<hr>

# 20. Make a Person

## Description
<section id='description'>
Fill in the object constructor with the following methods below:
<blockquote>getFirstName()
getLastName()
getFullName()
setFirstName(first)
setLastName(last)
setFullName(firstAndLast)</blockquote>
Run the tests to see the expected output for each method.
The methods that take an argument must accept only one argument and it has to be a string.
These methods must be the only available means of interacting with the object.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
var Person = function(firstAndLast) {
  // Complete the method below and implement the others similarly
  this.getFullName = function() {
    return "";
  };
  return firstAndLast;
};

var bob = new Person('Bob Ross');
bob.getFullName();
```

</div>



</section>

## Solution
<section id='solution'>


```js
var Person = function(firstAndLast) {

  var firstName, lastName;

  function updateName(str) {
    firstName = str.split(" ")[0];
    lastName = str.split(" ")[1];
  }

  updateName(firstAndLast);

  this.getFirstName = function(){
    return firstName;
  };

  this.getLastName = function(){
    return lastName;
  };

  this.getFullName = function(){
    return firstName + " " + lastName;
  };

  this.setFirstName = function(str){
    firstName = str;
  };


  this.setLastName = function(str){
    lastName = str;
  };

  this.setFullName = function(str){
    updateName(str);
  };
};

var bob = new Person('Bob Ross');
bob.getFullName();
```

</section>
<hr>

# 21. Map the Debris

## Description
<section id='description'>
Return a new array that transforms the elements' average altitude into their orbital periods (in seconds).
The array will contain objects in the format <code>{name: 'name', avgAlt: avgAlt}</code>.
You can read about orbital periods <a href="http://en.wikipedia.org/wiki/Orbital_period" target='_blank'>on Wikipedia</a>.
The values should be rounded to the nearest whole number. The body being orbited is Earth.
The radius of the earth is 6367.4447 kilometers, and the GM value of earth is 398600.4418 km<sup>3</sup>s<sup>-2</sup>.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function orbitalPeriod(arr) {
  var GM = 398600.4418;
  var earthRadius = 6367.4447;
  return arr;
}

orbitalPeriod([{name : "sputnik", avgAlt : 35873.5553}]);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function orbitalPeriod(arr) {
  var GM = 398600.4418;
  var earthRadius = 6367.4447;
  var TAU = 2 *Math.PI;
  return arr.map(function(obj) {
    return {
      name: obj.name,
      orbitalPeriod: Math.round(TAU *Math.sqrt(Math.pow(obj.avgAlt+earthRadius, 3)/GM))
    };
  });
}

orbitalPeriod([{name : "sputkin", avgAlt : 35873.5553}]);

```

</section>
<hr>

# JavaScript Algorithms and Data Structures Projects
# 1. Palindrome Checker

## Description
<section id='description'>
Return <code>true</code> if the given string is a palindrome. Otherwise, return <code>false</code>.
A <dfn>palindrome</dfn> is a word or sentence that's spelled the same way both forward and backward, ignoring punctuation, case, and spacing.
<strong>Note</strong><br>You'll need to remove <strong>all non-alphanumeric characters</strong> (punctuation, spaces and symbols) and turn everything into the same case (lower or upper case) in order to check for palindromes.
We'll pass strings with varying formats, such as <code>"racecar"</code>, <code>"RaceCar"</code>, and <code>"race CAR"</code> among others.
We'll also pass strings with special symbols, such as <code>"2A3*3a2"</code>, <code>"2A3  3a2"</code>, and <code>"2_A3*3#A2"</code>.
Remember to use <a href="http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514" target="_blank">Read-Search-Ask</a> if you get stuck. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function palindrome(str) {
  // Good luck!
  return true;
}



palindrome("eye");
```

</div>



</section>

## Solution
<section id='solution'>


```js
function palindrome(str) {
  var string = str.toLowerCase().split(/[^A-Za-z0-9]/gi).join('');
  var aux = string.split('');
  if (aux.join('') === aux.reverse().join('')){
    return true;
  }

  return false;
}
```

</section>
<hr>

# 2. Roman Numeral Converter

## Description
<section id='description'>
Convert the given number into a roman numeral.
All <a href="http://www.mathsisfun.com/roman-numerals.html" target="_blank">roman numerals</a> answers should be provided in upper-case.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function convertToRoman(num) {
 return num;
}

convertToRoman(36);
```

</div>



</section>

## Solution
<section id='solution'>


```js
function convertToRoman(num) {
  var ref = [['M', 1000], ['CM', 900], ['D', 500], ['CD', 400], ['C', 100], ['XC', 90], ['L', 50], ['XL', 40], ['X', 10], ['IX', 9], ['V', 5], ['IV', 4], ['I', 1]];
  var res = [];
  ref.forEach(function(p) {
    while (num >= p[1]) {
      res.push(p[0]);
      num -= p[1];
    }
  });
  return res.join('');
}
```

</section>
<hr>

# 3. Caesars Cipher

## Description
<section id='description'>
One of the simplest and most widely known <dfn>ciphers</dfn> is a <code>Caesar cipher</code>, also known as a <code>shift cipher</code>. In a <code>shift cipher</code> the meanings of the letters are shifted by some set amount.
A common modern use is the <a href="https://en.wikipedia.org/wiki/ROT13" target='_blank'>ROT13</a> cipher, where the values of the letters are shifted by 13 places. Thus 'A' &harr; 'N', 'B' &harr;  'O' and so on.
Write a function which takes a <a href="https://en.wikipedia.org/wiki/ROT13" target='_blank'>ROT13</a> encoded string as input and returns a decoded string.
All letters will be uppercase. Do not transform any non-alphabetic character (i.e. spaces, punctuation), but do pass them on.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function rot13(str) { // LBH QVQ VG!

  return str;
}

// Change the inputs below to test
rot13("SERR PBQR PNZC");
```

</div>



</section>

## Solution
<section id='solution'>


```js
var lookup = {
  'A': 'N','B': 'O','C': 'P','D': 'Q',
  'E': 'R','F': 'S','G': 'T','H': 'U',
  'I': 'V','J': 'W','K': 'X','L': 'Y',
  'M': 'Z','N': 'A','O': 'B','P': 'C',
  'Q': 'D','R': 'E','S': 'F','T': 'G',
  'U': 'H','V': 'I','W': 'J','X': 'K',
  'Y': 'L','Z': 'M'
};

function rot13(encodedStr) {
  var codeArr = encodedStr.split("");  // String to Array
  var decodedArr = []; // Your Result goes here
  // Only change code below this line

  decodedArr = codeArr.map(function(letter) {
    if(lookup.hasOwnProperty(letter)) {
      letter = lookup[letter];
    }
    return letter;
  });

  // Only change code above this line
  return decodedArr.join(""); // Array to String
}
```

</section>
<hr>

# 4. Telephone Number Validator

## Description
<section id='description'>
Return <code>true</code> if the passed string looks like a valid US phone number.
The user may fill out the form field any way they choose as long as it has the format of a valid US number. The following are examples of valid formats for US numbers (refer to the tests below for other variants):
<blockquote>555-555-5555<br>(555)555-5555<br>(555) 555-5555<br>555 555 5555<br>5555555555<br>1 555 555 5555</blockquote>
For this challenge you will be presented with a string such as <code>800-692-7753</code> or <code>8oo-six427676;laskdjf</code>. Your job is to validate or reject the US phone number based on any combination of the formats provided above. The area code is required. If the country code is provided, you must confirm that the country code is <code>1</code>. Return <code>true</code> if the string is a valid US phone number; otherwise return <code>false</code>.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function telephoneCheck(str) {
  // Good luck!
  return true;
}

telephoneCheck("555-555-5555");
```

</div>



</section>

## Solution
<section id='solution'>


```js
var re = /^([+]?1[\s]?)?((?:[(](?:[2-9]1[02-9]|[2-9][02-8][0-9])[)][\s]?)|(?:(?:[2-9]1[02-9]|[2-9][02-8][0-9])[\s.-]?)){1}([2-9]1[02-9]|[2-9][02-9]1|[2-9][02-9]{2}[\s.-]?){1}([0-9]{4}){1}$/;

function telephoneCheck(str) {
  return re.test(str);
}

telephoneCheck("555-555-5555");
```

</section>
<hr>

# 5. Cash Register

## Description
<section id='description'>
Design a cash register drawer function <code>checkCashRegister()</code> that accepts purchase price as the first argument (<code>price</code>), payment as the second argument (<code>cash</code>), and cash-in-drawer (<code>cid</code>) as the third argument.
<code>cid</code> is a 2D array listing available currency.
The <code>checkCashRegister()</code> function should always return an object with a <code>status</code> key and a <code>change</code> key.
Return <code>{status: "INSUFFICIENT_FUNDS", change: []}</code> if cash-in-drawer is less than the change due, or if you cannot return the exact change.
Return <code>{status: "CLOSED", change: [...]}</code> with cash-in-drawer as the value for the key <code>change</code> if it is equal to the change due.
Otherwise, return <code>{status: "OPEN", change: [...]}</code>, with the change due in coins and bills, sorted in highest to lowest order, as the value of the <code>change</code> key.
Remember to use <a href='http://forum.freecodecamp.org/t/how-to-get-help-when-you-are-stuck/19514' target='_blank'>Read-Search-Ask</a> if you get stuck. Try to pair program. Write your own code.
<table class='table table-striped'><tr><th>Currency Unit</th><th>Amount</th></tr><tr><td>Penny</td><td>$0.01 (PENNY)</td></tr><tr><td>Nickel</td><td>$0.05 (NICKEL)</td></tr><tr><td>Dime</td><td>$0.1 (DIME)</td></tr><tr><td>Quarter</td><td>$0.25 (QUARTER)</td></tr><tr><td>Dollar</td><td>$1 (DOLLAR)</td></tr><tr><td>Five Dollars</td><td>$5 (FIVE)</td></tr><tr><td>Ten Dollars</td><td>$10 (TEN)</td></tr><tr><td>Twenty Dollars</td><td>$20 (TWENTY)</td></tr><tr><td>One-hundred Dollars</td><td>$100 (ONE HUNDRED)</td></tr></table>
</section>

## Instructions
<section id='instructions'>

</section>



## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function checkCashRegister(price, cash, cid) {
  var change;
  // Here is your change, ma'am.
  return change;
}

// Example cash-in-drawer array:
// [["PENNY", 1.01],
// ["NICKEL", 2.05],
// ["DIME", 3.1],
// ["QUARTER", 4.25],
// ["ONE", 90],
// ["FIVE", 55],
// ["TEN", 20],
// ["TWENTY", 60],
// ["ONE HUNDRED", 100]]

checkCashRegister(19.5, 20, [["PENNY", 1.01], ["NICKEL", 2.05], ["DIME", 3.1], ["QUARTER", 4.25], ["ONE", 90], ["FIVE", 55], ["TEN", 20], ["TWENTY", 60], ["ONE HUNDRED", 100]]);
```

</div>



</section>

## Solution
<section id='solution'>


```js
var denom = [
	{ name: 'ONE HUNDRED', val: 100},
	{ name: 'TWENTY', val: 20},
	{ name: 'TEN', val: 10},
	{ name: 'FIVE', val: 5},
	{ name: 'ONE', val: 1},
	{ name: 'QUARTER', val: 0.25},
	{ name: 'DIME', val: 0.1},
	{ name: 'NICKEL', val: 0.05},
	{ name: 'PENNY', val: 0.01}
];

function checkCashRegister(price, cash, cid) {
 var output = {status: null, change: []};
 var change = cash - price;
 var register = cid.reduce(function(acc, curr) {
 acc.total += curr[1];
 acc[curr[0]] = curr[1];
 return acc;
 }, {total: 0});
 if(register.total === change) {
 output.status = 'CLOSED';
 output.change = cid;
 return output;
 }
 if(register.total < change) {
 output.status = 'INSUFFICIENT_FUNDS';
 return output;
 }
 var change_arr = denom.reduce(function(acc, curr) {
 var value = 0;
 while(register[curr.name] > 0 && change >= curr.val) {
 change -= curr.val;
 register[curr.name] -= curr.val;
 value += curr.val;
 change = Math.round(change *100) / 100;
 }
 if(value > 0) {
 acc.push([ curr.name, value ]);
 }
 return acc;
 }, []);
 if(change_arr.length < 1 || change > 0) {
 output.status = 'INSUFFICIENT_FUNDS';
 return output;
 }
 output.status = 'OPEN';
 output.change = change_arr;
 return output;
}
```

</section>
<hr>

