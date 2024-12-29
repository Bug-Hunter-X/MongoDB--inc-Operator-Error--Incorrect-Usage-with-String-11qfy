# MongoDB $inc Operator Error: Incorrect Usage with String

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries: providing a string value instead of a numerical value. This results in unexpected behavior or an error.

## Bug Description
The `$inc` operator is used to increment a numerical field by a given value.  If a string is provided as the increment value, MongoDB cannot perform the mathematical operation and will either throw an error or produce incorrect results. This bug showcases this specific error scenario.

## Bug Reproduction
The `bug.js` file contains the code that demonstrates the error. Running this code against a MongoDB collection will reproduce the unexpected behavior or error.

## Bug Solution
The `bugSolution.js` file shows the correct usage of the `$inc` operator using a numerical value for incrementing the field.

## How to Run
1. Ensure you have Node.js and a MongoDB instance running.
2. Clone this repository.
3. Run `npm install` to install dependencies (if needed).
4. Run `node bug.js` and `node bugSolution.js` to see the difference in behavior.
