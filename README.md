# Uncommon HTML Error: Accessing Non-Existent Attributes

This repository demonstrates a subtle error that can occur when working with HTML and JavaScript.  The bug involves attempting to access an attribute of a DOM element that doesn't actually exist.

## The Problem

The `bug.html` file contains JavaScript code that tries to access a non-existent attribute (`myNonExistentAttribute`) of an element with the ID `myDiv`.  This does not throw an error, but results in `undefined` being assigned to the variable `myVariable`. If code later assumes this variable holds a meaningful value, errors might occur.

## The Solution

The `bugSolution.html` file shows how to avoid this issue.  Before accessing the attribute, the code checks if it exists, preventing errors and potential unexpected behavior.