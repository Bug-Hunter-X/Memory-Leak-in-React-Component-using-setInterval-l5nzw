# React setInterval Memory Leak

This repository demonstrates a common mistake in React: using `setInterval` within a `useEffect` hook without proper cleanup. This leads to memory leaks because the interval continues to run even after the component unmounts.

The `bug.js` file contains the flawed code. The `bugSolution.js` file demonstrates the correct way to handle `setInterval` within `useEffect` to prevent memory leaks.

## How to reproduce

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the behavior of the component.  Unmounting the component will not stop the counter.