SLIDE: intro

As we saw in the previous lesson, hooks allow us to control React's behaviour from inside of functional components.

SLIDE: recap of useState code

The useState hook returns two values -- the state variable,

ADD: underline state variable

and a callback to update the state.

ADD: underline the callback

When we call the callback,

ADD: underline the call

React knows that we need to re-render the component and update the view

ADD: reload icon

SLIDE: [image]

In this lesson, we'll see how the useEffect hook can be used to run set-up and teardown code when a component is mounted and unmounted.

SLIDE: setInterval to do a timer

To set up a recurring timer in JavaScript, we can use the `setInterval` function.

If we were to put this code in a functional component, however, it would be called every time React re-rendered the component, and we might end up with multiple timers running simultaneously for the same component instance.

ADD: repeating arrow to code

SLIDE: useEffect code

To solve this problem, React provides the useEffect hook,

ADD: underline useEffect

which allows us to run a callback function only once when a component is mounted,

ADD: underline and optionally, another callback function when the component is unmounted.
