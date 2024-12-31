# JavaScript Function Bug: Null Handling

This repository demonstrates a common bug in JavaScript functions related to null value handling. The `foo` function is intended to add two numbers, but it incorrectly returns `null` when either input is `null`.

## Bug Description

The `foo` function uses `==` for comparison. This does not work as expected when comparing null with 0.  The function should return 0 when either `a` or `b` is `null`. 

## Bug Solution

The `bugSolution.js` file provides a corrected version of the function, addressing the null handling issue using strict equality and explicit checks for null values. It now returns 0 when either parameter is null, and it correctly returns a + b otherwise.