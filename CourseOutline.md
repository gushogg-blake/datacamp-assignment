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

### Lesson 1.1: HTML in JavaScript

> JSX allows us to write an HTML-like syntax to define the markup for our React components directly within JavaScript.

Learning objectives:

- Learner will be able to write a JavaScript function that returns JSX.

- Learner will be able to fix common JSX-vs-HTML errors like trying to return multiple elements unwrapped, not closing a self-closing tag, or using reserved word attributes (`class`, `for`).

Example exercise: fill in an empty function to return a `<div>` with some text inside it:

```javascript
function MyComponent() {
	// complete the function
}
```

Solution:

```javascript
function MyComponent() {
	return <div>This is JSX.</div>;
}
```

### Lesson 1.2: Expressions

> JSX can contain JavaScript expressions to display dynamic data.

Learning objectives:

- Learner will be able to use `{...}` syntax to set JSX attributes and content based on JavaScript variables.

Example exercise: change an attribute (such as a `className` for theming) or text content, from a hard-coded value to a variable.

### Lesson 1.3: Conditionals

> Introduce conditionals via ternary expressions. Give examples of both "if" (`{cond ? something : null}`) and "if-else" (`{cond ? something : somethingElse}`).

Learning objectives:

- Learner will be able to write JSX that renders a different markup structure depending on the value of a variable.

Example exercise: write a React component that displays the logged in user's name if present, or a login link otherwise.

## Chapter 2: Updating the View

> So far we've used JavaScript variables to include dynamic content in our JSX. It's important to note that in React, though, changing the value of a variable after the initial render won't automatically trigger a re-render.
> 
> For this to work, we need to use React's _hooks_, in particular the `useState` hook.

### Lesson 2.1: The `useState` Hook

Learning objectives:

- Learner will be able to use the `useState` hook to initialise and update a piece of dynamic state within a functional React component.

Example exercise: fix a simple clock component to use `useState` instead of a direct variable assignment to get it to update every second.



## Chapter 3: Components & Props



## Chapter 4: Handling Events

Tie everything together with an interactive example
