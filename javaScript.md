# Javascript

### 1. JavaScript Basics

- **Data Types**: What are the different data types in JavaScript? Can you explain the difference between `null` and `undefined`?
 ```
 Mainly we divide data into 2 different types: -1. Primivite Data Type, 2. Non- Primitive Data Type
 -----------------------------------
 1. Primitive Data/type: 
 - String, Number, Boolean, Bigint, Null, Undefined, Symbol.

 2. Non-Primitive Data/type: { Object }
 ```

 ### 2Q. How does type **coercion** work in javascript? give an example of an unexpected result due to type coercion.

 #### Type conversion is the process of converting a value from one type to another.
 - Type conversion can either be implicit (automatically done during code execution) or explicit (done by you the developer).

- **Implicit** Type Conversion is also known (and more commonly referred to) as **C**oercion while **Explicit** Type Conversion is also known as **T**ype Casting.
  ### Example: (concatenate) of a String + Number.
  ```
    const sum = 35 + "hello"

   console.log(sum)
   // 35hello

   console.log(typeof sum)
   // string
   ```
   it's happening becoz of JavaScript is weakly typed lanuague.
 ```
 https://www.freecodecamp.org/news/coercion-and-type-conversion-in-javascript/

 ```
 ## FUNCTIONS & SCOPE
 ### Function types:
 1Q. What is the difference between a function declaration and a function expression?
- 

Syntax:

Function Declaration:
javascript
Copy code
```
function myFunction() {
  // function body
}
Function Expression:
javascript
Copy code
var myFunction = function() {
  // function body
};
```
To declare a function, you use the function keyword and specify a name for the function. For example:
```
function generateName(name) {
  return `Hi, my name is ${name}`
}

const name = generateName("web devloper")
console.log(name)

// Hi, my name is web developer
```
----------------------------------

### you create a function expression and assign it to a variable that can be called.
```
const generateName = function(name) {
  return `Hi, my name is ${name}`
}

const name = generateName("full-stack developer")
console.log(name)

// Hi, my name is full-stack developer
ref :- https://www.freecodecamp.org/news/function-declaration-vs-function-expression/
```
### Scope and Hoisting: 
 `Can you explain the concept of scope and hoisting in JavaScript? How do they affect variable declarations?`

-  Hoisting is a JavaScript mechanism where variable and function declarations are put into memory during the compile phase. This means that no matter where functions and variables are declared, they are moved to the top of their scope regardless of whether their scope is global or local.

- Scope determines the accessibility of variables, objects, and functions from different parts `(Global, Functional, Block )` level of the code.

#### Affects of Variable Declarations:


