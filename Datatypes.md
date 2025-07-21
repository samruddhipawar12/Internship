#Datatypes

  In JavaScript, primitive data types are the most basic types of data that are immutable (i.e., their values cannot be changed once they are set). These are not objects and are not stored by reference. In total, JavaScript has 7 primitive data types:

1. Number
Represents both integer and floating-point numbers.

Includes positive and negative numbers, infinity (Infinity), negative infinity (-Infinity), and NaN (Not-a-Number).

Example:

let age = 25;            // integer
let temperature = 36.6;  // floating-point
let infinityValue = Infinity;
let notANumber = NaN;
Key Points:

No separate types for integer and floating-point numbers. Both are represented as Number.

Operations on numbers that result in an undefined result (like dividing by 0) will return special values such as Infinity, -Infinity, or NaN.

2. String
Represents a sequence of characters enclosed in single quotes (' ') or double quotes (" "), or even template literals (backticks ` `).

Example:
let name = "John Doe";        // double quotes
let greeting = 'Hello!';      // single quotes
let templateString = `Hi, ${name}`; // template literal
Key Points:

Strings are immutable, meaning once created, you cannot change individual characters of a string.

You can perform various string methods like .concat(), .substring(), .toUpperCase(), .split(), etc.

3. Boolean
Represents one of two values: true or false. Boolean values are used for logical operations.

Example:

let isJavaScriptFun = true;
let isOld = false;
Key Points:

Used in conditions and logical expressions like if, while, etc.

Booleans are typically the result of comparison operators (e.g., ==, ===, >, <).

4. Undefined
A variable that has been declared but not assigned a value has the value undefined.

Example:

let a;
console.log(a); // undefined
Key Points:

The undefined type is also the default value for uninitialized variables or function parameters that aren't passed any arguments.

5. Null
Represents the intentional absence of any value or object. It is often used as a placeholder when no value is assigned.

Example:

let person = null;
Key Points:

null is a special value. It’s different from undefined and can be assigned to a variable to indicate the absence of an object or value.

6. Symbol (ES6 and later)
A unique and immutable primitive value primarily used to create object properties that are unique (i.e., not accidental clashes with existing property names).

Example:

const uniqueSymbol = Symbol('description');
Key Points:

Every time you create a new symbol, it is guaranteed to be unique, even if the description is the same.

Symbols are often used to create unique object keys, preventing accidental overwriting of properties.

7. BigInt (ES11 and later)
Represents whole numbers larger than the Number type can safely represent (larger than 2^53 - 1).

Example:

const bigNumber = BigInt(1234567890123456789012345678901234567890);
const bigIntFromString = BigInt("1234567890123456789012345678901234567890");
Key Points:

BigInt can handle numbers that exceed the range of the Number type (which is approximately ±(2^53 - 1)).

You can perform arithmetic operations with BigInt, but you cannot mix it with regular Number types directly.

Key Characteristics of Primitive Data Types:
  1. Immutability: Once a primitive value is assigned, it cannot be modified. For instance, strings are immutable, so any operation on a string creates a new string.

  2. Pass-by-Value: Primitive types are copied by value. This means when you assign a primitive value to a variable or pass it to a function, a copy of the value is passed, and changes to the copy do not affect the original.

  3. No Properties or Methods: Primitive types do not have properties or methods. However, JavaScript temporarily wraps primitive values in their object equivalents (like String, Number, etc.) to allow access to methods.


How Primitive Data Types Work:
Assignment: When you assign a primitive value to a variable, it is directly stored in that variable.

let a = 10;  // 'a' holds the value 10.
let b = a;   // 'b' also gets a copy of the value 10.
a = 20;      // Changing 'a' does not affect 'b'.
console.log(b);  // 10, 'b' still holds the original value.
Operations: When you perform operations on primitive values, they return new values without altering the original.

let str = "Hello";
str = str + " World";  // String concatenation returns a new string.
console.log(str);  // "Hello World"