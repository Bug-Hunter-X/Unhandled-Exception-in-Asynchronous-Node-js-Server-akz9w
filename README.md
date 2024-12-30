# Unhandled Exception in Asynchronous Node.js Server

This repository demonstrates a common error in Node.js: an unhandled exception within an asynchronous callback.  The server simulates an operation that might fail; if it fails, an error is thrown, causing the server to crash without proper error handling.

## Bug Description
The provided `bug.js` file contains a simple HTTP server.  The server simulates an asynchronous operation using `setTimeout`. If a random number is less than 0.5, the response is successful. Otherwise, an error is thrown without proper handling, causing the server to terminate unexpectedly. 

## Bug Solution
The `bugSolution.js` file demonstrates how to properly handle this error using a `try...catch` block within the asynchronous operation.