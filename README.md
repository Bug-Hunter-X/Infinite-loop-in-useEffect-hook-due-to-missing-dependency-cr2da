# React useEffect Hook Bug

This repository demonstrates a common bug in React's `useEffect` hook: an infinite loop caused by a missing dependency in the dependency array.

## Bug Description

The `useEffect` hook in `bug.js` attempts to log the current count on every render. However, the dependency array `[count]` is missing, which means React re-runs the effect on every render, causing an infinite loop and crashing the application.

## Solution

The solution is provided in `bugSolution.js`, where the dependency array is correctly updated to include the `count` variable.