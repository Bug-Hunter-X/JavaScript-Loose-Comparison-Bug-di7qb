# JavaScript Loose Comparison Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to loose comparison (==) and how it can lead to unexpected results.

## The Bug

The `foo` function in `bug.js` intends to check if two variables are equal. However, due to JavaScript's loose comparison, it doesn't always work as expected.

Loose comparison does type coercion, leading to comparisons that might seem counterintuitive.

## The Solution

The solution in `bugSolution.js` demonstrates the use of strict equality (===) to avoid type coercion. Strict equality requires that both the values and the data types are the same for the comparison to be true.