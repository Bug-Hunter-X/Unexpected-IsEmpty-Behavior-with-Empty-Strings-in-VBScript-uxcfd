# Unexpected IsEmpty Behavior with Empty Strings in VBScript

This repository demonstrates an uncommon error related to VBScript's `IsEmpty` function. The function doesn't correctly identify empty strings as empty, leading to unexpected behavior when performing mathematical operations.

## Bug Description

The provided VBScript code intends to add two values, defaulting to 0 if either is empty. However, `IsEmpty` incorrectly evaluates empty strings as non-empty, leading to incorrect summation.

## Solution

The solution involves using the `Len` function to check the length of strings. If the length is 0, the string is considered empty.