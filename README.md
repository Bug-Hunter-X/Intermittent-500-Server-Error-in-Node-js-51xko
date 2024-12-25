# Intermittent 500 Server Error in Node.js

This repository demonstrates a scenario where a Node.js server intermittently throws a 500 error due to an issue within an asynchronous operation. The error is not consistently reproducible, which adds to its difficulty in detection and resolution.

## Bug Description
The `bug.js` file contains a simple HTTP server.  Due to the random nature of the error simulation in the `setTimeout` callback, the server may randomly return either a successful response (200 OK) or a 500 Internal Server Error. This makes debugging difficult as it doesn't present itself consistently.

## Bug Solution
The `bugSolution.js` file demonstrates how to mitigate the issue by introducing proper error handling to catch and manage any potential errors within the asynchronous operation.