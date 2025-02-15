# Unnecessary Re-renders in React useEffect Hook
This repository demonstrates a common React bug involving the `useEffect` hook. The `useEffect` hook runs more often than needed, causing unnecessary re-renders and potentially performance issues.  The solution shows how to correctly specify dependencies to optimize the hook's behavior.

## Bug
The provided code shows a simple counter component. The `useEffect` hook is supposed to log the count to the console, but it logs on every render, including when no change happened. This is inefficient.

## Solution
The solution fixes the issue by including the 'count' variable as a dependency in the useEffect hook. This ensures the effect only runs when the 'count' actually changes.