# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug showcases an infinite render loop caused by a missing dependency in the useEffect's dependency array. The solution demonstrates how to correctly add the dependency to resolve the issue.

## Bug Description

The initial code has an `useEffect` hook that runs after every render without specifying the dependency array correctly. This results in an infinite loop where the component continuously re-renders, causing performance issues and potential crashes. 

## Solution

The solution involves adding the `count` state variable to the dependency array of the `useEffect` hook. By doing this, the effect only runs when the `count` value changes, preventing the infinite loop.  This is crucial for efficient and predictable component behavior.
