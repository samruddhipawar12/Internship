#SpreadOperator

    The spread operator in JavaScript (...) is a powerful feature that allows you to "spread" the elements of an array, object, or other iterable structures into individual elements. It's often used in a variety of contexts, such as copying objects or arrays, combining them, or passing them as arguments to functions.
    The spread operator (...) is a powerful feature introduced in ES6 (ES2015) that allows you to expand iterable objects (like arrays, strings, or objects) into individual elements.


Important Notes:
    The spread operator performs a shallow copy. It copies only the first level of the object or array. If the object or array contains nested structures, those will be copied by reference, not by value.

    The spread operator is used primarily for copying and merging arrays/objects but is also handy for extracting and collecting elements or properties in various contexts. 



1. Spreading an Array
You can use the spread operator to expand an array into individual elements.

const arr = [1, 2, 3];
const newArr = [...arr, 4, 5];

console.log(newArr); // [1, 2, 3, 4, 5]


2. Spreading an Object
You can use the spread operator to copy or merge objects.

const obj = { name: "John", age: 25 };
const newObj = { ...obj, city: "New York" };

console.log(newObj); // { name: "John", age: 25, city: "New York" }

3. Merging Arrays
You can combine multiple arrays into a single array.

const arr1 = [1, 2];
const arr2 = [3, 4];
const mergedArr = [...arr1, ...arr2];

console.log(mergedArr); // [1, 2, 3, 4]

4. Cloning an Array or Object
The spread operator is commonly used to create shallow copies of arrays or objects.

const arr = [1, 2, 3];
const clonedArr = [...arr];

console.log(clonedArr); // [1, 2, 3]


