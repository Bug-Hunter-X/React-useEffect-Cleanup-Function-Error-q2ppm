# React useEffect Cleanup Function Error

This repository demonstrates a common error in React's `useEffect` hook: forgetting to include a cleanup function to remove event listeners or other side effects when the component unmounts.  Failure to do so can lead to memory leaks and unexpected behavior.

## Problem

The `bug.js` file shows a component that adds an event listener in `useEffect` without a cleanup function. This listener remains active even after the component is unmounted, potentially causing issues.

## Solution

The `bugSolution.js` file demonstrates the correct implementation.  A cleanup function is returned from `useEffect`, which removes the event listener when the component unmounts. This prevents memory leaks and ensures proper behavior.