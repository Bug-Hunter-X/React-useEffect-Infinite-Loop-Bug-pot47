# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by a missing dependency in the dependency array. 

The `bug.js` file shows the erroneous code, while `bugSolution.js` provides the corrected version.

## Problem

The `useEffect` hook, without the correct dependencies listed in the array, will run after every render. This will usually lead to an infinte loop and crash the application. 

## Solution

The solution involves adding the `count` state variable to the dependency array. This ensures that the effect only runs when the `count` variable changes.