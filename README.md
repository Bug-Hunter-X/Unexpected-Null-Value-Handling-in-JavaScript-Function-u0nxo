# Unexpected Null Value Handling in JavaScript Function

This repository demonstrates a common error in JavaScript: improper handling of null values passed as function parameters.

## The Problem

The `foo` function in `bug.js` doesn't explicitly handle cases where either `a` or `b` is `null`.  If `null` is passed in, it might lead to unexpected behavior or runtime errors (e.g., `TypeError: Cannot read properties of null (reading 'someProperty')`).

## The Solution

`bugSolution.js` provides a corrected version of the function which first checks for `null` values and returns an appropriate value (in this case, `null`) if either parameter is null.  This prevents the errors caused by trying to operate on null values.

## How to run

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in your favorite code editor.
3. Compare the two functions to see the difference.
4. Test the functions by calling them with various arguments, including `null` values.