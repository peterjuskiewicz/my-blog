---
title: Basic Functions of React
date: "2023-04-08T22:12:03.284Z"
description: "Exploring basic functions of React."
---

# Basic Functions of React

React is a popular JavaScript library that's used to build user interfaces. It was developed by Facebook and is now maintained by a large community of developers. If you're new to React, it can seem a bit daunting at first, but once you get the hang of it, you'll find that it's actually quite simple and intuitive. In this post, we'll take a look at some of the basic functions of React and how they work.

## Components

Components are the building blocks of React applications. A component is a self-contained unit of code that encapsulates functionality and can be reused throughout your application. Components can be thought of as small, independent parts of your user interface. For example, you might have a component that represents a button, a component that represents a form, and so on.

## JSX

JSX is a syntax extension for JavaScript that allows you to write HTML-like code in your JavaScript files. It's used to describe what your React components should look like. JSX is not required to use React, but it's a common way to write React code. Here's an example of what JSX looks like:

```jsx
const Hello = (props) => {
  return <h1>Hello, {props.name}!</h1>;
};
```

In this example, we're defining a component called "Hello" that takes in a "name" prop and displays a greeting.

## State

State is a way to store and update data in React components. It's used to keep track of things like user input, form data, and other dynamic information. When state changes, React re-renders the component to reflect the new state. Here's an example of how to use state:

```jsx
const Counter = () => {
  const [count, setCount] = useState(0);

  const handleClick = () => {
    setCount(count + 1);
  };

  return (
    <div>
      <p>You clicked the button {count} times.</p>
      <button onClick={handleClick}>Click me!</button>
    </div>
  );
};
```

In this example, we're defining a component called "Counter" that keeps track of a count using state. When the user clicks the button, the "handleClick" function is called, which updates the count and triggers a re-render.

## Props

Props are short for "properties" and are used to pass data from one component to another. Props are read-only and cannot be changed by the component that receives them. Here's an example of how to use props:

```jsx
const Greeting = (props) => {
  return <p>Hello, {props.name}!</p>;
};

const App = () => {
  return (
    <div>
      <Greeting name="Alice" />
      <Greeting name="Bob" />
    </div>
  );
};
```

In this example, we're defining a component called "Greeting" that takes in a "name" prop and displays a greeting. We're then using that component twice in the "App" component, passing in different names each time.

## Conclusion

These are just a few of the basic functions of React. There's a lot more to learn, but by understanding these concepts, you should be able to start building your own React applications. If you're new to React, I recommend checking out the official documentation, as well as some of the many tutorials and courses available online. Good luck!
