# React useEffect Hook Missing Dependency Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug arises from omitting a necessary dependency from the dependency array, leading to unexpected re-renders and potentially incorrect behavior.

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides the corrected version.

## Bug Description
The `useEffect` hook in `bug.js` is missing `count` from its dependency array. This means the effect will not run correctly every time the `count` state variable changes. It only runs after the initial render. 

## Solution
The solution in `bugSolution.js` adds `count` to the dependency array. Now the effect runs whenever the `count` value changes, ensuring correct behavior.