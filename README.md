# F# Mutable Variable Swap Bug

This repository demonstrates a common error when working with mutable variables in F#.  The `swap` function, intended to exchange the values of two variables, unexpectedly modifies the original variables instead of creating copies.

## The Bug
The issue stems from F#'s behavior with mutable variables. When passed to a function, these variables are passed by reference. Therefore, any modifications made within the function directly affect the original variables.

## The Solution
The solution involves creating copies of the variables before performing the swap operation. This ensures that the original values remain unchanged.