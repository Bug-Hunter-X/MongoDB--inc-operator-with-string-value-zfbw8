# MongoDB $inc operator with string value
This repository demonstrates an uncommon bug related to the MongoDB $inc operator.
The issue occurs when attempting to increment a field using a string value instead of a numerical one. This results in unexpected behavior and potential data corruption.
## Bug Description
The primary cause of the bug is using an incorrect data type with the $inc operator. The $inc operator requires a numerical value, but providing a string value leads to the query failing silently or producing unintended results.
## Solution
The solution is to ensure that the value provided to the $inc operator is a number. This resolves the issue and ensures that the data is updated correctly.