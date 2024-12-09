# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications involving the `useEffect` hook: creating an infinite loop by incorrectly specifying the dependency array.

## Description
The `MyComponent` component uses the `useEffect` hook to update the state variable `count` every time the component renders.  However, the dependency array `[]` is empty, causing the effect to run on every render, leading to an infinite loop.

## Solution
The solution involves correctly specifying the dependency array.  In this case, we want the effect to run only once after the initial render. Therefore, the dependency array should be empty `[]`.