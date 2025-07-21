#Operators
 
  🔧 JavaScript Operators
Operators in JavaScript are symbols used to perform operations on values and variables. They're essential for everything from math calculations to logic comparisons and assignments.

✅ ### 1. Arithmetic Operators
Used to perform mathematical calculations.
   Operator      	Description	         Example	       Result
     +	           Addition	            5 + 3	          8
     -	           Subtraction     	    5 - 3	          2
     *	           Multiplication	      5 * 3	         15
     /	            Division	          6 / 2	          3
     %	          Modulus (remainder)  	5 % 2	          1
     **	           Exponentiation	      2 ** 3	        8
     ++	           Increment	          x++         	x = x+1
     --	           Decrement	          x--	          x = x-1

✅ 2. Assignment Operators
Used to assign values to variables.
Operator     Description            Example     Equivalent To 

  =            Assign                x = 10                
  +=        Add and assign           x += 5      x = x + 5  
  -=       Subtract and assign       x -= 3      x = x - 3  
  *=       Multiply and assign      x *= 2      x = x * 2   
  /=       Divide and assign         x /= 4      x = x / 4   
  %=       Modulus and assign       x %= 2      x = x % 2   
  **=      Exponent and assign      x **=3      x = x ** 3  

 ✅ 3. Relational (Comparison) Operators
Used to compare values and return true or false.

Operator	Description	                     Example	          Result
==	        Equal to (loose equality)	     5 == "5"	          true
===	        Equal to (strict equality)	   5 === "5"	        false
!=	        Not equal (loose)	             5 != "5"	          false
!==	        Not equal (strict)	           5 !== "5"	        true
>	          Greater than	                 5 > 3	            true
<	          Less than	                     5 < 3	            false
>=	        Greater than or equal to	     5 >= 5             true
<=	        Less than or equal to	         5 <= 3	            false

 ✅ 4. Logical Operators
Used to combine boolean expressions.

Operator	      Description     	Example	          Result
&&	            Logical AND	     true && false	    false
`		                                 `	            Logical OR
!	              Logical NOT	       !true	          false

 ✅ 5. String Operators
 The + operator is also used to concatenate strings.

javascript
e.g
let greeting = "Hello" + " " + "World!";
console.log(greeting); // "Hello World!"


✅ 6. Type Operators
Operator	     Description
typeof	        Returns the type of a variable
instanceof     	Checks if an object is an instance of a class

javascript
e.g
typeof "hello"; // "string"
[1,2,3] instanceof Array; // true


✅ 7. Ternary Operator
Shorthand for if...else.

javascript
e.g
let age = 18;
let canVote = (age >= 18) ? "Yes" : "No";
console.log(canVote); // "Yes"
