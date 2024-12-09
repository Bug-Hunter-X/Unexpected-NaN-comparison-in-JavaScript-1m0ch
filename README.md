# Unexpected NaN Comparison in JavaScript

This repository demonstrates a common, yet subtle, error in JavaScript related to the comparison of NaN (Not a Number) values.

## The Bug

JavaScript's loose comparison (==) and strict comparison (===) operators behave unexpectedly when comparing NaN values.  The `===` operator, in particular, will always return `false` even when comparing `NaN` with itself. This can lead to unexpected behavior in programs where NaN values are handled.

## The Solution

The most robust way to check for NaN is to use the `isNaN()` global function which returns `true` if the value is NaN and `false` otherwise.