Day 05 — Semantic HTML

Topics -
1.	Introduction to Semantic HTML
2.	Header
3.	Navigation (nav)
4.	Main
5.	Section
6.	Footer

   
1. What is Semantic HTML?
Semantic HTML means using HTML elements that clearly describe the purpose and meaning of their content.
Instead of using generic elements for everything, we can use meaningful elements to organize different parts of a webpage.
For example, a website usually has a header at the top, a navigation menu, a main content area, and a footer at the bottom.
Semantic HTML helps browsers, developers, and screen readers understand the structure of a webpage more easily.
Semantic HTML Example
<header>
    <h1>My Website</h1>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
</nav>

<main>
    <section>
        <h2>About Me</h2>
        <p>This is my personal website.</p>
    </section>
</main>

<footer>
    <p>Copyright 2026 My Website</p>
</footer>
2. Header Element
The <header> element represents the introductory part of a webpage or a section.
It commonly contains:
·	Website name or logo.
·	Main heading.
·	Short introduction.
·	Navigation menu.
A website can have a main header, and individual sections or articles can also have their own headers.
Example
<header>
    <h1>My Personal Website</h1>
    <p>Welcome to my website.</p>
</header>
Remember: The header usually introduces the website or the content that follows it.
3. Navigation Element (nav)
The <nav> element is used to create a navigation area containing important links.
It helps visitors move between different pages or sections of a website.
Common navigation links include:
·	Home
·	About
·	Services
·	Projects
·	Contact
Example
<nav>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>
Remember: The nav element should be used for important navigation links, not every single link on a webpage.
4. Main Element
The <main> element contains the primary content of a webpage.
It represents the main information that visitors come to see.
For example, on a personal portfolio website, the main content might include:
·	Personal introduction.
·	About section.
·	Technical skills.
·	Projects.
·	Contact information.
Example
<main>
    <section>
        <h2>About Me</h2>
        <p>I am learning web development.</p>
    </section>

    <section>
        <h2>My Skills</h2>
        <p>I am currently practicing HTML and CSS.</p>
    </section>
</main>
Remember
·	A webpage should normally have one visible main element.
·	The main element should contain the central content of the page.
·	Header, navigation, and footer elements are generally placed outside the main element when they belong to the overall page layout.
5. Section Element
The <section> element is used to divide a webpage into different meaningful parts.
Each section usually focuses on a particular topic and normally has its own heading.
For example, a portfolio website can have separate sections for About Me, Skills, Projects, and Contact.
Example
<section id="about">
    <h2>About Me</h2>
    <p>I am a university student interested in technology.</p>
</section>

<section id="skills">
    <h2>My Skills</h2>
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
    </ul>
</section>

<section id="projects">
    <h2>My Projects</h2>
    <p>Here are some projects I have worked on.</p>
</section>
Remember: Each section should represent a meaningful group of related content. It is not simply a replacement for every div.
6. Footer Element
The <footer> element represents the footer of a webpage or a section.
It usually contains information about the website, its owner, or related resources.
Common footer content includes:
·	Copyright information.
·	Contact information.
·	Social media links.
·	Privacy policy.
·	Terms and conditions.
·	Additional navigation links.
Example
<footer>
    <p>&copy; 2026 My Personal Semantic Website.</p>

    <p>All rights reserved by MD Nazmul Alam.</p>

    <a href="#home">Back to Top</a>
</footer>
Remember: A footer can belong to the entire webpage or to an individual section or article.
7. Difference Between Semantic and Non-Semantic HTML
HTML elements can be divided into two broad groups based on whether they communicate the meaning of their content.
Semantic Elements
Semantic elements clearly describe their purpose.
Examples:
·	<header>
·	<nav>
·	<main>
·	<section>
·	<footer>
·	<article>
·	<aside>
Non-Semantic Elements
Non-semantic elements do not describe the meaning of their content by themselves.
Examples:
·	<div>
·	<span>

8. Why Should We Use Semantic HTML?
Semantic HTML is important when building professional websites.
Some of its main benefits are:
1.	Better Readability: The code becomes easier to understand.
2.	Better Accessibility: Screen readers can identify important page landmarks.
3.	SEO Support: Search engines can better understand the structure and meaning of webpage content.
4.	Easy Maintenance: Developers can identify different parts of a webpage more easily.
5.	Better Structure: Related content can be organized into meaningful sections.
Learning Resources
·	MDN — Semantic HTML
·	MDN — HTML Elements Reference
·	W3Schools — HTML Semantic Elements
