# Silent JavaScript Error: Accessing a Non-Existent Element

This repository demonstrates a common yet subtle bug in HTML/JavaScript interactions: attempting to manipulate a DOM element that doesn't exist. This example highlights the importance of robust error handling and careful DOM manipulation.

The `bug.html` file contains the problematic code.  The `solution.html` demonstrates a corrected version using conditional checks to prevent errors.

## Bug

The bug lies in the JavaScript code which tries to access an element with the ID 'myNonExistentDiv'. Because no such element exists in the HTML, this results in a silent error in the browser's console. This can be challenging to track because there is no immediate visual indication of the problem, potentially leading to unforeseen consequences.

## Solution

The solution involves adding a check to see if the element exists before attempting to access it. The corrected code employs `getElementById()` to retrieve the element and checks if the result is null before performing the style change.