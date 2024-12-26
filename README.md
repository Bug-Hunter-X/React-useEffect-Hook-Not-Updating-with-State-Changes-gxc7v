# React useEffect Hook Not Updating with State Changes

This example demonstrates a common mistake when using the `useEffect` hook in React.  The `useEffect` hook is intended to perform side effects based on changes to specific values.  However, if the dependency array is empty (`[]`), the effect runs only once after the initial render, even if the component's state changes.

The provided `bug.js` file contains code that showcases this issue.  The `console.log` statement inside `useEffect` should update every time the `count` changes; but because the dependency array is empty it only runs once. The solution file (`bugSolution.js`) provides the correct implementation.