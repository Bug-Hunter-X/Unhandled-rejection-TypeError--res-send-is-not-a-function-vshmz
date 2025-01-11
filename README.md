# Unhandled rejection TypeError: res.send is not a function
This repository demonstrates a common error in Express.js applications: the `Unhandled rejection TypeError: res.send is not a function` error. This error typically arises when you attempt to use `res.send()` outside the context of a request handler (e.g., within a middleware function or outside the route definition).

## Bug
The bug is in `bug.js`. The code attempts to use `res.send()` in a place where it's not accessible.

## Solution
The `bugSolution.js` file demonstrates the correct usage of `res.send()` within the route handler.

## How to Reproduce
1. Clone this repository.
2. Navigate to the directory.
3. Run `node bug.js`.
4. Observe the error message.
5. Then, run `node bugSolution.js` to see the corrected version.