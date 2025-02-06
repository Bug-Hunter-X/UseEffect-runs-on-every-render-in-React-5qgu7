# React useEffect Runs on Every Render

This repository demonstrates a common React bug where the `useEffect` hook runs on every render instead of only when its dependencies change.  The solution shows how to correctly specify dependencies to fix the issue.

## Bug
The original `MyComponent` function uses `useEffect` without specifying the correct dependencies. This leads to an unnecessary re-render and repeated console logging with every state update. 

## Solution
The solution demonstrates how to correctly specify the `count` as a dependency in `useEffect`.  This ensures that the effect only runs when the `count` variable changes.