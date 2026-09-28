# JavaScript Variables and Data Types
If HTML is the skeleton of the human body and CSS is the skin, hair, and appearance, then JavaScript is like the body's central nervous system. JavaScript brings interactivity to websites by enabling complex functionality, such as handling user input, animating elements, and even building full web applications.


## Data Types in JavaScript
We can divide JavaScript data types into two main categories:

1. **Primitive Data Types**
2. **Non-Primitive (Reference) Data Types**

## Primitive Data Types

JavaScript has **7 primitive data types**:

- Number
- String
- Boolean
- Undefined
- Null
- Symbol
- BigInt

## Non-Primitive Data Types

**Objects** are non-primitive data types.

Objects include:

- Object
- Array
- Function

> **Note:** Arrays and functions are technically specialized types of objects in JavaScript.

- Number: A number represents both integers and floating-point values. Examples of integers include 7, 19, and 90.
- Floating point: A floating point number is a number with a decimal point. Examples include 3.14, 0.5, and 0.0001.
- String: A string is a sequence of characters, or text, enclosed in quotes. "I like coding" and 'JavaScript is fun' are examples of strings.
- Boolean: A boolean represents one of two possible values: true or false. You can use a boolean to represent a condition, such as isLoggedIn = true.
- Undefined and Null: An undefined value is a variable that has been declared but not assigned a value. A null value is an empty value, or a variable that has intentionally been assigned a value of null.
- Object: An object is a collection of key-value pairs. The key is the property name, and the value is the property value.
- BigInt: When the number is too large for the Number data type, you can use the BigInt data type to represent integers of arbitrary length.
- Symbol: The Symbol data type is a unique and immutable value that may be used as an identifier for object properties.
```JavaScript
const crypticKey1= Symbol("saltNpepper");
const crypticKey2= Symbol("saltNpepper");
console.log(crypticKey1 === crypticKey2); // false
```
## Variables in JavaScript
- Variables can be declared using the let keyword.
- To assign a value to a variable, you can use the assignment operator =.
- Variables declared using let can be reassigned a new value.
- After Asign a variabklle no need to reasign it
- Apart from let, you can also use const to declare a variable. However, a const variable cannot be reassigned a new value.
- Variables declared using const find uses in declaring constants, that are not allowed to change throughout the code, such as PI or MAX_SIZE.
### Variable Naming Conventions
- Variable names should be descriptive and meaningful.
- Variable names should be camelCase like cityName, isLoggedIn, and veryBigNumber.
- Variable names should not start with a number. They must begin with a letter, _, or $.
- Variable names should not contain spaces or special characters, except for _ and $.
- Variable names should not be reserved keywords.
- Variable names are case-sensitive. age and Age are different variables.
## Strings
- Strings are sequences of characters enclosed in quotes. They can be created using single quotes and double quotes.
- Concatenation is the process of joining multiple strings or combining strings with variables that hold text. The + operator is one of the simplest and most frequently used methods to concatenate strings.
- If you need to add or append to an existing string, then you can use the += operator. This is helpful when you want to build upon a string by adding more text to it over time.
- Another way you can concatenate strings is to use the concat() method. This method joins two or more strings together.

## Logging Messages with console.log()
The console.log() method is used to log messages to the console. It's a helpful tool for debugging and testing your code.
```JavaScript
console.log("Hello, World!");
// Output: Hello, World!
```
### Template Literal in JavaScript
Same like F-String in Python
```JS
let name = "Ayaz";
let message = `Hello ${name}`;
```
## Semicolons in JavaScript
- Semicolons are primarily used to mark the end of a statement. This helps the JavaScript engine understand the separation of individual instructions, which is crucial for correct execution.
- Semicolons help prevent ambiguities in code execution and ensure that statements are correctly terminated.

## Comments in JavaScript
- Any line of code that is commented out is ignored by the JavaScript engine. Comments are used to explain code, make notes, or temporarily disable code.
- Single-line comments are created using //.
- Multi-line comments are created using /* to start the comment and */ to end the comment.

## JavaScript as a Dynamically Typed Language
- JavaScript is a dynamically typed language, which means that you don't have to specify the data type of a variable when you declare it. The JavaScript 
```javaScript
engine automatically determines the data type based on the value assigned to the variable.
let error = 404; // JavaScript treats error as a number
error = "Not Found"; // JavaScript now treats error as a string
```
- Other languages, like C#, that are not dynamically typed would result in an error:
```JavaScript
int error = 404; // value must always be an integer
error = "Not Found"; // This would cause an error in C#
```
## Using the typeof Operator
- The typeof operator is used to check the data type of a variable. It returns a string indicating the type of the variable.
- However, there's a well-known quirk in JavaScript when it comes to null. The typeof operator returns "object" for null values.
```Js
let user = null;
console.log(typeof user); // "object"
```