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
