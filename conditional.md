#conditionals
  🔀 Conditionals in JavaScript
Conditionals let you run different blocks of code depending on whether a condition is true or false.

✅ 1. if Statement

  if (condition) {
    // code to run if condition is true
   }

Example:
let age = 18;

if (age >= 18) {
  console.log("You are an adult.");
}


✅ 2. if...else Statement

if (condition) {
  // code if condition is true
} else {
  // code if condition is false
}

Example:
let age = 16;

if (age >= 18) {
  console.log("You can vote.");
} else {
  console.log("You are too young to vote.");
}
✅ 3. if...else if...else Chain
Use when checking multiple conditions.
let score = 85;

if (score >= 90) {
  console.log("Grade: A");
} else if (score >= 80) {
  console.log("Grade: B");
} else if (score >= 70) {
  console.log("Grade: C");
} else {
  console.log("Fail");
}


✅ 4. Ternary Operator (Shorthand if...else)

condition ? expressionIfTrue : expressionIfFalse;
Example:

let isLoggedIn = true;
let message = isLoggedIn ? "Welcome back!" : "Please log in.";
console.log(message);


✅ 5. switch Statement
Used for checking one variable against many possible values.

let fruit = "apple";

switch (fruit) {
  case "apple":
    console.log("Apples are $1 each.");
    break;
  case "banana":
    console.log("Bananas are $0.50 each.");
    break;
  case "orange":
    console.log("Oranges are $0.80 each.");
    break;
  default:
    console.log("Sorry, we don't have that fruit.");
}
🔹 break is important to stop checking after a match.
🔹 default runs if no cases match.



