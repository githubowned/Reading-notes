# Read: Class 02 - Readings: State and Props

> - Remember:  React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.

<p>&nbsp;</p>

## State Vs. Life cycle
- The state object is where you store property values that belongs to the component. When the state object changes, the component re-renders.

- Every React Component has a lifecycle of its own, lifecycle of a component can be defined as the series of methods that are invoked in different stages of the component's existence.
<p>&nbsp;</p>

## How to convert a function to a class ?
- You can convert a function component into  a class in five steps:
1. Create an ES6 class, with the same name, that extends React.Component.
2. Add a single empty method to it called render().
3. Move the body of the function into the render() method.
4. Replace props with this.props in the render() body.
5. Delete the remaining empty function declaration.

<p>&nbsp;</p>

## How to add a Local State to a Class?
1. Replace this.props. with this.state. in the render() method.


2. Add a class constructor that assigns the initial this.state.
<p>&nbsp;</p>

>notes :
>1. Do Not Modify State Directly
>2. The only place where you can assign this.state is the constructor.

<p>&nbsp;</p>

- Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

1. React events are named using camelCase, rather than lowercase.
2. With JSX you pass a function as the event handler, rather than a string.
<p>&nbsp;</p>

For example, the HTML:

```
<button onClick={activateLasers}>
  Activate Lasers
</button>
```

>Note:  If you forget to bind this.handleClick and pass it to onClick, this will be undefined when the function is actually called.
<p>&nbsp;</p>

 -  ## Consider these code lines: 
---
<p>&nbsp;</p>

```js
function UserGreeting(props) {
  return <h1>Welcome back!</h1>;
}

function GuestGreeting(props) {
  return <h1>Please sign up.</h1>;
}
```


```js
function Greeting(props) {
  const isLoggedIn = props.isLoggedIn;
  if (isLoggedIn) {
    return <UserGreeting />;
  }
  return <GuestGreeting />;
}

ReactDOM.render(
  // Try changing to isLoggedIn={true}:
  <Greeting isLoggedIn={false} />,
  document.getElementById('root')
);
```
<p>&nbsp;</p>

> Conditional rendering in React works the same way conditions work in JavaScript.


<p>&nbsp;</p>
<p>&nbsp;</p>

## References:
---
1. [ React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html).
2. [ React Docs - handling events](https://reactjs.org/docs/handling-events.html)
3. [ React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)
4. [ React Tutorial through ‘Developer Tools’](https://reactjs.org/tutorial/tutorial.html)