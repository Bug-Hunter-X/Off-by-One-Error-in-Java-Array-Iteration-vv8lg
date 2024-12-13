# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error in Java code that occurs when iterating over arrays. The bug causes an `ArrayIndexOutOfBoundsException` because the loop index goes beyond the valid array bounds.

The `bug.java` file contains the erroneous code, while `bugSolution.java` provides a corrected version.

## Bug

The bug is present in the `for` loop within the `main` method of `MyClass`. The loop condition `i <= arr.length` causes the loop to iterate one time too many, resulting in an attempt to access an element beyond the array's bounds. 

## Solution

The solution in `bugSolution.java` simply changes the loop condition to `i < arr.length`. This ensures that the loop iterates only up to, but not including, the last element of the array, thus avoiding the `ArrayIndexOutOfBoundsException`.