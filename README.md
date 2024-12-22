# Incorrect Usage of $inc Operator in MongoDB Update Query

This repository demonstrates a common error when using the `$inc` operator in MongoDB update queries. The error occurs when using a string instead of a number with the `$inc` operator.

## Bug
The original code attempts to increment the value of a field using `$inc` with a string value. This results in unexpected behavior and incorrect data updates. The `$inc` operator requires a numerical value for incrementing fields.

## Solution
The corrected code uses a numerical value with the `$inc` operator, ensuring that the field is incremented correctly.

## How to reproduce the bug
1. Connect to your MongoDB instance.
2. Create a sample collection.
3. Execute the incorrect query from `bug.js`.
4. Observe the unexpected update result.
5. Run the correct query from `bugSolution.js` and verify the correct incremented value.
