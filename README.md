# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js where a long-running synchronous operation in the request handler causes the server to hang or become unresponsive.  The event loop is blocked, resulting in a poor user experience and inability to handle new requests.

## Bug

The `bug.js` file contains a server that simulates a long-running task within the request handler.  This task blocks the event loop and prevents the server from responding to subsequent requests.

## Solution

The `bugSolution.js` file demonstrates how to fix this issue by using asynchronous operations or offloading the long-running task to a worker thread or other process.