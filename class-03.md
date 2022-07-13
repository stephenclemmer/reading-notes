# Read 3: HTML Lists, Control Flow with JS, and the CSS Box Model

## Learn HTML

### Ordered and Unordered lists

**When to use an unordered list in an HTML document**
An unordered list should be used when the order is ***not*** meaningful.

**When to use an ordered list in an HTML document**
An ordered list should be used when the order is meaningful.

**Ways to change the bullet style of unordered list items**
Attributes can be used to change the style of bullets in an unordered list.

1. List items in an \<ul> with no attributes will display as bulleted.
2. Using the ***type*** attribute, one can change an unordered list's bullets to be circles, discs, or squares. i.e.,

- \<ul type="circle">  This is the default and displays the typical arabic numerals.
- \<ul type="disc">  List ordered with lowercase letters
- \<ul type="square">List ordered with uppercase letters

**Ways to change the numbers on list items provided by an ordered list**
Attributes can be used to change the style of numbers in an ordered list.

1. List items in an \<ol> with no attributes will display as arabic numberals, i.e., 1, 2, 3...
2. Using the ***type*** attribute, one can change an ordered list in many ways. i.e.,

- \<ol type="1">  This is the default and displays the typical arabic numerals.
- \<ol type="a">  List ordered with lowercase letters
- \<ol type="A">  List ordered with uppercase letters
- \<ol type="I">  List ordered with lowercase Roman numerals
- \<ol type="i">  List ordered with uppercase Roman numerals

3. The ***reversed*** attribute specifies that the list's items are in reverse order. Items will be numbered from high to low.

4. The ***start*** attribute designates an integer, or numeral, from which the list will begin counting. i.e., start=4 will begin the list on 4, d, iv, or IV, depending on the list typer indicated.

## Learn CSS

### The Box Model

**Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?**
Margin and Padding were in love, They lived on different sides of the Border, but were unable to cross it. Padding searched within herself to find Content and realized that since neither she nor her love could cross the Border, the only way they could come together would be to eliminate the border completely.

**List and describe the four parts of an HTML elements box as referred to by the box model.**

1. Content: The area where your content is displayed;
Size it using properties like inline-size and block-size or width and height.

2. Padding: Sits around the content as white space;

3. Border: Wraps the content and any padding;

4. Margin: The outermost layer, it wraps the content, padding, and border as whitespace between this box and other elements


## Learn JavaScript

### Arrays, Operators and Expressions, Conditionals, Loops

What data types can be stored inside of an Array?

Is the people array a valid JavaScript array? If so, how can one access the values stored? If not, why?

``` text
 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
```

**List five shorthand operators for assignment in javascript and describe what they do.**

**Read the code below and evaluate the last expression and explain what the result would be and why.**

``` text
 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;
```

**Describe a real world example of when a conditional statement should be used in a JavaScript program.**
