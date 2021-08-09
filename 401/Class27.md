# Reading: `useState()` Hook


# What is a Hook?
 A Hook is a special function that lets you “hook into” React features. For example, `useState` is a Hook that lets you add React state to function components. We’ll learn other Hooks later.
<br/>
<br/>



# What does useState return? It returns a pair of values:
-  the current state and a function that updates it. This is why we write const `[count, setCount] = useState()`.
<br/>
<br/>
<br/>



> The Effect Hook, `useEffect`, adds the ability to perform side effects from a function component. It serves the same purpose as ***componentDidMount, componentDidUpdate, and componentWillUnmount*** in React classes, but unified into a single API. 

<br/>
<br/>
<br/>
<br/>



## Rules of Hooks:
 
  1. Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.

  2. Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions.
  <br/>
<br/>


# some less common hooks:

 - `useContext` lets you subscribe to React context without introducing nesting.

```js
function Example() {
  const locale = useContext(LocaleContext);
  const theme = useContext(ThemeContext);
  // ...
}
```

- `useReducer` lets you manage local state of complex components with a reducer.

```js
function Todos() {
  const [todos, dispatch] = useReducer(todosReducer);
  // 
  ...}
  ```

  <br/>
<br/>


## review :
1. How does React differ from vanilla JS/HTML/CSS?
-  React breaks down the UI into smaller and reusable components that can move around data amongst each other. This breaking down of the UI is what gives React an edge over Vanilla JS.

<br/>
<br/>


2. What is the primary difference between a function component and a class component?

- A functional component is just a plain JavaScript function that accepts props as an argument and returns a React element. A class component requires you to extend from React. Component and create a render function which returns a React element. There is no render method used in functional components.
<br/>
<br/>


# Definitions:

- Functional Components: Functional components are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword. Sometimes referred to as “dumb” or “stateless” components as they simply accept data and display them in some form; that is they are mainly responsible for rendering UI.
<br/>
<br/>


- Children / Child Components: A child component is a more specific part inside a parent component. Example would be a parent component being a PERSON. ARMS and LEGS are child components of it.

<br/>
<br/>


# Review

### Which 3 things had you heard about previously and now have better clarity on?
- Hooks
<br/>


### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- useState hook
<br/>


### What are you most excited about trying to implement or see how it works?
- the hooks manipulation.
<br/>


<br/>
<br/>
<br/>
<br/>


# References:

1. [making sense of hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

2. [the state hook](https://reactjs.org/docs/hooks-state.html)

3. [hooks api](https://reactjs.org/docs/hooks-overview.html)

4. [hooks api reference](https://reactjs.org/docs/hooks-reference.html)