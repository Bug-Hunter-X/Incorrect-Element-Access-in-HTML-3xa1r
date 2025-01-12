# Uncommon HTML Bug: Incorrect Element Access

This repository demonstrates a common yet subtle error in HTML and JavaScript interaction: incorrectly accessing a DOM element using `getElementsByTagName`.  The example shows how to correctly use `getElementById` for accessing single elements.

## Bug Description

The `bug.html` file contains a simple HTML page with a div element. The JavaScript code attempts to hide this div, but it does it incorrectly using `getElementsByTagName`.  This function returns a collection (NodeList) even if there's only one matching element, so you need to select the specific index.

## Solution

The `bugSolution.html` file demonstrates the correct way to select the element using `getElementById`, ensuring that you only target the correct element. 

This is an important detail to be aware of in order to avoid unexpected behavior and errors in web development. 