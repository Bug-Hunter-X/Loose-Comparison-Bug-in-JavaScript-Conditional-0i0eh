# Loose Comparison Bug in JavaScript

This repository demonstrates a common JavaScript bug caused by using loose comparison (==) instead of strict comparison (===) in conditional statements. Loose comparison can lead to unexpected behavior when comparing values of different types.

## Bug Description
The provided JavaScript function `foo` uses loose comparison to check for null values.  This can lead to unexpected results.  For instance, `0 == false` evaluates to `true`, which can cause the function to return 0 even when `a` and `b` are not null but are equivalent to `false` (e.g., 0).

## Bug Solution
The solution replaces the loose comparison (==) with strict comparison (===). Strict comparison checks for both value and type equality, preventing the unexpected behavior observed with loose comparison. 

## How to Reproduce
1. Clone this repository.
2. Run `bug.js` in a JavaScript environment (browser console or Node.js).
3. Observe that the function produces incorrect results in certain cases due to loose comparison.
4. Run `bugSolution.js` to see the correct implementation using strict comparison.