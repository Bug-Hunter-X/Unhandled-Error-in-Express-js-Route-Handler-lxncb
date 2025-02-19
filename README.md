# Unhandled Error in Express.js Route Handler

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  Specifically, the `/users/:id` route attempts to parse the `id` parameter as an integer without validating it, potentially causing unexpected behavior or crashes if the `id` is not a valid number.

## Bug
The `bug.js` file contains the erroneous code.  It fetches a user by ID but doesn't handle cases where the ID is not a number or does not exist.

## Solution
The `bugSolution.js` file provides a corrected version.  It includes input validation and explicit error handling to gracefully manage invalid user IDs.