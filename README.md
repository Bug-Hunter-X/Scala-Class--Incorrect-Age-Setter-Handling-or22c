# Scala Class: Incorrect Age Setter Handling

This repository demonstrates a common error in Scala class design: improper handling of invalid input in a setter method. The `MyClass` class includes a setter for the `age` property that doesn't explicitly address the case of negative ages.

The `MyClassSolution.scala` file provides a corrected version with improved error handling.

**Bug:** The original `MyClass` setter silently allows negative ages to be assigned, which is incorrect in this context.

**Solution:** The solution throws an `IllegalArgumentException` when a negative age is provided, ensuring that the `age` property maintains its valid state.