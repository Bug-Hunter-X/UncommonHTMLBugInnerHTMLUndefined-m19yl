# Uncommon HTML Bug: Setting innerHTML to Undefined

This repository demonstrates a subtle bug in HTML where setting the `innerHTML` property of an element to an undefined variable leads to unexpected behavior. The content within the targeted element is cleared, rather than producing an error.

## Bug Description
The bug lies in the script's attempt to assign an undefined variable `myVar` to the `innerHTML` of a div.  Modern browsers handle this quietly by effectively setting the `innerHTML` to an empty string. 

## Solution
The solution involves ensuring that the variable used for setting `innerHTML` is defined and contains the intended HTML content.