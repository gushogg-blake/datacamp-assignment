# Exercise: Re-rendering on updates

So far we've used JavaScript variables to include dynamic content in our JSX. But if we change the value of these variables after the initial render, React won't know to update the associated DOM elements.

For this to work, we need to use the `useState` hook.

Fix the `Clock` component so that the time display updates every second.

## Instructions

- Use `useState` to make the `now` variable reactive.

## Hint


