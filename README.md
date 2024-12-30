# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug causes an infinite loop due to an improperly defined dependency array in `useEffect`.

## Bug Description
The `useEffect` hook in `MyComponent` is designed to log the current value of `count` to the console.  However, if the dependency array is missing or improperly specified, it will trigger on every render, leading to an infinite loop and likely crashing the application.

## Solution
The solution involves correctly defining the dependency array to ensure `useEffect` only runs when the value of `count` changes.