#loops
  🔁 Loops in JavaScript
Loops let you repeat blocks of code until a condition is met — perfect for working with arrays, iterating values, or automating repetitive tasks.

 1. for Loop
Runs a block of code a specific number of times.

for (let i = 0; i < 5; i++) {
  console.log("Count: " + i);
}
Explanation:

i = 0 → Initialization

i < 5 → Condition to run

i++ → Increment step after each loop

 2. while Loop
Runs as long as the condition is true.

let i = 0;

while (i < 5) {
  console.log("While loop count: " + i);
  i++;
}


3. do while Loop
Runs at least once, then checks the condition.

let i = 0;

do {
  console.log("Do-While loop count: " + i);
  i++;
} while (i < 5);


4. for of Loop
Used to loop over iterables (like arrays, strings, etc.).


let colors = ["red", "green", "blue"];

for (let color of colors) {
  console.log(color);
}

5. for in Loop
Used to loop over object keys.


let person = { name: "Alice", age: 30, city: "New York" };

for (let key in person) {
  console.log(key + ": " + person[key]);
}
 6. Loop Control Keywords
Keyword    	Description
break	    Exits the loop early
continue	Skips the current iteration

Example with break and continue:


for (let i = 1; i <= 5; i++) {
  if (i === 3) continue;  // Skip 3
  if (i === 5) break;     // Stop at 5
  console.log(i);         // Output: 1, 2, 4
}
    Summary Table
Loop Type	       Use For
for          	Known number of iterations
while	        Unknown number, condition-based
do while	    Run at least once

