# Read 1: Introductory HTML and JavaScript

HTML, CSS, and JavaScript are the basis of modern webpages. Understanding their structure and interactivity are essential to being able to program.

Sources for the notes that follow include pages from 'https://developer.mozilla.org/'


## Things I Want to Know More About

1. What are practical uses for (!) the Bang Operator?

## How the Web Works

### **How HTTP sends data between computers:**

  **The client requests service. The server responds with service.**

  ***The client asks for a menu. The server responds with a menu.***

  The client orders a meal. The server puts in the order.

  *The kitchen makes the order. The client picks up the meal.*

### **How HTML, CSS, and JS files are “parsed” in the browser:**

**The browser parses the HTML file first, and that leads to the browser to recognize:**

1. any \<link>-element references to external CSS stylesheets
2. any \<script>-element references to scripts.

**As the browser parses the HTML:**

1. It sends requests back to the server for any CSS files it has found from \<link> elements,
2. Then sends requests back to the server for any JavaScript files it has found from \<script> elements,
3. Then uses the CSS files and JavaScript files to parse the CSS and JavaScript.

**The browser then:**

1. Generates an in-memory DOM tree from the parsed HTML,
2. Generates an in-memory CSSOM structure from the parsed CSS,
3. Compiles and executes the parsed JavaScript.

**As the browser builds the DOM tree and applies the styles from the CSSOM tree and executes the JavaScript:**

1. A visual representation of the page is painted to the screen,
2. The user sees the page content and can begin to interact with it.

## Website Design and Process

Planning
- What is your website about?
- What information are you presenting on the subject?
- What does your website look like?
  - Sketch out your design
  - Choose your assets
  - Text
  - Theme Color
  - Images
  - Font

**How to find images to add to a Website:**
1. Go to Google Images and search for something suitable.
2. Click on the image to get an enlarged view of it.
3. Right-click the image (Ctrl + click on a Mac), choose Save Image As..., and choose a safe place to save your image, or alternatively, copy the image's web address from your browser's address bar for later use.

## JavaScript Basics

***JavaScript is used for adding interactive behavior to web pages. JavaScript allows users to interact with web pages:***

- Show or hide more information with the click of a button
- Change the color of a button when the mouse hovers over it
- Slide through a carousel of images on the homepage
- Zooming in or zooming out on an image
- Displaying a timer or count-down on a website
- Playing audio and video in a web page
- Displaying animations

**How to Add JavaScript to a Page:**

1. Create a new folder named scripts. Within the scripts folder, create a new text document called main.js, and save it.
2. In your index.html file, enter this code on a new line, just before the closing \</body> tag:

