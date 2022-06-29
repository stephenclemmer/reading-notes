DOM: Document Object Model: https://developer.mozilla.org/en-US/docs/Glossary/DOM

Input Output in plain JavaScript: https://code-maven.com/input-output-in-plain-javascript

Javascript Variables
Variables are containers for storing data (storing data values).
In this example, x, y, and z, are variables, declared with the var keyword:
var x = 5;
var y = 6;
var z = x + y;

4 Ways to Declare a JavaScript Variable:
Using var 
Using let (can be reassigned)
Using const (a constant variable that cannot be reassigned)
Using nothing

The Script element. The <script> HTML element is used to embed executable code or data; this is typically used to embed or refer to JavaScript code.

<!DOCTYPE html>
<html>
<body>

<h1>JavaScript Variables</h1>

<p>In this example, x, y, and z are variables.</p>

<p id="demo"></p>

<script>
var x = 5;
var y = 8;
var z = x + y;
document.getElementById("demo").innerHTML =
"The value of z is: " + z;
</script>

</body>
</html>

What is the difference between var, let and const?: https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/

Javascript introduces INTERACTIVITY to a website. 

BEST PRACTICE: It is a good programming practice to declare all variables at the beginning of a script.

A variable is a pointer to a type of data, i.e. String, Number/Integer, Boolean, (Array). A variable holds datas and can be changed just like in algebra.

PRO TIP: Because javascript reads from top to bottom, variables must be defined prior to the function. 

What does it mean to declare a variable? Make a variable AND/OR assign a value. 
Let x; ← declare variable… (consult class viseo before the 1:30:00 mark to see Kassie’s notes.)

Conditional Logic: If something is true, do this, otherwise do another thing.

When referencing variables, do not use quotation marks
When referencing strings, use quotation marks
prompt(“”) 
console.log();   - prints the contents in the parentheses to the console
= (assigns meaning to a variable)
== (equals)
=== (STRICTLY equals)
if {} (when true, do this)
else {} (when not true, do this other thing)
Else if {} (if this other thing is true, then do this instead.)
document.write(); (will write it on the HTML document)

Functions allow one to control where on a page the javascript shows up. 



To link java script file to HTML file, is with a <script> tag. I.e., 
<script scr=”nameoffile.js”></script>



API: An API (Application Programming Interface) is a set of features and rules that exist inside a software program (the application) enabling interaction with it through software - as opposed to a human user interface. The API can be seen as a simple contract (the interface) between the application offering it and other items, such as third party software or hardware.
In Web development, an API is generally a set of code features (e.g. methods, properties, events, and URLs) that a developer can use in their apps for interacting with components of a user's web browser, or other software/hardware on the user's computer, or third party websites and services.
For example:
The getUserMedia API can be used to grab audio and video from a user's webcam, which can then be used in any way the developer likes, for example, recording video and audio, broadcasting it to another user in a conference call, or capturing image stills from the video.
The Geolocation API can be used to retrieve location information from whatever service the user has available on their device (e.g. GPS), which can then be used in conjunction with the Google Maps APIs to for example plot the user's location on a custom map and show them what tourist attractions are in their area.
Differences between APIs and Interfaces: https://zellwk.com/blog/interface-vs-api/



There are many APIs available
Interfaces: There are a lot of different interfaces available


