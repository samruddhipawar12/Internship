#ThisKeyword
 
     The this Keyword in JavaScript
In JavaScript, the this keyword refers to the object that is executing the current function. Its value depends on how and where the function is called.

1. this in the Global Scope

console.log(this); // Refers to the `window` object
In Node.js:
console.log(this); // Refers to an empty object (`{}`) in modules

 2. this Inside a Function (Non-strict vs Strict Mode)

function show() {
  console.log(this);
}

show(); // In non-strict mode: window (in browsers)
// In strict mode: undefined

 3. this Inside an Object Method
When a method is called using dot notation, this refers to the object before the dot.

const person = {
  name: "Alice",
  greet: function() {
    console.log("Hello, I'm " + this.name);
  }
};

person.greet(); // "Hello, I'm Alice"

 4. this Inside an Arrow Function
Arrow functions do not have their own this.
They inherit this from their surrounding (lexical) context.

const person = {
  name: "Bob",
  greet: () => {
    console.log("Hi, I'm " + this.name);
  }
};

person.greet(); // "Hi, I'm undefined" — because `this` is not `person`

 5. this in Constructor Functions
In constructor functions, this refers to the newly created object.

function Car(make, model) {
  this.make = make;
  this.model = model;
}

const myCar = new Car("Toyota", "Corolla");
console.log(myCar.make); // "Toyota"

 6. this in Event Handlers (DOM)
In regular functions, this refers to the DOM element that received the event.
document.getElementById("btn").addEventListener("click", function() {
  console.log(this); // The button element
});