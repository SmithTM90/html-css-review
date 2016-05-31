# HTML/CSS Review

This is a review of your working knowledge of HTML and CSS. Note that this review is designed to help you recall and familiarize yourself with technical concepts.

## Getting Started

* Fork and clone this repository
* Answer the following questions by...
  * Opening this file in Sublime
  * Answering the questions via Markdown. Feel free to refer to this [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Commit your changes
* Make a pull request for submission

---

## HTML

1.) Create a valid, empty HTML page with the necessary tags.

```html
<!DOCTYPE html>
<html>
<head>
  <title></title>
</head>
<body>

</body>
</html>
```

2.) What are the differences between these tags?

```html
<!-- Tag 1 -->
<img src="images/me.jpg" alt="My profile image">

<!-- Tag 2 -->
<div></div>
```

```
Explain here.
The <img src> tag, is making a reference to a specific image's location of exsistence, so that it can be displayed on the page.
The <div></div> tag is creating an html element that can have any number of other html elements inside of it. It has it's own default properties, like most html elements. 
```

---

## CSS

1.) Compare and contrast the following ways to add CSS to HTML elements.

```html
<!-- Inline CSS -->
<div style="background-color: red;"></div>

<!-- Internal style sheet -->
<style type="text/css">
  div {
    background-color: red;
  }
</style>

<!-- External style sheet (not shown) -->
<link rel="stylesheet" type="text/css" href="css/style.css">
```

```
Explain here
Inline CSS is CSS that is applied from within the html file to the specific element, "on the fly", and less desireable than other methods of applying CSS rules.

Internal stylesheet CSS is CSS that is "seperated" from the html but still "lives" in the html, the diference between internal and inline CSS is that you can set up CSS rules for multiple elements in the Internal style sheet, because the html will refer back to it for all the elements that the internal style sheet is applying CSS rules to.

External style sheets are the best practice way to applying CSS rules to your html elements, you make a reference to the style sheet from within the html, which is it's own file. The CSS file that you are using outside of the html will be far easier to read and easier to work with when applying your CSS rules to your elements.
```

2.) Below are some different CSS selectors. Use CSS comments to describe what each selector will do.

```css
/* comment like this */
div {
  border-radius: 50%;
}
/*This would apply a rounded appearance to the div element's border*/

.header p {
  font-size: 18px;
}
/*This would select all paragraph elements with the class of "header" and give them a font size of 18px*/

.footer {
  position: absolute;
  bottom: 0;
}
/*This would select all elements with the footer class, and set their position to be absolute or "exact", and the bottom: 0 would give them the exact parameter that would make the position: absolute have a reference for where it should be*/

.splash-image {
  background-image: url("../images/ocean.jpg");
  background-size: cover;
  width: 100%;
}
/*This would select all elements with the splash-image class, and apply a background image to them, the "cover" property tells the image to "stretch to fit" the entire element that the image is applied to, and the width being set to 100%, tells the element to always have a width that is equal to 100% the width of it's parent element*/

.ninja:hover {
  display: none;
  color: black;
}
/*This would select all elements with the ninja class, and apply the functionality to them of detecting when a mouse cursor is hovering over the top of them, and based on that condition being met, would give them a display of none, which makes that specific element "dissapear", and at the same time apply a color of black to elements that accept that CSS rule */
```

