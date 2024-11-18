# Exercise: Using `useEffect` to perform set-up routines

Functional components can be called multiple times throughout the app's lifetime in order to update the view. This means that any set-up code placed at the top level of the function would be re-run every time time the component was re-rendered!

To solve this problem, we can use the `useEffect` hook, which lets us run set-up, teardown, and respond to changes in the state only when we need to.

Fix the `Timer` component below to make sure that the interval is created and destroyed exactly once for each component instance.

## Instructions

- Move the `setInterval` call into a `useEffect` callback.

- In the teardown callback for `useEffect`, clear the interval.

## Hint

- `useEffect` accepts a single argument -- a callback function to do any set-up work needed. We can move our timer set-up line into a `useEffect` callback.

- The `useEffect` callback can return another function to do any cleanup work. We can use this to clear the timer interval when the component is unmounted.

## Code before

Functional React component for a timer counting up in seconds. Current count initialised to 0 with a `useState` hook, followed by a bare `setInterval` call to increment the count every second. Since a new `setInterval` is created on every re-render, the count starts increasing by 2, then 3, etc after each re-render when it should just increase by 1.

## Solution

`setInterval` wrapped in `useEffect` callback, with `clearInterval` in the teardown function.
