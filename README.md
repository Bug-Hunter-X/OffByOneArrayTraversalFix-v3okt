# Off-by-One Error in Java Array

This repository demonstrates a common off-by-one error in Java when iterating over an array. The error occurs when the loop condition is `i <= array.length`, which causes an attempt to access an index beyond the array's bounds.

The `Bug.java` file contains the erroneous code. The `BugSolution.java` file provides a corrected version.

## How to Reproduce

1. Compile `Bug.java`.
2. Run the compiled code. An `ArrayIndexOutOfBoundsException` will be thrown.

## Solution

The solution involves modifying the loop condition to `i < array.length`. This ensures that the loop terminates before attempting to access the non-existent element at index `array.length`.