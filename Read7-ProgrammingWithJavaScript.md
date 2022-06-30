# Read 7: Programming with JavaScript

## Control flow

Control flow: the order in which the computer executes statements in a script. Code is run in order from the first line in the file to the last line, unless the computer runs across structures that change the control flow, such as conditionals and loops. A typical script in JavaScript or PHP (and the like) includes many control structures, including conditionals, loops and functions. Parts of a script may also be set to execute when events occur. Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution.

## Conditionals

A condition is a set of rules that can interrupt normal code execution or change it, depending on whether the condition is completed or not. An instruction or a set of instructions is executed if a specific condition is fulfilled. Otherwise, another instruction is executed. It is also possible to repeat the execution of an instruction, or set of instructions, while a condition is not yet fulfilled. In any programming language, the code needs to make decisions and carry out actions accordingly depending on different inputs. For example, in a game, if the player's number of lives is 0, then it's game over. In a weather app, if it is being looked at in the morning, show a sunrise graphic; show stars and a moon if it is nighttime. 

## Loops

For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:

if (field==empty) {
    promptUser();
} else {
    submitForm();
}

For example, the above excerpt might be inside a function that runs when the user clicks the Submit button for the form. The function could also include a loop, which iterates through all of the fields in the form, checking each one in turn. Looking back at the code in the if and else sections, the lines promptUser and submitForm could also be calls to other functions in the script. As you can see, control structures can dictate complex flows of processing even with only a few lines of code.

## Operators

JavaScript has both binary and unary operators, and one special ternary operator, the conditional operator. 

### Binary Operator

A binary operator requires two operands, one before the operator and one after the operator:

operand1 operator operand2

For example, 3+4 or x*y.

### Unary Operator

A unary operator requires a single operand, either before or after the operator:
operator operand or operand operator

## Assignment operators

An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = f() is an assignment expression that assigns the value of f() to x.

## Functions

Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.

### Defining a Function

A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

- The name of the function.
- A list of parameters to the function, enclosed in parentheses and separated by commas.
- The JavaScript statements that define the function, enclosed in curly brackets, {...}.

Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called. For example, the following code defines a simple function named square:

    function square(number) {
    return number * number;
    }

The function square takes one parameter, called number. The function consists of one statement that says to return the parameter of the function (that is, number) multiplied by itself. The statement return specifies the value returned by the function:

    return number * number;

Parameters are essentially passed to functions by value — so if the code within the body of a function assigns a completely new value to a parameter that was passed to the function, the change is not reflected globally or in the code which called that function.

## Calling a Function

Calling the function actually performs the specified actions with the indicated parameters.

## Array

The Array object, as with arrays in other programming languages, enables storing a collection of multiple items under a single variable name, and has members for performing common array operations.

- In JavaScript, arrays aren't primitives but are instead Array objects with the following core characteristics:
- JavaScript arrays are resizable and can contain a mix of different data types. (When those characteristics are undesirable, use typed arrays instead.)
- JavaScript arrays are not associative arrays and so, array elements cannot be accessed using arbitrary strings as indexes, but must be accessed using nonnegative integers (or their respective string form) as indexes.
- JavaScript arrays are zero-indexed: the first element of an array is at index 0, the second is at index 1, and so on — and the last element is at the value of the array's length property minus 1.
- JavaScript array-copy operations create shallow copies. (All standard built-in copy operations with any JavaScript objects create shallow copies, rather than deep copies).

## Kassie’s Demo:

### Defining the condition

If…else statements to write a message to the console/webpage
if…
else if…
else…

### Structure of a function

#### To declare a function:

1. Use the keyword “function” (there are other ways to do this too.)
2. Name the function followed by a set of parentheses without a space between the function name and parentheses, followed by a code block that is between curly braces. 
Parameters go in the parentheses
3. The code block goes in the curly braces (i.e. the code the function executes)

    Function nameOfFunction(){}

*The prior steps outlined are Declaring the function. To use the function, it must be called, which is done by using the function’s name.*

    nameOfFunction()

#### To return a message to the user

1. define the message by using let command to define the message
2. then ask to return that defined message value.

    let message;....

    return message; (should be within the function)

### Parameters 
- Exist in the function between its parentheses) 
- The parameters should be separated by commas.

### Arguments: 
When a function is invoked, the variables entered into the parentheses will be what the user chooses to run. 

    console.log();
    document .write();

*Use a <script></script> tag to call a function inside of your html.*
