# Read 2: Basics of HTML, CSS & JavaScript

## Introduction to HTML

### HTML Text Fundamentals

**Why is it important to use semantic elements in our HTML?**
HTML seeks to give a page structure and meaning with paragraphs, headings, lists, emphasis, and quotations. Semantic elements are used to more clearly demonstrate the intent of the programmer to others reading the code. For instance:

Paragraphs: \<p>
Headings: \<h1> - \<h6>
Lists: \<ul>, \<ol>, \<li>
Emphasis: \<em>
Quotations: \<q>
Strong: \<stromg>
Bold: \<b>
Italic: \<i>
Underline: \<u>

Other reasons that using semantic HTML is beneficial:

- Users can more easily scan the page for relevant content
- Search engines indexing the page consider the contents of headings to be relevant keywords, so choosing making sure that headings contain keywords will affect SEO.
- Semantic HTML allows screen readers and other accessibility features to be effective
- Elements that affect style in CSS or functionality with JavaScript need to wrap relevant content to ensure that they are effectively targted.

**How many levels of headings are there in HTML?**
There are six levels of headings in HTML H1 - H6

**Adding Hyperlinks to a Page**
A basic link is created by wrapping the text or other content inside an \<a> element and using the href attribute, also known as a Hypertext Reference, or target, that contains the web address.

> \<p>I'm creating a link to
> \<a href="https://www.mozilla.org/en-US/">the Mozilla homepage</a>.
> \</p>

### HTML Advanced Text Formatting

**What are some uses for the \<sup> and \<sub> elements?**
Superscript and subscript are used when marking up items like dates, chemical formulae, and mathematical equations so they have the correct meaning.

- \<sup> elements are denoted on the top half of the script's line.
- \<sub> elements are denoted on the bottom half of the script's line.

**When using the \<abbr> element, what attribute must be added to provide the full expansion of the term?**
The abbreviation element, \<abbr> , is used to wrap around an abbreviation or acronym, and provide a full expansion of the term (included inside a title attribute. For example:

> \<p>We use \<abbr title="Hypertext Markup Language">HTML</abbr> to structure our web documents.\</p>

## Learn CSS

### How CSS is Structured

**Three methods to apply CSS to HTML:**

1. External stylesheet: An external stylesheet contains CSS in a separate file with a .css extension. This is the most common and useful method of bringing CSS to a document. You can link a single CSS file to multiple web pages, styling all of them with the same CSS stylesheet. The external stylesheet would be linked to the .html file within the head, for example:

`<!DOCTYPE html>`
`<html>`
`  <head>`
`    <meta charset="utf-8">`
`    <title>My CSS experiment</title>`
`    <link rel="stylesheet" href="styles.css">`
`  </head>`
`  <body>`
`    <h1>Hello World!</h1>`
`    <p>This is my first CSS example</p>`
`  </body>`
`</html>`


2. Internal stylesheet: An internal stylesheet resides within an HTML document. To create an internal stylesheet, you place CSS inside a \<style> element contained inside the HTML \<head>.

`<!DOCTYPE html>`
`<html>`
`  <head>`
`    <meta charset="utf-8">`
`    <title>My CSS experiment</title>`
`    <style>`
`      h1 {`
`        color: blue;`
`        background-color: yellow;`
`        border: 1px solid black;`
`      }`
` `
`      p {`
`        color: red;`
`      }`
`    </style>`
`  </head>`
`  <body>`
`    <h1>Hello World!</h1>`
`    <p>This is my first CSS example</p>`
`  </body>`
`</html>`


3. Inline styles: Inline styles are CSS declarations that affect a single HTML element, contained within a style attribute. For instance:

`<!DOCTYPE html>`
`<html>`
`  <head>`
`    <meta charset="utf-8">`
`    <title>My CSS experiment</title>`
`  </head>`
`  <body>`
`    <h1 style="color: blue;background-color: yellow;border: 1px solid black;">Hello World!</h1>`
`    <p style="color:red;">This is my first CSS example</p>`
`  </body>`
`</html>`

**Why should we avoid using inline styles?**

**Review the block of code below and answer the following questions:**

**What is representing the selector?**

**Which components are the CSS declarations?**

**Which components are considered properties?**

## Learn JavaScript

### JavaScript Basics: Comments - Events

**What data type is a sequence of text enclosed in single quote marks?**

**List 4 types of JavaScript operators.**

**Describe a real world Problem you could solve with a Function.**

### Making Decisions in Your Code - Conditionals

An if statement checks a condition and if it evaluates to true, then the code block will execute. Otherwise it will not execute and will proceed to try and execute the next codeblock in the function.

An else-if statement tells the computer to execute the argument if the preceding command did not evaluate to true.

List 3 different types of comparison operators.
**Different types of comparison operators:**

**Difference between the logical operator && and ||?**
&& means that the computer should evaluate as true if ***both*** statements on either side of the && evaluate to true.

|| means that the computer should evaluate as true if ***either*** of the statements on either side of the && evaluate to true.
