Day 06 — Introduction to CSS
Topics-
1.	Introduction to CSS
2.	CSS Selectors
3.	CSS Colors
4.	CSS Units
5.	CSS Typography
1. What is CSS?
CSS stands for Cascading Style Sheets. It is used to control how HTML elements look on a webpage.
HTML gives a webpage its structure and content, while CSS makes that structure look better by adding colors, changing text styles, adjusting font sizes, and controlling the overall appearance.
For example, HTML can create a heading and a paragraph, but CSS can change their colors, font sizes, and alignment.
Example
>HTML:
<h1>Welcome to My Website</h1>
<p>I am learning web development.</p>
>CSS:
h1 {
    color: blue;
    font-size: 32px;
}

p {
    color: gray;
    font-size: 18px;
}
In this example, CSS changes the heading to blue and makes its text larger. It also changes the paragraph color and font size.
Three Ways to Add CSS
There are three common ways to apply CSS to HTML.
1. Inline CSS
Inline CSS is written directly inside an HTML element using the style attribute.
<h1 style="color: blue;">Welcome to My Website</h1>
2. Internal CSS
Internal CSS is written inside a <style> element in the HTML document, usually within the <head> section.
<head>
    <style>
        h1 {
            color: blue;
            font-size: 32px;
        }
    </style>
</head>
3. External CSS
External CSS is written in a separate .css file and connected to the HTML document using the <link> element.
<link rel="stylesheet" href="style.css">
The CSS rules are then written inside style.css.
>Remember: External CSS is generally the preferred approach for larger projects because it keeps HTML and CSS separate and makes the code easier to maintain.
2. CSS Selectors
CSS selectors are used to target specific HTML elements so that we can apply styles to them.
In simple words, selectors tell the browser which elements should receive a particular style.
Common Types of CSS Selectors
1. Universal Selector (*)
The universal selector targets all HTML elements on a webpage.
* {
    font-family: Arial, sans-serif;
}
2. Element Selector
An element selector targets all elements with a particular HTML tag name.
h1 {
    color: blue;
}

p {
    font-size: 18px;
}
3. Class Selector (.)
A class selector targets HTML elements that have a specific class name. A class can be used on multiple elements.
<p class="highlight">This is an important message.</p>.highlight {
    color: green;
}
4. ID Selector (#)
An ID selector targets an element with a specific ID. An ID should be unique within a webpage.
<h1 id="main-heading">My Personal Website</h1>#main-heading {
    color: darkblue;
}
5. Grouping Selector
A grouping selector allows us to apply the same styles to multiple selectors without writing the same CSS rules separately.
h1, h2, p {
    font-family: Arial, sans-serif;
}
6. Descendant Selector
A descendant selector targets elements that are located inside another specified element.
nav a {
    color: white;
}
Here, the style applies to anchor (a) elements inside a nav element.
>Quick Comparison
Selector	Symbol or Format	Purpose
Universal	*	Targets all elements.
Element	p	Targets all elements with a particular tag.
Class	.name	Targets elements with a specific class.
ID	#name	Targets an element with a specific ID.
Grouping	h1, p	Applies the same styles to multiple selectors.
Descendant	nav a	Targets elements inside another element.
Remember: Class selectors use a dot (.), while ID selectors use a hash (#).
3. CSS Colors
CSS colors are used to change the appearance of text, backgrounds, borders, and other elements.
We can apply colors using different formats depending on what we need.
>Common Ways to Write Colors in CSS
1. Color Names
We can use predefined color names directly.
h1 {
    color: red;
}
2. HEX Color
HEX colors use hexadecimal values to represent colors. They begin with a hash (#).
h1 {
    color: #2563eb;
}
3. RGB Color
RGB stands for Red, Green, and Blue. Each value normally ranges from 0 to 255.
h1 {
    color: rgb(37, 99, 235);
}
4. RGBA Color
RGBA works like RGB but includes an additional alpha value to control transparency.
The alpha value ranges from 0 (fully transparent) to 1 (fully opaque).
p {
    color: rgba(0, 0, 0, 0.7);
}
>Common CSS Color Properties
body {
    background-color: #f4f4f4;
}

h1 {
    color: #2563eb;
}
·	color changes the text color.
·	background-color changes the background color.
>Remember: Choosing suitable colors helps make a webpage easier to read and more visually appealing.
4. CSS Units
CSS units are used to define measurements such as font sizes, widths, and other dimensions.
Different units are useful in different situations.
Common CSS Units
1. Pixels (px)
Pixels are fixed units commonly used for defining specific sizes.
h1 {
    font-size: 32px;
}
2. Root EM (rem)
rem is relative to the font size of the root HTML element.
For example, when the root font size is 16px, 2rem equals 32px.
h1 {
    font-size: 2rem;
}
3. EM (em)
em is relative to the font size of the element's parent (for properties such as font-size).
.parent {
    font-size: 20px;
}

.parent p {
    font-size: 1.5em;
}
Here, the paragraph's font size becomes 30px.
4. Percentage (%)
Percentage is a relative unit. Its actual size depends on the relevant property and the element's containing block or parent.
.profile {
    width: 80%;
}
Here, the width is 80% of the containing block's width.
5. Viewport Width (vw)
vw represents a percentage of the browser's viewport width.
h1 {
    font-size: 5vw;
}
6. Viewport Height (vh)
vh represents a percentage of the browser's viewport height.
.hero {
    height: 50vh;
}
>Quick Comparison
Unit	Meaning	Example
px	Pixels	font-size: 16px;
rem	Relative to the root font size	font-size: 2rem;
em	Relative to the parent font size for font sizing	font-size: 1.5em;
%	Percentage of a relevant reference size	width: 80%;
vw	Viewport width	width: 50vw;
vh	Viewport height	height: 50vh;
>Remember: px is useful when you need a specific size, while relative units such as rem, em, and % can help create more flexible layouts.
5. CSS Typography
Typography refers to how text is displayed on a webpage. It includes the font family, size, weight, alignment, and spacing of text.
Good typography makes website content easier to read and gives the webpage a more polished appearance.
Important Typography Properties
1. font-family
It defines which font should be used for the text.
body {
    font-family: Arial, sans-serif;
}
2. font-size
It controls the size of the text.
h1 {
    font-size: 32px;
}
3. font-weight
It controls how bold or light the text appears.
h1 {
    font-weight: bold;
}
Common values include normal, bold, and numeric values such as 400 and 700.
4. text-align
It controls the horizontal alignment of text.
h1 {
    text-align: center;
}
Common values include left, right, center, and justify.
5. text-decoration
It adds or removes decorative lines from text.
a {
    text-decoration: none;
}
6. line-height
It controls the vertical space between lines of text.
p {
    line-height: 1.6;
}
7. letter-spacing
It controls the space between individual letters.
h1 {
    letter-spacing: 2px;
}
8. text-transform
It changes the capitalization of text without changing the original HTML content.
h2 {
    text-transform: uppercase;
}
>Example Combining Typography Properties
h1 {
    font-family: Arial, sans-serif;
    font-size: 32px;
    font-weight: bold;
    text-align: center;
    letter-spacing: 1px;
}

p {
    font-size: 16px;
    line-height: 1.6;
}
>Remember: Good typography is not just about choosing a stylish font. Text should also be comfortable to read.
