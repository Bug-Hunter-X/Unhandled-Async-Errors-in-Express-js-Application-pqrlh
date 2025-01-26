# Unhandled Async Errors in Express.js

This repository demonstrates a common error in Express.js applications: the lack of proper error handling for asynchronous operations.

The `bug.js` file contains an Express.js app with an asynchronous operation (`someAsyncOperation`) that might throw an error.  However, the error isn't handled correctly, resulting in a silent failure or application crash.

The `bugSolution.js` file provides a corrected version of the application with appropriate error handling to ensure a graceful response even if the async operation fails.

## How to Reproduce

1. Clone the repository.
2. Navigate to the directory.
3. Run `npm install` to install Express.js.
4. Run `node bug.js` to see the unhandled error behavior.
5. Run `node bugSolution.js` to see the improved error handling.

## Lesson Learned
Always handle potential errors in your asynchronous operations to prevent application crashes and provide better user experiences.  Use try...catch blocks or promises' `.catch()` method to gracefully handle errors that may occur during the execution of asynchronous code within your Express.js application.