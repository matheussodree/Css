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
Note: Monospace fonts can be either serif or sans serif. Monospace just means that all letters are the same size.

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
