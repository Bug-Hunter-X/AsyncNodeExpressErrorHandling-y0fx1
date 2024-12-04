# Unhandled Error in Asynchronous Node.js Express.js App
This repository demonstrates a common error in asynchronous Node.js applications using Express.js: unhandled errors within asynchronous callbacks.
The `bug.js` file shows an Express.js server that simulates an asynchronous operation.  If a random number is less than 0.5, it returns 'Hello World!'.  Otherwise, it throws an error, causing the server to crash without any informative error message.
The `bugSolution.js` file provides a solution by using a `try...catch` block within the asynchronous callback to gracefully handle potential errors.  Error handling best practices for Node.js asynchronous functions are demonstrated.  This ensures that the server does not crash and allows for more robust error logging and reporting.