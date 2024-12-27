# React useEffect Cleanup Function Inconsistency

This repository demonstrates a bug related to the cleanup function in React's `useEffect` hook. The cleanup function is not consistently called, potentially causing memory leaks or other unexpected behavior.  The `bug.js` file contains the problematic code and `bugSolution.js` provides the corrected version.

## Bug Description
The `useEffect` hook's cleanup function should be executed before each subsequent render.  However, in the provided example, this isn't always the case, leading to inconsistent logging of the 'Cleanup!' message.  This inconsistency is a subtle bug, particularly in applications with frequent component updates.