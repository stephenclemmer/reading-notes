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
Margin and Padding were in love, They lived on different sides of the Border, but were unable to cross it. Padding searched within herself to find Content and realized that since neither she nor her love could cross the Border, the only way they could come together would be to eliminate the Border completely.

**List and describe the four parts of an HTML elements box as referred to by the box model.**

1. Content: The area where your content is displayed;
Size it using properties like inline-size and block-size or width and height.

2. Padding: Sits around the content as white space;

3. Border: Wraps the content and any padding;

4. Margin: The outermost layer, it wraps the content, padding, and border as whitespace between this box and other elements

## Learn JavaScript

### Arrays, Operators and Expressions, Conditionals, Loops

**Data types that can be stored inside of an Array?**

- Strings
- Numbers
- Objects
- Other arrays

**Is the people array a valid JavaScript array? If so, how can one access the values stored? If not, why?**

``` text
 const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
```

The people array is a valid JavaScript array. It is a multidimensional array because it is an array containing three arrays. Arrays and objects within arrays are numbered starting with zero. The values can be accessed by chaining numbers together to access items in the array's three different arrays. for instance:

- **people [0]** yields: **['pete', 32, 'librarian', null]**
- **people [1[** yields: **['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing']**
- **people [2]** yields: **['bill', null, 'artist', null]**
- **people [0][3]** yields: **null** (the first null in the series)
- **people [2][2]** yields: **artist**
- **people [2][1]** yields: **null** (the second-to-last null in the series)
- **people [2][3]** yields: **null** (the last null in the series)

**Shorthand operators for assignment in javascript and what they do.**

An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x.

Compound assignment operators that are shorthand for operations

``` text
x = f()    Assignment:......................x = f()
x += f()   Addition assignment:.............x = x + f()
x -= f()   Subtraction assignment:..........x = x - f()
x *= f()   Multiplication assignment:.......x = x * f()
x /= f()   Division assignment:.............x = x / f()
x %= f()   Remainder assignment:............x = x % f()
x **= f()  Exponentiation assignment:.......x = x ** f()
x <<= f()  Left shift assignment:...........x = x << f()
x >>= f()  Right shift assignment:..........x = x >> f()
x >>>= f() Unsigned right shift assignment: x = x >>> f()
x &= f()   Bitwise AND assignment:..........x = x & f()
x ^= f()   Bitwise XOR assignment:..........x = x ^ f()
x |= f()   Bitwise OR assignment:...........x = x | f()
x &&= f()  Logical AND assignment:..........x && (x = f())
x ||= f()  Logical OR assignment:...........x || (x = f())
x ??= f()  Logical nullish assignment:......x ?? (x = f())
```

**Read the code below and evaluate the last expression and explain what the result would be and why.**

``` text
 let a = 10;
 let b = 'dog';
 let c = false;

 // evaluate this
 (a + c) + b;
```

**The result would be: '10dog'**

false = 0 and true = 1

10 + 0 = 10
10 + 'dog' = '10dog'

This is best understood if one were to change the false value to true

false = 0 and true = 1

10 + 1 = 11
11 + 'dog' = '11dog'

**Describe a real world example of when a conditional statement should be used in a JavaScript program.**

Conditional statements create rules that result in consequences. In a JavaScript program, they may manifest as, "If a condition is met, then give an output." For instance if a person was asked to pick a number the computer may give one answer if the nbumber chosen were even, and another answer if the number chosen was odd.
