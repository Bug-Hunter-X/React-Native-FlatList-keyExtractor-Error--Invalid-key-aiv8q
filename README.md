# React Native FlatList KeyExtractor Error
This repository demonstrates a common error encountered when using the FlatList component in React Native: providing an invalid key to the `keyExtractor` function.  The `keyExtractor` function must return a unique string or number for each item in your data array.  Failure to do so results in errors and unexpected behavior.

## Bug Reproduction
The `bug.js` file contains the buggy code. Running this code will reproduce the error, demonstrating the issue of providing a null value as a key.

## Solution
The `bugSolution.js` file provides the corrected code.  The keyExtractor function now handles the case of a missing or invalid ID, providing a fallback unique key.