# MongoDB $inc Operator Unexpected Behavior
This repository demonstrates an uncommon error related to the MongoDB `$inc` operator when used to decrement a counter. The issue arises from using a negative value directly within the `$inc` operator, leading to incorrect counter updates.

## Bug Description
The original code attempts to decrement a counter in a MongoDB collection using the `$inc` operator with a negative value (-1).  However, instead of decrementation, this leads to unexpected behavior which might include data loss or inconsistency.

## Solution
The correct approach to decrement a counter uses the `$inc` operator with a positive integer value for the update. This ensures that a counter decrements correctly and prevents unexpected errors.