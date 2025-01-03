# ActionScript 3 Null/Undefined String Parameter Bug

This repository demonstrates a subtle bug in ActionScript 3 related to handling null or undefined parameters in string operations.  When a function receives null or undefined string parameters, unexpected errors or crashes can occur due to how ActionScript handles these cases.

## Bug Description
The bug manifests when a function attempts to concatenate strings without first checking for null or undefined values. In ActionScript 3, performing string operations on null or undefined variables can lead to errors.

## Solution
The solution involves adding checks to handle these cases. Before concatenating the strings, the code should verify that the parameters are not null or undefined. If they are, an appropriate error message or action can be taken.

## How to reproduce
1.  Compile and run the file `bug.as` using an ActionScript 3 compiler (like the one included with Adobe Flash Professional or a command-line compiler like ASC 2.0).
2. Notice the errors when attempting to run it using `null` or `undefined` parameters.
3.  Compile and run the solution in `bugSolution.as` to observe the improved error handling.
