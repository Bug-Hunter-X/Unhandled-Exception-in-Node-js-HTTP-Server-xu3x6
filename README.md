# Unhandled Exception in Node.js HTTP Server

This repository demonstrates an example of an unhandled exception in a Node.js HTTP server and how to properly handle it.

## Bug

The `bug.js` file contains a Node.js HTTP server that throws an error if the request URL is '/error'.  However, this error is not caught, causing the server to crash.

## Solution

The `bugSolution.js` file provides a corrected version of the server.  It uses a `try...catch` block to handle the error gracefully and prevents the server from crashing.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `node bug.js`.
4. Open your browser and navigate to `http://localhost:3000/error`. You will see that the server crashes.
5. Run `node bugSolution.js`.
6. Open your browser and navigate to `http://localhost:3000/error`. You will see an error message in the console, but the server will remain running.

## Learning Points

* The importance of proper error handling in Node.js applications.
* How to use `try...catch` blocks to handle exceptions.
* The use of event listeners for handling server errors.