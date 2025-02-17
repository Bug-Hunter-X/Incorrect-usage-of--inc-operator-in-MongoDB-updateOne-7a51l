# MongoDB $inc Operator Usage Error

This repository demonstrates an incorrect usage of the `$inc` operator in a MongoDB `updateOne` operation.  The example shows how providing a string instead of a number to the `$inc` operator leads to unexpected behavior and potential data corruption.  The solution demonstrates the correct usage of the operator.

## Bug
The original code attempts to increment a field by a string value, which is not supported. This leads to an error and/or unexpected data manipulation.  The specific error depends on the version of MongoDB and the schema of your collection.

## Solution
The solution corrects the code by providing the correct numeric value to the `$inc` operator.  The value to be incremented should always be a numerical value.