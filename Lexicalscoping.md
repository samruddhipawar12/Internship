#LexicalScoping.md

  Lexical Scoping in JavaScript
Lexical scoping is a fundamental concept in JavaScript (and many other programming languages) that determines the visibility and lifetime of variables based on where they are defined in the code.

In simple terms, lexical scoping means that the scope of a variable is determined by the physical structure of the code—its position within the source code. This is different from dynamic scoping, where the scope would depend on the call stack (the runtime execution context).

How Lexical Scoping Works in JavaScript:
   1.Function Scope: Variables declared inside a function are only accessible within that function, even if the function is called from another scope.
   2.Block Scope (with let and const): Variables declared with let or const inside a block (e.g., if, for, etc.) are scoped to that block.
   3.Global Scope: Variables declared outside of any function or block are in the global scope and can be accessed anywhere in the code.

Key Takeaways:
  Lexical scoping means that a variable's scope is determined by where it is written in the code, not where it is called.
  Variables are accessible within the scope in which they are defined, and inner functions can access variables from their outer function scopes.
  Closures are created when an inner function retains access to variables from its lexical scope, even after the outer function has returned.
  This is one of the key concepts that enable powerful JavaScript patterns, like closures and callback functions.