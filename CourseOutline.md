# Course Outline: Introduction to React

## Prerequisites

Before starting this course, you should be comfortable creating web pages with HTML and adding interactive elements with JavaScript.

> Overall course objective: Get from simple HTML pages and ad-hoc event handlers & DOM manipulation, to understanding a more structured approach---knowing React syntax (JSX) and fundamental concepts (view as a function of state; encapsulation via components)---and appreciating the reasoning behind them.
> 
> By the end of the course we will be able to create a React project in which two or more components display & update some state via props, the `useState` hook, and event handlers, giving us a solid foundation from which to start building apps and learning the more advanced concepts.

## Chapter 1: JSX

> As the de facto standard for writing markup in React, we will be working with JSX throughout the course and it will be required to write our first component.
> 
> The basic building blocks of a React project are _components_, JavaScript functions that take some app state as input and produce some HTML as output. Components allow you to organise the different areas of your app into re-usable JavaScript modules, each with a clearly defined responsibility. For example, you might create components for a `Header`, `Article`, `Input`, or `Button` in your app.

### Lesson 1.1: Creating markup with JSX

> JSX allows us to write an HTML-like syntax to define the markup for our React components directly within JavaScript.

Learning objectives:

- Learner will be able to write a JavaScript function that returns JSX.

- Learner will be able to fix common JSX-vs-HTML errors like trying to return multiple elements unwrapped, not closing a self-closing tag, or using reserved word attributes (`class`, `for`).

Example exercise: fill in an empty function to return a `<div>` with some text inside it:

```javascript
function MyComponent() {
	return ; // complete the function
}
```

Solution:

```javascript
function MyComponent() {
	return <div>This is JSX.</div>;
}
```

### Lesson 1.2: JSX expressions

> JSX can contain JavaScript expressions to display dynamic data.

Learning objectives:

- Learner will be able to use `{...}` syntax to set JSX attributes and content based on JavaScript variables.

Example exercise: change an attribute (such as a `className` for theming) or text content, from a hard-coded value to a variable.

### Lesson 1.3: Conditional rendering

> Introduce conditionals via ternary expressions. Give examples of both "if" (`{cond ? something : null}`) and "if-else" (`{cond ? something : somethingElse}`).

Learning objectives:

- Learner will be able to write JSX that renders a different DOM structure depending on the value of a variable.

Example exercise: write JSX markup to display the logged-in user's name if present, or a login link if the user is `null`.

## Chapter 2: Components

> I was going to start with writing a simple functional component but this is already covered by writing a function that returns JSX, so this can be explained in the intro video for this chapter.

### Lesson 2.1: Nested components

Learning objectives:

- Learner will be able to create two React components in separate modules, import one from the other, and render the child within the parent's JSX.

- Learner will be able to choose an appropriate boundary for components based on separation of concerns and encapsulation principles.

Example exercise: refactor a component to split part of it out into a subcomponent.

### Lesson 2.2: Passing props

Learning objectives:

- Learner will be able to pass a prop from a parent component to a child component.

- Learner will be able to decide when to use a prop and when to store the data locally based on its scope.

Example exercise: convert a local variable to a prop.

### Lesson 2.3: Handling events

Learning objectives:

- Learner will be able to define an event handler function and attach it to a DOM element.

- Learner will be able to attach an event handler to a component as a prop.

- Learner will be able to explain why event handler references don't have the `()` after the function name.

Example exercise: add a click handler to a `Button` component.

## Chapter 3: Managing state

> So far we've used JavaScript variables to include dynamic content in our JSX. It's important to note that in React, though, changing the value of a variable after the initial render won't automatically trigger a re-render.
> 
> For this to work, we need to use React's _hooks_, in particular the `useState` hook.

### Lesson 2.1: The `useState` hook

Learning objectives:

- Learner will be able to use the `useState` hook to manage state within a functional React component.

- Learner will be able to explain why simply reassigning a variable doesn't automatically update the DOM.

Example exercise: fix a simple clock component to use `useState` instead of a direct variable assignment to get it to update every second.

### Lesson 2.2: Hook rules

Learning objectives:

- Learner will be able to explain what context hooks can be called in and why.

- Learner will be able to recognise where a hook would be out of context and factor the code out into a new component in order to make it work.

Example exercise: fix a broken component by moving hook usage out of a conditional or loop and into a new subcomponent.

### Lesson 2.3: Shared state

Learning objectives:

- Learner will be able to lift state up to share it between multiple components.



Example exercise: 

