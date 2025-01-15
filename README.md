# React Native: Handling Null or Undefined Object Properties

This repository demonstrates a common error in React Native applications: attempting to access properties of objects that might be null or undefined.  It also shows how to effectively handle these situations to prevent runtime errors.

## The Problem

Accessing properties of null or undefined objects leads to `TypeError: Cannot read properties of undefined (reading 'property')` errors. This often occurs when dealing with asynchronous data fetching or navigating between screens.

## The Solution

The best way to prevent these errors is to use optional chaining (`?.`) and the nullish coalescing operator (`??`).

* **Optional Chaining (`?.`):** Safely accesses nested object properties, returning `undefined` if any part of the chain is null or undefined.
* **Nullish Coalescing (`??`):** Provides a default value if the expression on the left is `null` or `undefined`.

## Usage

Refer to the `bug.js` file for the example with the error, and `bugSolution.js` for the corrected code.