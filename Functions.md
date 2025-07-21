#Functions
 
    🔧 Functions in JavaScript
A function in JavaScript is a block of code designed to perform a specific task. Functions help you reuse code, organize logic, and improve readability.

 1. Declaring a Function

function greet() {
  console.log("Hello!");
}

 2. Calling a Function

greet(); // Output: Hello!

 3. Function with Parameters
You can pass parameters to make functions dynamic.


function greet(name) {
  console.log("Hello, " + name + "!");
}
greet("Alice"); // Output: Hello, Alice!


 4. Function with Return Value
Use return to return a value from the function.

function add(a, b) {
  return a + b;
}
let result = add(5, 3); // result = 8

 5. Function Expressions (Anonymous Functions)
Functions can also be assigned to variables.

const multiply = function(x, y) {
  return x * y;
};
console.log(multiply(4, 5)); // 20

 6. Arrow Functions (ES6)
Shorter syntax for writing functions.
const divide = (a, b) => {
  return a / b;
};

console.log(divide(10, 2)); // 5
For one-line returns:
const square = x => x * x;
console.log(square(4)); // 16

7. Default Parameters
You can give default values to parameters.

function greet(name = "Guest") {
  console.log("Hello, " + name + "!");
}
greet(); // Hello, Guest!


 8. Rest Parameters
Used to handle multiple arguments.
function sum(...numbers) {
  return numbers.reduce((acc, curr) => acc + curr, 0);
}

console.log(sum(1, 2, 3, 4)); // 10

 9. Callback Functions
Functions passed as arguments to other functions.

function greetUser(name, callback) {
  console.log("Hello, " + name);
  callback();
}

function sayBye() {
  console.log("Goodbye!");
}

greetUser("Alice", sayBye);
// Output:
// Hello, Alice
// Goodbye!


