# MongoDB $inc operator error
This repository contains a bug report and solution for an incorrect usage of the MongoDB $inc operator. The bug arises from passing a non-numeric value to the $inc operator in an update query, resulting in an error.
## Bug Description
The $inc operator in MongoDB is used to increment a numerical field by a specified value. However, if a non-numeric value is passed to the $inc operator, the update operation will fail.
## Bug Solution
The solution involves ensuring that the value passed to the $inc operator is a number.  This can be done by explicitly converting the value to a number or by ensuring that the field being incremented already contains a number.
## Files
- `bug.js`: Demonstrates the incorrect usage of the $inc operator.
- `bugSolution.js`: Demonstrates the correct usage of the $inc operator.