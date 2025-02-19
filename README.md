# Uncommon HTML Bug: Accessing Non-Existent Element

This repository demonstrates a subtle bug in HTML that can be difficult to track down. The core issue involves attempting to modify the content of an element using `getElementById()` when that element doesn't actually exist in the HTML structure. 

## Bug Description
The `bug.html` file contains a script that attempts to access and modify an element with the ID `myDiv2`. However, this element isn't defined in the HTML.  This results in the script failing silently—no errors are thrown, but the intended change doesn't happen and it could cause unexpected behavior in larger applications.

## Solution
The `bugSolution.html` file corrects this by ensuring the target element exists before attempting to modify it.  Proper error handling is added to gracefully handle situations where the element is not found.  This ensures that the application doesn't crash and provides useful debugging information.