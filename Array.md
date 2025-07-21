#Array
   In JavaScript, an array is a data structure used to store multiple values in a single variable. Arrays can hold items of any type, including numbers, strings, objects, and even other arrays.

1. Creating an Array

// Using square brackets (most common)
let fruits = ["apple", "banana", "cherry"];

// Using the Array constructor
let numbers = new Array(1, 2, 3, 4);

2. Accessing Array Elements
console.log(fruits[0]); // "apple"
console.log(fruits[2]); // "cherry"

3. Array Properties and Methods
.length – returns the number of elements

.push() – adds an element to the end

.pop() – removes the last element

.shift() – removes the first element

.unshift() – adds an element to the beginning

.forEach() – executes a function for each item

.map() – creates a new array with the results of a function

.filter() – creates a new array with elements that pass a test

.includes() – checks if an array contains a certain value

Example:

let numbers = [1, 2, 3, 4, 5];

// Add an item
numbers.push(6);

// Remove last item
numbers.pop();

// Filter even numbers
let evens = numbers.filter(num => num % 2 === 0);

console.log(evens); // [2, 4]

4. Looping Through an Array

let colors = ["red", "green", "blue"];

for (let i = 0; i < colors.length; i++) {
  console.log(colors[i]);
}

// or using forEach
colors.forEach(color => {
  console.log(color);
});