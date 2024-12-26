# MongoDB $inc operator error with string value
This repository demonstrates an uncommon error that can occur when using the $inc operator in MongoDB update queries.  The error involves providing a string value instead of a numeric value to the $inc operator. This example uses Javascript.

## Bug Description
The bug occurs when a string value is used with the `$inc` operator in a MongoDB update operation. The expected behavior is to increment the field's value by the specified amount. However, when a string is used, MongoDB may not increment correctly, potentially leading to unexpected results or an error.

## Bug Solution
The solution involves ensuring that the value passed to the `$inc` operator is a number (integer or float) instead of a string.  The code in `bugSolution.js` demonstrates this correction.