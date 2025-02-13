# F# Mutable Variable Swap Bug

This example demonstrates a common error when working with mutable variables in F#.  The `swap` function appears to swap the values of `x` and `y`, but due to pass-by-reference semantics, it actually modifies the original variables directly.

## Bug Description
The code attempts to swap two mutable variables using a function. However, because mutable variables are passed by reference, the function modifies the original variables, leading to incorrect results.  The solution shows the proper way to handle this using tuples.