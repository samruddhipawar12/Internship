#objects

  🧱 Objects in JavaScript
In JavaScript, an object is a collection of key-value pairs used to store multiple values in a single variable.

   1. Creating an Object
a. Using Object Literal (most common):

const person = {
  name: "Alice",
  age: 30,
  isStudent: false
};
b. Using the new Object() syntax:

const person = new Object();
person.name = "Alice";
person.age = 30;


 2. Accessing Object Properties
 Method	              Syntax Example
Dot notation	      person.name
Bracket notation	  person["name"]

console.log(person.name);      // "Alice"
console.log(person["age"]);    // 30


 3. Modifying Object Properties

person.age = 31;              // Update
person.city = "New York";     // Add new property


 4. Deleting Properties

delete person.isStudent;

 5. Object Methods
You can store functions inside objects — these are called methods.

const person = {
  name: "Alice",
  greet: function() {
    console.log("Hello, I'm " + this.name);
  }
};

person.greet(); // Output: Hello, I'm Alice

 6. Nested Objects
Objects can contain other objects or arrays.
const user = {
  name: "Bob",
  address: {
    city: "London",
    zip: "12345"
  },
  hobbies: ["reading", "gaming"]
};

console.log(user.address.city);  // "London"
console.log(user.hobbies[0]);    // "reading"

 7. Looping Through Object Properties
for (let key in person) {
  console.log(key + ": " + person[key]);
}

8. Built-in Object Methods
Method	Description
Object.keys(obj)	Returns an array of keys
Object.values(obj)	Returns an array of values
Object.entries(obj)	Returns key-value pairs as arrays
hasOwnProperty(key)	Checks if property exists

Example:
const car = { make: "Toyota", model: "Corolla" };

console.log(Object.keys(car));    // ["make", "model"]
console.log(Object.values(car));  // ["Toyota", "Corolla"]
console.log(car.hasOwnProperty("make")); // true


 9. Object Destructuring
Extract properties into variables easily:
const { name, age } = person;
console.log(name); // "Alice"
