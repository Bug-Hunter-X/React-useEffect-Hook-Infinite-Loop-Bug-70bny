# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook.  The bug causes an infinite loop due to a missing dependency in the `useEffect` dependency array.

## Bug Description

The `useEffect` hook is used to perform side effects, but if a value used within the effect changes during the effect's execution it leads to an infinite loop. The `bug.js` file demonstrates this issue, while `bugSolution.js` presents a corrected version.

## How to Reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
5. Observe the infinite loop in the browser's console and potentially a crashing application. 

## Solution

The solution involves correctly specifying the dependencies in the `useEffect` hook's dependency array (`[]`). The fixed code is in `bugSolution.js`.