# Object-Oriented Programming, HTML Tables

## Domain Modeling

**Explain why we need domain modeling.**

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

## HTML Table Basics

**Why should tables not be used for page layouts?**

1. Layout tables reduce accessibility for visually impaired users because they are difficult for screen readers to read.
2. Tables involve more complex markup structures than proper layout techniques which makes code harder to write, maintain, and debug.
3. Tables are not automatically reaponsive because they are sized according to their content by default, so extra measures are needed to get table layout styling to effectively work across a variety of devices.

**List and describe 3 different semantic HTML elements used in an HTML \<table>.**

- \<table> : Encloses the contenet of a table.
- \<td> ; Table Data, creates a single cell in a table
- \<tr> : Table Row, acts as a parent element to \<td> elements


## Introducing Constructors

**What is a constructor and what are some advantages to using it?**
A constructor is a means to create multiple similar objects with the same properties and methods.

**How does the term this differ when used in an object literal versus when used in a constructor?**
In JavaScript, the keyword called ‘this’ is the object that “owns” the code. The value of this, when used in an object, is the object itself. From within a constructor, you can also use the this keyword to call another constructor in the same class.

## Object Prototypes Using A Constructor

**Explain prototypes and inheritance via an analogy from your previous work experience.**

NOTE: This is a very common front end developer interview question
