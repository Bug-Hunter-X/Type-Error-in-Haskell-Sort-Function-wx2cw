# Haskell Sort Function Type Error

This repository demonstrates a common type error encountered when using the `sort` function from `Data.List` in Haskell. The `sort` function requires a list of elements of the same type. Attempting to sort a list containing elements of different types will result in a type error.

## Bug

The bug is in the `main` function of `bug.hs`.  The list `xs` contains elements of different types (integers, strings, and booleans).  The `sort` function attempts to compare these incompatible types, resulting in a type error.

## Solution

The solution in `bugSolution.hs` demonstrates proper type handling.  Either use a homogenous list of the same data type or employ more advanced techniques like using a data type that handles multiple types (such as `Either`).