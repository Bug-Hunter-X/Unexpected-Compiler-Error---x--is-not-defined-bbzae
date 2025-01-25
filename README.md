# ActionScript 3 Compiler Error: Variable Used Before Declaration

This repository demonstrates a subtle ActionScript 3 compiler error related to variable usage before declaration.  Even when the declaration is within the same function's scope, the compiler may throw an error if the variable's use precedes its definition, particularly in control flow structures like `if` statements or loops where the compiler might not be able to ascertain execution order definitively.

The `bug.as` file showcases the problematic code.  The `bugSolution.as` file offers a corrected version.

## How to Reproduce

1. Compile `bug.as` using an ActionScript 3 compiler (like the one included with Adobe Flex or an alternative compiler).
2. Observe the compiler error indicating that the variable is undefined.