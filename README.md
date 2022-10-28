# _Css_
### _Css Documentation_ 

* Inline style
~~~css
<p style = "color: red;">
~~~

* Internal style
~~~css

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Internal Style</title>
    <style>
    P {
    color: blue;
    background-color: yellow;
    }
    </style>
  </head>
  <body>
    <p>
    The content of this tag will be displayed in blue with a yellow background!
    </p>
    <p>
    <strong>Also</strong> will be displayed in blue with a yellow background!
    </p>
  </body>
</html>

~~~

* External style
~~~css

<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>External Style</title>
    <!-- Inclusion of the CSS file -->
    <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <p>
    The content of this tag will be displayed in blue with a yellow background!
    </p>
    <p>
    <strong>Also</strong> will be displayed in blue with a yellow background!
    </p>
  </body>
</html>

And inside the styles.css file we put only the CSS content:
P {
color: blue;
background-color: yellow;
}
~~~

* Fonts property
~~~css
We can define fonts using
of the font-family property

The font-family property can receive its value with or without quotes depending on its composition
,for example, when a font has its name separated by a space.

h1 {
font-family: serif;
}
h2 {
font-family: sans-serif;
}
P {
font-family: monospace;
}
Note: Monospace fonts can be either serif or sans serif. Monospace just means that all letters 
are the same size.

body {
font-family: "Helvetica", "Lucida Grande", sans-serif;
}

We have other properties to manipulate the font, such as the font-style property, 
which defines the font style that can be: 
normal (normal vertical), italic (slanted) and oblique (slanted).
~~~

* Text Alignment
~~~css
In the following example we are going to change the text alignment with the text-align property.

P {
text-align: right;
}

The example dictates that all paragraphs on our page have the text aligned to the right.

You can also configure a number of text spacing with CSS:

P {
line height: 3px; /* size of the height of each row */
letter-spacing: 3px; /* size of space between each letter */
word-spacing: 5px; /* size of space between each word */
text-indent: 30px; /* size of the margin of the first line of text
*/
}
~~~

* Background image
~~~css
The background-image property allows specifying an image file to be displayed 
in the background of the element. For example:

h1 {
background-image: url(over-background.jpg);
}

But we can also pass a web address to grab images remotely:

body {
background-image: url(https://i.imgur.com/uAhjMNd.jpg);
}
~~~

* Borders

~~~css

The CSS properties for defining the borders of an element present us with a series of options. 
We can, for each edge of an element, determine its color, its display style and its
width. For example:

body {
border-color: red;
border-style: solid;
border-width: 1px;
}

The border property has an abbreviated way to write the same styles we added above, but in a simpler way:

body {
border: 1px solid red;
}

We can also speak on which side of our element we want the border using the subproperty that indicates side:

h1 {
border-top: 1px solid red; /* red border on top */
border-right: 1px solid red; /* red border on the right */
border-bottom: 1px solid red; /* red border at the bottom */
border-left: 1px solid red; /* red border on the left */
}

~~~

* Colors in CSS
~~~css
Properties such as background-color , color , border-color , among others accept a color as a value.
There are several ways to define colors when using CSS.

The first, simplest, is using the color name:
h1 {
color: red;
}
h2 {
background-color: yellow;
}

In CSS, we can write colors based on their RGB composition:

h3 {
color: rgb(255, 200, 0);
}

The most common is hexadecimal notation.
This syntax is universally supported across browsers and is shorter to write, despite being more cryptic.

h3 {
background-color: #f2eded;
}
~~~

* Dimensions
~~~css
You can determine the dimensions of an element, for example:

P {
background-color: red;
height: 300px;
width: 300px;
}
~~~

* Padding
~~~css

The padding property is used to define an internal spacing on elements 
(by internal spacing we mean the distance between the element's boundary, 
its edge, and its respective content) and has the sub-properties listed below:

-> padding-top
-> padding-right
-> padding-bottom
-> padding-left

If four values are passed, they will be applied respectively to padding-top ,
padding-right , padding-bottom and padding-left .
To facilitate the memorization of this order, it is enough to remember that the
values are applied clockwise
P {
       padding: 10px 20px 15px 5px;
}

~~~

* Margin
~~~css

The margin property is very similar to the padding property, 
except that it adds space after the element boundary, 
i.e., it is a spacing beyond the element itself (outer spacing).

-> margin-top
-> margin-right
-> margin-bottom
-> margin-left

There is also a way to allow the browser to define the dimension of the padding or margin 
property according to the available space on the screen: 
we set the value auto to the spacings we want

P {
margin: 0 auto;
}

~~~

* Lists

~~~css

HTML lists

-> Unordered list

<ul>
<li>First item on the list</li>
<li>
Second item on the list:
<ul>
<li>First item of nested list</li>
<li>Second item in nested list</li>
</ul>
</li>
<li>Third item on the list</li>
</ul>

-> Ordered list

<ol>
<li>First item on the list</li>
<li>Second list item</li>
<li>Third item on the list</li>
<li>Fourth item on the list</li>
<li>Fifth item on the list</li>
</ol>

~~~

* Definition lists

~~~css

This list is the definition list.
<dl>
<dt>HTML</dt>
<dd>
HTML is the text markup language used to display text as pages on the Internet.
</dd>
<dt>Browser</dt>
<dd>
Browser is software that requests an HTML document
over the HTTP protocol and displays its content in a
window.
</dd>
</dl

~~~

* Stylized Lists

~~~css

To style the default format of ordered and unordered lists, we can use the list-style-type property in CSS:

ul {
/* change to circle before each <li> in the unordered list */
list style type: circle;
}
ol {
/* switches to an alphabetical sequence before each <li> in the sorted list */
list style type: upper alpha;
}
~~~
