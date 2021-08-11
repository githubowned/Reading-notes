# Reading: Advanced State with Reducers

```js 
const [state, dispatch] = useReducer(reducer, initialArg, init);
```

<br/>

- An alternative to `useState`. Accepts a reducer of type `(state, action) => newState`, and returns the current state paired with a `dispatch` method.
<br/>


- `useReducer` is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.
<br/>
<br/>
<br/>

## How does useReducer work?
 - `useReducer` is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.
<br/>
<br/>
<br/>

## Code example : 

```js
const initialState = {count: 0};

function reducer(state, action) {
  switch (action.type) {
    case 'increment':
      return {count: state.count + 1};
    case 'decrement':
      return {count: state.count - 1};
    default:
      throw new Error();
  }
}

function Counter() {
  const [state, dispatch] = useReducer(reducer, initialState);
  return (
    <>
      Count: {state.count}
      <button onClick={() => dispatch({type: 'decrement'})}>-</button>
      <button onClick={() => dispatch({type: 'increment'})}>+</button>
    </>
  );
}
```

<br/>
<br/>
<br/>

## Specifying the initial state:

- The simplest way is to pass the initial state as a second argument:


```js
const memoizedCallback = useCallback(
  () => {
    doSomething(a, b);
  },
  [a, b],
);
```

<br/>
<br/>
<br/>

# Review: 

## How can we ensure that an effect hook runs only once?

- Add a second parameter to the effect hook; Example
```js
function App() {

  useEffect(() => {
  // Run! Like go get some data from an API.
}, []);
}
```
<br/>
<br/>
<br/>


## Can useState() update more than one state variable at the same time?
- we could do one setState call and there will only be one render. Unlike the setState in class components, the setState returned from useState doesn’t merge objects with the existing state, it replaces the object entirely.

<br/>
<br/>



## Is useState() synchronous?

- useState and setState both are asynchronous.Even though they are asynchronous, the useState and setState functions do not return promises.Therefore we cannot attach a then handler to it or use async/await to get the updated state values.

<br/>
<br/>
<br/>
<br/>



# Definitions:

- State Hook: The state is an instance of React Component can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component.
<br/>

- Component Lifecycle: Every React Component has a lifecycle of its own, lifecycle of a component can be defined as the series of methods that are invoked in different stages of the component's existence. Mounting: Mounting is the stage of rendering the JSX returned by the render method itself.

<br/>
<br/>


# preview:

- Which 3 things had you heard about previously and now have better clarity on? Hooks.

- Which 3 things are you hoping to learn more about in the upcoming lecture/demo? the reducer.

- What are you most excited about trying to implement or see how it works? a full functional app with hooks.

<br/>
<br/>
<br/>

# References:
- [useReducer hook](https://reactjs.org/docs/hooks-reference.html#usereducer)

- [Ultimate Guide to useReducer](https://blog.logrocket.com/guide-to-react-usereducer-hook/)