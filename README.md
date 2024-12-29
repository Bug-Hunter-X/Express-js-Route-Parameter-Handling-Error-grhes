# Express.js Route Parameter Handling Bug

This repository demonstrates a common error in Express.js applications related to handling route parameters and potential database query failures.  The `bug.js` file contains the erroneous code, and `bugSolution.js` provides a corrected implementation with robust error handling.

## Problem Description:
The original code doesn't handle the scenario where a user with the specified ID is not found in the database. This can lead to errors or unexpected behavior in the application.

## Solution:
The solution adds comprehensive error handling to check if the database query returns a valid user object before sending a response.  It returns an appropriate 404 status code if the user is not found.