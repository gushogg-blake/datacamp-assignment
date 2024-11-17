# Exercise: Using `useEffect` to perform set-up routines

Functional components can be called multiple times throughout the app's lifetime in order to update the view. This means that any set-up code placed at the top level of the function would be re-run every time time the component was re-rendered!

To solve this problem, we can use the `useEffect` hook, which is designed for exactly this purpose: performing set-up (and teardown) routines just once for each instance of the component.

Fix the `Clock` component below to make sure that the interval is created and destroyed exactly once for each component instance.

## Instructions

- Move the `setInterval` call into a `useEffect` callback.

- In the teardown callback for `useEffect`, clear the interval.

## Hint

- `useEffect` accepts a single argument -- a callback function to do any set-up work needed. We can move our timer set-up line into a `useEffect` callback.

- The `useEffect` callback can return another function to do any cleanup work -- that's where we need to clear the timer interval.
