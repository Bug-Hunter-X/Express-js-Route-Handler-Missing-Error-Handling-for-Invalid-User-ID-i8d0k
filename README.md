# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling when dealing with potentially invalid user input.

The `bug.js` file shows the faulty code, attempting to parse a user ID from the request parameters without any checks.  This can lead to runtime errors if the ID is not a valid integer or is missing altogether.

The `bugSolution.js` file provides a corrected version with improved error handling.  It checks for the presence of the ID and its validity as an integer, gracefully handling cases where the ID is invalid or the user is not found.