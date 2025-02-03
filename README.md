# React Native useState Hook Not Updating UI After Direct Object Mutation

This repository demonstrates a common issue in React Native: the failure of the `useState` hook to update the UI after a direct mutation of an object or array within the state.  The `bug.js` file showcases the problem, while `bugSolution.js` provides the correct solution.

**Problem:**
Directly modifying an object or array in state leads to unexpected behavior because React's shallow comparison doesn't detect the change. 

**Solution:**
Always create a new object or array using spread syntax or other methods to update the state. This ensures that React recognizes the change and updates the UI.