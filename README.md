# React useEffect Hook Runs Only Once

This repository demonstrates a common issue with the `useEffect` Hook in React. The `useEffect` Hook with an empty dependency array `[]` only runs once after the component mounts.  This example highlights how to use the `useEffect` hook correctly and how to avoid common pitfalls. 

## Bug

The provided code shows a `MyComponent` that uses a `useState` Hook for counting clicks and a `useEffect` Hook with an empty dependency array. The `useEffect`'s intent is to log a message when the component is mounted; however, the behavior is unexpected when expecting the effect to run more than once.

## Solution

The solution provides a revised `MyComponent` with the `useEffect` Hook correctly using the `count` state as a dependency. This ensures the effect runs whenever the `count` value changes.