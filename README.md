# React Counter Bug

This repository demonstrates a common bug in React applications involving the `useState` hook.  The `Counter` component fails to increment correctly due to an error in how the state update function is used.

## Bug Description

The provided `Counter` component uses `useState` to manage a counter. The `increment` function is supposed to add 1 to the counter's value. However, it incorrectly calls `setCount` with the existing value of `count`, preventing the counter from updating.

## Solution

The solution file (`bugSolution.js`) corrects this issue by properly updating the state. This is achieved by passing a function to `setCount`, which receives the previous state as an argument and returns the updated state.  This ensures React correctly updates the component's display.

## How to reproduce

1. Clone this repository.
2. Navigate to the repository's root directory.
3. Run `npm install`.
4. Run `npm start`.
5. Click the increment button; observe that the counter does not increment.

## How to fix

Review the solution provided in `bugSolution.js` to see how to properly update state using `useState`.