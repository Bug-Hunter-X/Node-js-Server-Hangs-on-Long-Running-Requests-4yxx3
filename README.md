# Node.js Server Hanging Issue

This repository demonstrates a common issue in Node.js where a long-running request can cause the server to hang, becoming unresponsive to other requests.  The original `server.js` showcases this problem. The solution is provided in `serverSolution.js`.

**Problem:** The server performs a 5-second CPU-bound task within the request handler.  During this time, the server cannot process other requests, leading to a hang.

**Solution:** Employ techniques like asynchronous operations or worker threads to handle long-running tasks concurrently without blocking the main event loop.

The solution demonstrates the use of asynchronous operations for a non-blocking server operation.