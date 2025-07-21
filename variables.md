#Variables And Datatypes


In JavaScript, variables are used to store data, and data types define the kind of data that can be stored in a variable.

✅ 1. Declaring Variables
JavaScript provides three ways to declare variables:
 

  Keyword	       Description
   var        	  Function-scoped, older way to declare variables.
   let	          Block-scoped, modern and preferred for mutable variables.
  const	          Block-scoped, for variables that should not be reassigned.


  Example:

javascript

  var name = "Alice";
  let age = 25;
  const pi = 3.14159;


  ✅ 2. JavaScript Data Types
JavaScript has two categories of data types:

🔹 Primitive Data Types (immutable)
Type	           Example	              Description
String	          "hello"	          Text, enclosed in quotes.
Number             42, 3.14	          Integers and floats.
Boolean            true, false	      Logical values.
Undefined	       undefined	      Variable declared but not assigned.
Null	           null               Explicitly no value.
BigInt	           1234567890123      Large integers.
Symbol	          Symbol("id")	      Unique identifiers.

🔹 Non-Primitive (Reference) Types
Type	          Example	       Description
Object	        {name: "Bob"}	   Key-value pairs.
Array	         [1, 2, 3]	       List of items.
Function	    function() {}  	   Reusable blocks of code.


✅ 3. Checking Data Types
Use typeof to check a variable’s type:
typeof "hello";         // "string"
typeof 42;              // "number"
typeof true;            // "boolean"
typeof undefined;       // "undefined"
typeof null;            // "object" (quirk in JavaScript)
typeof {};              // "object"
typeof [];              // "object" (use Array.isArray() to check arrays)
typeof function(){};    // "function"



JavaScript is dynamically typed, meaning variables do not need a type declaration, and types can change.
    let x = 10;     // number
    x = "hello";    // now a string
