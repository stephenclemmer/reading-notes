# Problem Domain, Objects, and the DOM

## JavaScript Object Basics

An object is a collection of *related* data and/or functionality. These usually consist of several variables and functions (which are called properties and methods when they are inside objects)

**properties**: data items within an object.
**methods** functions that exist within an opbject to do something with the properties.

creating an object often begins with defining and initializing a variable.

``` text
const objectName = {}
```

Properties and Methods are then added within the curly braces of the object, by naming members and then giving each member a value.

The syntax for an object ALWAYS follows this pattern:

``` text
const objectName = {
  member1Name: member1Value,
  member2Name: member2Value,
  member3Name: member3Value
};
```

*When the object's members are functions there's a simpler syntax. Instead of* bio: function() *one can just write* bio() *instead.*

#### Purpose

An **object literal** is an object whose contents have been literally written out as it has been created. It is very common to create an object using an object literal when you want to transfer a series of structured, related data items in some manner, for example sending a request to the server to be put into a database. Sending a single object is much more efficient than sending several items individually, and it is easier to work with than an array, when you want to identify individual items by name.

#### How to access things inside of objects

**Dot Notation**
Use **Dot Notation** to access the properties and methods inside of objects.

```text
objectName.property
objectName.methodName()
objectName.memberName
objectName.memberName\[arrayElement] (when the memberValue is an array)
```

**Bracket Notation**

``` text
objectName\['property']
objectName\['methodName()']
objectName\['memberName']\[membervalue]
objectName\['memberName\[arrayElement]'] (when the memberValue is an array)
```

Bracket notation is why objects are sometimes called associative arrays — they map strings to values in the same way that arrays map numbers to values.

Dot notation is generally preferred over bracket notation because it is more succint and easier to read. However there are some cases where you have to use brackets. For example, if an object property name is defined at runtime (i.e., when the user will be defining the input through a prompt) then you can't use dot notation to access the value, but you can pass the name as a variable inside brackets as shown with input below:

``` text
const person = {
  name: ['Bob', 'Smith'],
  age: 32
}
const input = prompt('Get name or age?')
console.log(person[input])
```

One useful aspect of bracket notation is that it can be used to set not only member values dynamically, but member names too. Adding a property to an object using the method above isn't possible with dot notation, which can only accept a literal member name, not a variable value pointing to a name.

#### Setting Object Members
One can use Dot Notation or Bracket Notation to declare a new value for an Object Member. i.e.,

```text
objectName.memberName = newMemberNameValue
objectName[memberName][memberValue] = newMemberValue
```

Additionally, this can also be used to create completely new Members. For example:

```text
person['eyes'] = 'hazel';
person.farewell = function() {
  console.log('Bye everybody!');
}
```

#### this

The word "this" is a means to refers to the keyword the current object the code is being written inside; particularly useful when using **Constructors** to create more than one object from a single object definition.

#### Constructors

A constructor is just a function called by using the "new" keyword. 

**syntax**
Constructors, by convention, start with a capital letter and are named for the type of object they create.

When you call a constructor, it will:

- Create a new object
- Bind "this" to the new object, so you can refer to "this" in your constructor code
- run the code in the constructor
- return the new object.

``` text
function Person(name) {
  this.name = name;
  this.introduceSelf = function() {
    console.log(`Hi! I'm ${this.name}.`);
  }
}
```

To call Person() as a constructor, we use the word "new":

``` text
const salva = new Person('Salva');
salva.name;
salva.introduceSelf();

