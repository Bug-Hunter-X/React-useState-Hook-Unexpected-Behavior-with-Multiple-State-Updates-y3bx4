# React useState Hook Unexpected Behavior

This repository demonstrates a subtle bug related to how React's `useState` hook handles multiple state updates within a single render cycle. The issue arises when calling `setCount` multiple times in quick succession, potentially leading to unexpected state values.

## The Problem

The `bug.js` file contains a component that increments a counter using the `useState` hook.  However, calling `setCount` twice within the `handleClick` function can cause the counter to increment inconsistently.

## The Solution

The `bugSolution.js` file provides a solution to fix this problem by using a functional update method within the `useState` hook. This ensures that the update is based on the current state value, avoiding the issues caused by multiple sequential updates.

## How to Run

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.