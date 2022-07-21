# Forms and JS Events

## HTML Forms

### Your first Web Form. How To Structure A Web Form.

**Why are forms so important in web development?**
Forms are versatilke and can create complex structures on the web. 

**When designing a form, what are some key things to keep in mind when it comes to user experience?**

- NEVER nest a form inside of another form. It causes them to behave unpredictably.
- Use the \<form> element to define a form. Nest all of the form's contents inside this opening and closing tag.

**List 5 form elements and explain their importance.**

- \<form> formally defines a form. Nest all of the form's contents inside this opening and closing tag.
- \<fieldset> creates groups of widgets that share the same purpose, for styling and semantic purposes.
- \<legend> by including a \<legend> element just below the opening \<fieldset> tag. The text content of the \<legend> formally describes the purpose of the \<fieldset> it is included inside.
- \<label> element is the formal way to define a label for an HTML form widget. This is the most important element if you want to build accessible forms. Screenreaders will speak a form element's label along with any related instructions. One can click or tap the label to activate the corresponding widget. This is useful for controls like text inputs, where you can click the label as well as the input to focus it, but it is especially useful for radio buttons and checkboxes
- \<button> is used to submit data from the form.

## Learn JS

### Introduction To Events.

**How would you describe events to a non-technical friend?**
An event is an instance when something in the program has done something for qwhich the user should be alerted so they can choose to interact further wioth the program. This can be as simple as the user placing their cursor over a button, and the button changing color to indicate that their cursor is on top of the button.

**When using the addEventListener() method, what 2 arguments will you need to provide?**
Objects that can fire events have an addEventListener() method, that takes at least two arguments: 

1. The name of the event.
2. A function to handle the event.

**Describe the event object. Why is the target within the event object useful?**
The event object is automatically passed to event handlers to provide extra features and information. This is useful because it is communicating information about the part of the system that was acted upon. I imagine that keyboard shortcuts use this to register an event object when a certain combination of keys is pressed simultaneously within a program, by reporting that those keys have all been activated. 

**What is the difference between event bubbling and event capturing?**
In the capturing phase:

- The browser checks to see if the element's outer-most ancestor (<html>) has a click event handler registered on it for the capturing phase, and runs it if so.
- Then it moves on to the next element inside <html> and does the same thing, then the next one, and so on until it reaches the direct parent of the element that was actually clicked.


In the bubbling phase, the exact opposite of the capturing phase occurs:

- The browser checks to see if the direct parent of the clicked element has a click event handler registered on it for the bubbling phase, and runs it if so.
- Then it moves on to the next immediate ancestor element and does the same thing, then the next one, and so on until it reaches the <html> element.