const frankie = new Person('Frankie');
frankie.name;
frankie.introduceSelf();
```


##### Questions for class

**How would you describe an object to a non-technical friend you grew up with?**
An object is a collection of *related* data  and/or functionality , usually consisting of several variables (a.k.a. properties) and functions (a.k.a. methods). An analogy to help one understand this concept is a car. A car is an object because it's made up of related parts that make it go. Its fuel is a property, i.e., 85, 87, or 93 octane. Its engine is a method that takes whatever fuel it is given and processes it to perfrom a task (i.e., firing a piston). The engine too is an object, made up of constituent parts (properties and methods) that work together to allow it to function. The fuel is also an object, made up of properties that will allow it to store energy and combust upon reaching a certain temperature. In this way, objects are made up of other objects, who may be made up of other objects, etc.  At the most basic level, defining a variable and setting it up to receive a program is creating the simplest object possible, i.e.,

```text
const variableName = {}
```

**What are some advantages to creating object literals?**
*Using an object literal when you want to transfer a series of structured, related data items in some manner, for example sending a request to the server to be put into a database. Sending a single object is much more efficient than sending several items individually, and it is easier to work with than an array, when you want to identify individual items by name.*

**How do objects differ from arrays?**
Objects and arays are similar insofar as they each store a collection of information. 

An array simply stores a list of information to be accessed at a later time.

An object is a means to manipulate a store of information which can include vartiables and functions.

For instance, an avatar in a game would be an object. One could choose to dress the avatar in a red shirt with blue shoes and black pants. The arrays that sit within the avatar object may include:
let shirtOptions = \[red, blue, black, orange]
let pantsOptions = \[red, blue, black, orange]
let shoeOptions = \[red, blue, black, orange]

**Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.**
If an object property name is defined at runtime (i.e., when the user will be defining the input through a prompt) then you can't use dot notation to access the value, but you can pass the name as a variable inside brackets

**Evaluate the code below. What does the term this refer to and what is the advantage to using this?**

``` text
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```

The term "this" refers to the object name, dog. The term "this" is used to be able to run the same function within other objects that are named something other than 'dog'.

## Introduction To The DOM

**What is the DOM?**
The Document Object Model represents a webpage so that different programming languages can interact with it and affect its structure, style, and content. The DOM is a Web API, that allows different programs to interact with one another.

**Briefly describe the relationship between the DOM and JavaScript.**
The DOM is like an interpreter that allows two different programs to work toward a common purpose. For instance, the HTML builds the structure of a building, while the JavaScript installs the electrical system and plumbing system. The DOM is like the foreman that understands what the architect is trying to do and ensures that both the HTML and JavaScript's work takes the form or a working building, rather than a separate structure, and sewer/electrical system.

**Understanding the problem domain is the hardest part of programming**
THIS LINK IS BROKEN!

### Primitve Values and Object References
**What’s the difference between primitive values and object references in JavaScript?**
Primitive Values are any JavaScript data type, other than Objects. These include the following seven data types:

- Boolean
- Null
- Undefined
- Number
- BinInt
- String
- Symbol

Object references are the eighth Javascript data type, Objects. These include:

- Arrays
- Functions
- dates

**How Primitive Values and Object References are Stored Differently**
When a primitive value is assigned to a variable, the variable is set to that value directly. i.e., 

``` text
let stringOne = 'tiger'
```

When the variable is assigned with an object, however, things are different. Instead of containing the value directly, that variable contains a reference to it.

const moe = {
  name: 'Moe Szyslak',
  occupation: 'Bartender',
  voicedBy: 'Hank Azaria'
}

When this code is executed, the computer memopry will store it for later use. The variable "moe" doeasn;t contain the object directly. Instead it contains a reference to the memory address that currenrtly stores the object.

***Immutable Data vs. Mutable Data***
 Primitive values are immutable, meaning that they cannot be changed.
 Object references are mutable, meaning that they can be changed.

``` text
let word = 'snow'
word[0] = 'k'
console.log(word) // "snow" (The code above did not change the word)
```

 whereas...

``` text
let letters = ['s', 'n', 'o', 'w']
letters[0] = 'k'
console.log(letters) // (4) ["k", "n", "o", "w"]
```

### IMPORTANT: 

Aside: the code written above used the let keyword to create the letters variable, but you could define the variable with const and the result would still be the same. const prevents you from reassigning values, but it does not prevent you from mutating existing values.

**Primitive Values and Object References affect Variable Assignments**
Primitive Values such a s strings cannot be reassigned, but object references can. To keep from reassigningthem, use Object.assign to retain the target object while also having the ability to create source objects to be passed through that same object.

**Primitive Values and Object References affect Equality Comparisons**

Since primitives contain direct values, equality comparisons made with them perform in the way you probably expect:

``` text
'Moe Szyslak' === 'Moe Szyslak' // true
false === false // true
1970 === 1970 // true
undefined === undefined // true
```

Because the Object Reference is actually storing the memory address of the location where the object exists, in order to check whether the contents of two objects are the same you need to either:

Iterate through the object and check that each key and value match. This can be tricky because an object’s property can be an object in itself.
Convert the object to a suitable primitive before doing the equality check.

``` text
const moeA = { name: 'Moe Szyslak' }
const moeB = { name: 'Moe Szyslak' }
moeA === moeB // false
JSON.stringify(moeA) === JSON.stringify(moeB) // true
```

``` text
const dateA = new Date(0)
const dateB = new Date(0)
dateA === dateB // false
dateA.getTime() === dateB.getTime() // true
```

### IMPORTANT

Developing a strong grasp of primitive values, object references, and mutability is a critical step in progressing past the beginner stages of JavaScript programming.

This knowledge will help you identify bugs, understand key differences in programming paradigms, and help you understand your code at a deeper level.