> \<script src="scripts/main.js"></script>`

This is doing the same job as the \<link> element for CSS. It applies the JavaScript to the page, so it can have an effect on the HTML (along with the CSS, and anything else on the page).

3. Add this code to the main.js file:

> const myHeading = document.querySelector('h1');
> myHeading.textContent = 'Hello world!';

4. Make sure the HTML and JavaScript files are saved. Then load index.html in your browser.

**How to denote a String vs a Number in JavaScript?**
To signify that the value is a string, enclose it in single quote marks. Numbers are written without quotes around them. 

**String:**
> let myVariable = 'Bob';

**Number:**
> let myVariable = 10;

### Important Concepts

**Variables and Why They are Important in JavaScript**

- **Variables** are containers that store values. You start by declaring a variable with the let keyword, followed by the name you give to the variable:

> let myVariable;

A semicolon at the end of a line indicates where a statement ends. It is only required when you need to separate statements on a single line. However, some people believe it's good practice to have semicolons at the end of each statement.

Variables are necessary to do anything interesting in programming. If values couldn't change, then one couldn't do anything dynamic, like personalize a greeting message or change an image displayed in an image gallery.

- **Operators** are mathematical symbols that produces a result based on two values (or variables). 

- **Conditionals** are code structures used to test if an expression returns true or not. A very common form of conditionals is the if ... else statement.

- **Functions** are a way of packaging functionality that you wish to reuse.

- **Events**: Real interactivity on a website requires event handlers. These are code structures that listen for activity in the browser, and run code in response.



### Getting Started with HTML: HTML Document Structure and Metadata in HTML:

- **Anatomy of an HTML Document**: 

><!DOCTYPE html>
>\<html>
>  <head>
>    <meta charset="utf-8">
>    <title>My test page</title>
>  </head>
>  <body>
>    <p>This is my page</p>
>  </body>
></html>

- **Additional Elements within a Typical Website**:
  - header: \<header>.
  - navigation bar: \<nav>.
  - main content: \<main>, with various content subsections represented by \<article>, \<section>, and \<div> elements.
  - sidebar: \<aside>; often placed inside \<main>.
  - footer: \<footer>.
  - anchor tags: \<a>

- **Anatomy of an HTML Element**:
An eleent contains an opening tag and a closing tag. Content to be displayed is written in between these tags. 

- **HTML Attribute**: Attributes contain extra information about the element that won't appear in the content. An attribute should have:

  - A space between it and the element name. (For an element with more than one attribute, the attributes should be separated by spaces too.)
  - The attribute name, followed by an equal sign.
  - An attribute value, wrapped with opening and closing quote marks.

- **Difference between \<article> and \<Section> element tags**:

**\<article>**: The \<article> HTML element represents a self-contained composition in a document, page, application, or site, ***which is intended to be independently distributable or reusable*** (e.g., in syndication). Examples include: a forum post, a magazine or newspaper article, or a blog entry, a product card, a user-submitted comment, an interactive widget or gadget, or any other independent item of content.

**\<section>**: The \<section> HTML element represents a ***generic*** standalone section of a document, which doesn't have a more specific semantic element to represent it. Sections should always have a heading, with very few exceptions.

**Metadata's Influence on SEO**
Although metadata is not displayed to the user, it helps to define how relevant information is, which will afect where it shows up on the results page.

**The \<meta> tag's Purpose:
The \<meta> tag defines metadata about an HTML document. Metadata is data (information) about data. \<meta> tags always go inside the \<head> element, and are typically used to specify character set, page description, keywords, author of the document, and viewport settings.

### How to Start to Design a Website

Websites are tools. The first step to designing a website is to define what one wishes to accomplish with it. The most important question to answer is: "What exactly is this site trying to accomplish?"

### Semantics
Using an \<h1> element to define a top-level heading rather than using a \<span> element is an example of employing a semantic element over an element that is not semantic.

The \<h1> element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page", whereas the \<span> element is not semantic and does not lend any meaning to understanding the content.



## Ryan's Linux Tutorial

### Important Concepts

- Everything is a file under Linux, even directories.
- Linux is an extensionless system. Files can have any extension they like or none at all.
- Linux is case sensitive. Beware of silly typos.
- No undo. The Linux command line does not have an undo feature. Perform destructive actions carefully.
- Command line options: Most commands have many useful command line options. Make sure you skim the man page for new commands so you are familiar with what they can do and what is available.

### The Command Line

ex:

Prompt: Command: Command-line arguments

- There must be a space between the command and the first command line argument
- The first command line argument is also referred to as an option. Options are typically used to modify the behaviour of the command. Options are usually listed before other arguments and typically start with a dash ( - ).

***Shortcut***: Use the up and down arrow keys to scroll through previously entered commands
***Shortcut***: Run cd by otself to be taken back to the home directory
***Shortcut***: **Tab Completion**: Hit the Tab key on your keyboard at any time which will invoke an auto complete action. If nothing happens then that means there are several possibilities. If you hit Tab again it will show you those possibilities. You may then continue typing and hit Tab again and it will again try to auto complete for you.
***Shortcut***: ~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /Users/Stephen then you could refer to the directory Documents with the path /Users/Stephen/Documents or ~/Documents

### Commands

**pwd**: (print working directory) Tells you what your current or present working directory is.
**ls**: (list) Lists the contents of the current directory. i.e., ls \[options][location]
-- **-l**: (long listing, i.e., ls -l)
-- **/etc***: (i.e., ls /etc) Tells ls not to list our current directory but instead to list that directory's contents.
**ls -a**: will list all files, including those that are hidden.
**cd**: (change directory ex, cd \[location]) Change Directories - ie. move to another directory.
**/etc**: - Stores config files for the system.
**/var/log**: - Stores log files for various system programs. 
**/bin**: - The location of several commonly used programs.
**/usr/bin**: - Another location for programs on the system.
**file \[path]**: To obtain information about what type of file a file or directory is.
**man \<command to look up>**: Accesses the manual for a particular command.

### Paths

Whenever we refer to either a file or directory on the command line, we are in fact referring to a path. ie. A path is a means to get to a particular file or directory on the system.

**Absolute Paths**: Absolute paths specify a location (file or directory) in relation to the root directory. You can identify them easily as they always begin with a forward slash ( / )

**Relative Paths**: Relative paths specify a location (file or directory) in relation to where we currently are in the system. They will not begin with a slash.

#### Path Navigation

~ (tilde) - This is a shortcut for your home directory. eg, if your home directory is /Users/Stephen then you could refer to the directory Documents with the path /Users/Stephen/Documents or ~/Documents
. (dot) - This is a reference to your current directory. eg in the example above we referred to Documents on line 4 with a relative path. It could also be written as ./Documents (Normally this extra bit is not required but in later sections we will see where it comes in handy).
.. (dotdot)- This is a reference to the parent directory. You can use this several times in a path to keep going up the hierarchy. eg if you were in the path /Users/Stephen you could run the command ls ../../ and this would do a listing of the root directory.

#### Spaces in Names

- Use quotes or an escape character before spaces ( \ ) to denote that a file name with spaces in the title is a single command line argument.
- Use Tab Completion to automatically escape spaces in a title.

#### Hidden Files

- Use a period ( . ) at the beginning of a file name to make it hidden.
- ls -a will list all files, including those that are hidden.

### Manual Pages

The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept. You invoke the manual pages with the following command:

**man [command to look up]**

To exit the manual pages, pres 'q' for quit.

Keyword search on Manual pages:

**man -k [search term]**

If you want to search within a manual page while you are in the particular manual page,  search press forward slash '/' followed by the term you would like to search for and hit 'enter' If the term appears multiple times you may cycle through them by pressing the 'n' button for next.

### File Manipulation

**mkdir**: command used to make a new directory. i.e., mkdir \[options]\<Directory>
**mk dir -p**: Tells mkdir to make parent directories as needed, i.e., mkdir -p directory/subdirectory1/subdirectory2
**mk dir -v**: The v stands for verbose. The terminal will display in detail what was done.
**rmdir**: Removes a directory. i.e., rmdir \[options]\<Directory>. Technically a directory needs to be empty before it can be removed, however there is a way around this that I will learn later. -p and -v are both available on rmdir.

#### Creating a Blank File

**touch**: Creates a blank file i.e., touch \[options]\<filename>
What is being taken advantage of is that if we touch a file and it does not exist, the command will do us a favor and automatically creating it for us. Touch is actually a command one may use to modify the access and modification times on a file (normally not needed but sometimes when you're testing a system that relies on file access or modification times it can be useful).

#### Copying a File or Directory

**cp**: Copies a file or directory, i.e., cp \[options]\<source>\<destination>

#### Moving a File or Directory

**mv**: Moves a file or directory, i.e., mv \[options]\<source>\<destination>

#### Renaming Files and Directories

Renaming can be done using mv. Were one to specify the *destination* to be the *same directory as the source, but with a different name*, then one may effectively use mv to rename a file or directory.

#### Removing a File (and Non-Empty Directories)

**rm**: Removes a file, i.e., rm \[options]\<file>
**rm -r**: Removes directories and all files contained within them.
*A good option to use in combination with r is i which stands for interactive. This option will prompt you before removing each file and directory and give you the option to cancel the command.*
