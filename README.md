# Unhandled Promise Rejection in Node.js Express.js Application

This repository demonstrates a common error in Node.js applications: unhandled promise rejections.  The `bug.js` file contains code that simulates an asynchronous operation within an Express.js route handler.  If an error occurs within the `setTimeout` callback, the application will crash without proper error handling. The `bugSolution.js` file showcases how to handle this type of error effectively.

## How to Reproduce

1. Clone this repository.
2. Run `npm install express` to install the necessary dependencies.
3. Run `node bug.js`.
4. Observe that the application might crash randomly due to an unhandled promise rejection if the random condition is met.

## Solution

The `bugSolution.js` file provides a solution for handling the error effectively using a `try...catch` block within the asynchronous operation or by adding an error handling mechanism using `.catch()` method.