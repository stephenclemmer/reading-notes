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


##### Questions for class

**How would you describe an object to a non-technical friend you grew up with?**
An object is a collection of *related* data  and/or functionality , usually consisting of several variables (a.k.a. properties) and functions (a.k.a. methods). An analogy to help one understand this concept is a car. A car is an object because it's made up of related parts that make it go. Its fuel is a property, i.e., 85, 87, or 93 octane. Its engine is a method that takes whatever fuel it is given and processes it to perfrom a task (i.e., firing a piston). The engine too is an object, made up of constituent parts (properties and methods) that work together to allow it to function. The fuel is also an object, made up of properties that will allow it to store energy and combust upon reaching a certain temperature. In this way, objects are made up of other objects, who may be made up of other objects, etc.  At the most basic level, defining a variable and setting it up to receive a program is creating the simplest object possible, i.e.,

```text
const variableName = {}
```

**What are some advantages to creating object literals?**
*Using an object literal when you want to transfer a series of structured, related data items in some manner, for example sending a request to the server to be put into a database. Sending a single object is much more efficient than sending several items individually, and it is easier to work with than an array, when you want to identify individual items by name.*

**How do objects differ from arrays?**

**Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.**

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

## Introduction To The DOM

**What is the DOM?**

**Briefly describe the relationship between the DOM and JavaScript.**

**Understanding the problem domain is the hardest part of programming**

**What’s the difference between primitive values and object references in JavaScript?**
