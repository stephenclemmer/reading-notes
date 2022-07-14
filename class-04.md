# HTML Links, JS Functions, and Intro to CSS Layout

## Learn HTML

### Creating Hyperlinks

**To create a basic link, we wrap text or other content inside what element?**
The anchor element: \<a></a>

**The href attribute contains what information?**
The href contains the web address.

**What are some ways we can ensure links on our pages are accessible to all readers?**

- Create descriptive text links
- include keywords in your link text to effectively describe what is being linked to
- Don't repeat the URL as part of the link text
- Don't say "link" or "links to" in the link text
- Keep link text as short as possible
- Minimize instances where multiple copies of the same text are linked to different places.

## CSS Layout

### CSS Layout: Normal Flow CSS Layout: Positioning

**What is meant by “normal flow”?**
Elements on a webpage lay out in normal flow if you haven't applied any CSS to change the way they behave.

**What are a few differences between block-level and inline elements?**
#### Block-level Elements
By default, a block level element's content fills the available inline space of the parent element containing it and grows along the block dimension to accommodate its content.

By default, block-level elements are laid out in the block flow direction, which is based on the parent's writing mode (initial: horizontal-tb). Each element will appear on a new line below the last one, with each one separated by whatever margin that's been specified. 

#### Inline Elements
The size of Inline elements is just the size of their content. You can't set width or height on inline elements — they just sit inside the content of block level elements. If you want to control the size of an inline element in this manner, you need to set it to behave like a block level element

Inline elements don't appear on new lines; instead, they all sit on the same line along with any adjacent (or wrapped) text content as long as there is space for them to do so inside the width of the parent block level element. If there isn't space, then the overflowing content will move down to a new line.

**Static positioning is the default for every html element.**

**Name a few advantages to using absolute positioning on an element.**
Good cross-browser support.
Less dependence on floats.
Less dependence on margins.

**What is a key difference between fixed positioning and absolute positioning?**
The position and dimensions of an element with absolute positioning: are relative to its containing block
The position and dimensions of an element with fixed positioning are always relative to the initial containing block. This is normally the viewport: the browser window or the paper's page box.

## Learn JavaScript

### Functions – Reusable Blocks of Code

**Describe the difference between a function declaration and a function invocation.**
Function Declarations: A function declaration has the following parts: returnType functionName( parameter list ); A function declaration tells the compiler about a function name and how to call the function.

Invoking a Function: The code inside a function is executed when the function is invoked. It is common to use the term "call a function" instead of "invoke a function".

**What is the difference between a parameter and an argument?**
Parameters and Arguments are the same. They need to be specified when you are invoking a function. They are need to be included inside the function's parentheses.

**Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.**

Pair programming allows one to expand their knowledge by learning from their peers. It also allows one to practicve their vocabulary by choosing the correct terms to communicate an idea. 