Day 02 – HTML Introduction and Document Structure

Challenge: DIU CPC – 99 Days of Coding
Phase: 01 – Web Fundamentals, HTML & CSS

1. Introduction to HTML

HTML stands for HyperText Markup Language. It is the standard markup language used to create and structure content on web pages.

HTML provides the basic structure of a website. It tells the browser how different pieces of content should be organized, such as headings, paragraphs, images, links, tables, and forms.

In simple terms, HTML provides the skeleton of a webpage.

HTML works together with other web technologies:

HTML: Defines the structure and content of a webpage.

CSS: Controls the appearance, design, colors, spacing, and layout.

JavaScript: Adds interactivity and dynamic behavior.

For example, when creating a personal portfolio website, HTML defines the sections and content, CSS makes the website visually attractive, and JavaScript can be used to add interactive features.
Is HTML a programming language?

HTML is not considered a programming language because it does not have programming logic such as conditions, loops, or functions. It is a markup language that describes the structure and meaning of webpage content.

2. What is HTML5?

HTML5 is the fifth major version of HTML and introduced modern features that make building websites easier and more powerful.

It supports modern web content, multimedia, improved forms, and semantic elements.

Some important HTML5 features include:

Support for audio and video.

Improved form input types.

Semantic elements such as header, nav, section, and footer.

Better support for modern web applications.

HTML5 is the foundation of modern HTML development.

3. Understanding HTML Tags
An HTML tag is a special keyword written inside angle brackets that tells the browser how to interpret a particular part of the document.

Most HTML elements use an opening tag and a closing tag.

Example:

<p>This is a paragraph.</p>

Here:

<p> is the opening tag.

This is a paragraph. is the content.

</p> is the closing tag.

The forward slash / indicates the closing tag.

Some HTML elements are void elements, meaning they do not require a separate closing tag.

Examples:

<br>
<hr>
<img>

4. Understanding HTML Elements

An HTML element generally consists of an opening tag, content, and a closing tag.

Example:

<h1>Welcome to My Website</h1>

In this example, the complete structure is called an HTML element.

The main parts are:

Opening tag: <h1>

Content: Welcome to My Website

Closing tag: </h1>

Difference Between Tags and Elements

A tag is the markup written inside angle brackets, while an element represents the complete HTML structure.

For example:

<p>Hello World!</p>
The <p> and </p> are tags, while the entire line is an HTML element.

5. Understanding HTML Attributes

HTML attributes provide additional information about HTML elements.

They are generally written inside the opening tag and usually consist of a name and a value.

Example:

<a href="https://www.google.com">Visit Google</a>

Here:

<a> is the anchor tag.

href is the attribute name.

https://www.google.com is the attribute value.

Visit Google is the visible link text.

Example:

<img src="profile.jpg" alt="My profile picture">

In this example, src identifies the image file, while alt provides alternative text describing the image.

6. Understanding HTML Document Structure

Every standard HTML document follows a basic structure. This structure helps the browser understand and process the webpage correctly.

Example:

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Website</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>This is my first HTML webpage.</p>
</body>

</html>

Explanation of Each Part

1. <!DOCTYPE html>

This declaration tells the browser that the document uses modern HTML (HTML5).

2. <html lang="en">
This is the root element of the HTML document. All other HTML elements are placed inside it. The lang attribute specifies that the primary language of the page is English.

3. <head>

The head section contains information about the webpage, such as its title, character encoding, metadata, and links to external resources. Most of this information is not directly displayed as webpage content.

4. <meta charset="UTF-8">

This specifies the character encoding used by the webpage. UTF-8 supports a wide range of characters and languages.

5. <meta name="viewport" content="width=device-width, initial-scale=1.0">

This helps the webpage display properly on different screen sizes, including mobile devices.

6. <title>

This defines the title of the webpage, which usually appears in the browser tab.

7. <body>

The body contains the actual content displayed on the webpage, such as text, headings, images, links, and other elements.
7. HTML Comments

HTML comments allow developers to write notes inside their code. These comments are not displayed on the webpage.

Example:

<!-- This is an HTML comment -->

<h1>My First Website</h1>

Comments are useful for explaining code and organizing larger HTML documents.
