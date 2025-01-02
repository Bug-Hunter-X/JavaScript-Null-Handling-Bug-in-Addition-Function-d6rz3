# JavaScript Null Handling Bug

This repository demonstrates a common yet subtle bug in JavaScript related to null value handling within a simple addition function.

## Bug Description
The `foo` function is designed to add two numbers. However, it prematurely returns 0 if either input is null, even if the other input is a valid number.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js`.
3. Run the code in a JavaScript environment (e.g., Node.js, browser console).
4. Observe the output; it will show 0 for cases where one or both inputs are null, which is incorrect behavior for a simple addition operation.

## Solution
The solution involves more robust null handling. Instead of returning 0 immediately, the function should either explicitly check for null values and handle them separately, or use a technique like the nullish coalescing operator (??) to provide default values.  See `bugSolution.js` for a corrected implementation.

## Lessons Learned
This example highlights the importance of thorough null checking and appropriate handling of edge cases in JavaScript to avoid unexpected behavior and potential errors.