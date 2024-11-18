# Course Outline: Introduction to React

## Prerequisites

Before starting this course, you should be comfortable creating web pages with HTML, CSS and JavaScript.

## Chapter 1: JSX

### Lesson 1.1: Creating markup with JSX

Learning objectives:

- Learner will be able to write a JavaScript function that returns JSX.

- Learner will be able to fix common JSX-vs-HTML errors like trying to return multiple elements unwrapped, not closing a self-closing tag, or using reserved word attributes (`class`, `for`).

Example exercise: update this function to return a `<div>` with some text inside it.

### Lesson 1.2: JSX expressions

Learning objectives:

- Learner will be able to use `{...}` syntax to set JSX attributes and content based on JavaScript variables.

Example exercise: change an attribute (such as a `className` for theming) or text content, from a hard-coded value to a variable.

### Lesson 1.3: Conditional rendering

Learning objectives:

- Learner will be able to write JSX that renders a different DOM structure depending on the value of a variable.

Example exercise: write JSX markup to display the logged-in user's name if present, or a login link if the user is `null`.

## Chapter 2: Components

### Lesson 2.1: Using components

Learning objectives:

- Learner will be able to create two React components in separate modules, import one from the other, and render the child within the parent's JSX.

- Learner will be able to choose an appropriate boundary for components based on separation of concerns and encapsulation principles.

Example exercise: refactor a component to split part of it out into a subcomponent.

### Lesson 2.2: Passing props

Learning objectives:

- Learner will be able to pass a prop from a parent component to a child component.

- Learner will be able to decide when to use a prop and when to store the data locally based on its scope.

Example exercise: convert a local variable to a prop.

### Lesson 2.3: Styling

Learning objectives:

- Learner will be able to apply styles inline in JSX.

- Learner will be able to create and import a CSS file into a React component.

- Learner will be able to choose an appropriate method of including CSS where dynamic styling is required, e.g. theming.

Example exercise: apply a drop shadow to all buttons in this component.

### Lesson 2.4: Handling events

Learning objectives:

- Learner will be able to define an event handler function and attach it to a DOM element.

- Learner will be able to attach an event handler to a component as a prop.

- Learner will be able to explain why event handler references don't have the `()` after the function name.

Example exercise: add a click handler to a `Button` component.

## Chapter 3: Updating State

### Lesson 3.1: The `useState` hook

Learning objectives:

- Learner will be able to use the `useState` hook to manage state within a functional React component.

- Learner will be able to explain why simply reassigning a variable doesn't automatically update the DOM.

Example exercise: fix a click counter to use `useState` instead of direct variable assignment.

### Lesson 3.2: The `useEffect` hook

Learning objectives:

- Learner will be able to use the `useEffect` hook to perform actions on component mount.

- Learner will be able to identify variables for the dependency array, if any.

- Learner will be able to identify and explain what needs to go in the clean-up function, if anything.

- Learner will be able to explain why `useEffect` is needed to coordinate side effects in a functional model (because the component function itself can be called at any time to re-render).

Example exercise: fix a simple `Timer` component to use `useEffect` and `useState` to set up an update interval.

### Lesson 3.3: Hook rules

Learning objectives:

- Learner will be able to explain what context hooks must be called in and why.

- Learner will be able to recognise where a hook would be out of context and factor the code out into a new component in order to make it work.

Example exercise: what is wrong with the following code and how should it be fixed? E.g. "hook is used after `if` statement, move to separate component".

### Lesson 3.4: Input binding

Learning objectives:

- Learner will be able to get the value from a text field and store it in a state variable using an event handler.

- Learner will be able to state an advantage and a disadvantage of one-way data binding (e.g., easy to reason about but more verbose)

Example exercise: display a word count next to a text field.

## Chapter 4: Modeling Data

### Lesson 4.1: Working with collections

Learning objectives:

- Learner will be able to render items in an array using `map`.

Example exercise: given an array of items such as blog posts, display each item in a list using a subcomponent.

### Lesson 4.2: Keys

Learning objectives:

- Learner will be able to explain why keys are needed when dealing with mutable arrays (e.g., "to let React know which DOM node to associate with which object from the array").

- Learner will be able to choose a suitable key and explain why (unique, stable).

Example exercise: add a key to the blog posts list. (Note: previous lesson will have given a warning about it so it should be mentioned there.)

### Lesson 4.3: Shared state

Learning objectives:

- Learner will be able to lift state up to share it between multiple components.

- Learner will be able to state an advantage and a disadvantage of prop-drilling (e.g., simple but repetitious) and when it might be more appropriate to use a solution like contexts.

Example exercise: refactor prop-drilling to use `useContext`.
