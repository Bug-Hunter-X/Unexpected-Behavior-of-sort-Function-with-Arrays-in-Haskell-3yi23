# Haskell Sort Function Bug

This repository demonstrates a common misunderstanding regarding the `sort` function in Haskell's `Data.List` module.  The `sort` function is designed to operate on lists, not arrays (which are not a native Haskell data structure). Using it with data structures that aren't lists (e.g., expecting array-like behavior from a list) can lead to unexpected results or compilation errors.

The `bug.hs` file contains code that illustrates this issue. The `bugSolution.hs` file demonstrates the correct way to use the `sort` function with lists.

## How to reproduce the bug

1.  Clone this repository.
2.  Run `bug.hs` using a Haskell compiler (e.g., GHC).  Notice the output does not match expected sorted array output.

## How to fix the bug

Refer to `bugSolution.hs` for the corrected implementation. The solution involves explicitly using lists and leveraging the `sort` function correctly. This ensures that the sorting operates correctly on lists.