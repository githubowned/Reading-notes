# Readings: Redux - Asynchronous Actions


## How granular should your reducers be?
- It depends on the implementation but generally the more granular the better.

<br/>
<br/>

## Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
- Well, it is a Pro more than a Con since we have to change multiple states in multiple components, the fact that all the reducers can listen when the action is dispatched can reduce a lot of work, each reducer can provide a different logic to the same dispatcher.

<br/>
<br/>

## Name a strategy for preventing the above
- Using Redux middleware thunk, allows for evaluating the actions.

<br/>
<br/>

# Define the folowing terms: 
###  store :
-  The Redux store brings together the state, actions, and reducers that make up your app. The store has several responsibilities:

  - Holds the current application state inside
  - Allows access to the current state via store.getState();
  - Allows state to be updated via store.dispatch(action);
  - Registers listener callbacks via store.subscribe(listener);
  - Handles unregistering of listeners via the unsubscribe function returned by store.subscribe(listener).

<br/>
<br/>

### combineReducers: 
- The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore . The resulting reducer calls every child reducer, and gathers their results into a single state object.

<br/>
<br/>

## Redux Thunk 
-  Redux reducers must never contain "side effects". 

<br/>
<br/>

- A "side effect" is any change to state or behavior that can be seen outside of returning a value from a function. 

<br/>
<br/>

### Some common kinds of side effects are things like:

- Logging a value to the console

- Saving a file

- Setting an async timer

- Making an AJAX HTTP request

<br/>

- Modifying some state that exists outside of a function, or mutating arguments to a function
Generating random numbers or unique random IDs (such as Math.random() or Date.now())

<br/>
<br/>



> Redux middleware were designed to enable writing logic that has side effects.

<br/>
<br/>



## Writing an Async Function Middleware

```js
const asyncFunctionMiddleware = storeAPI => next => action => {
  // If the "action" is actually a function instead...
  if (typeof action === 'function') {
    // then call the function and pass `dispatch` and `getState` as arguments
    return action(storeAPI.dispatch, storeAPI.getState)
  }

  // Otherwise, it's a normal action - send it onwards
  return next(action)
}
```
<br/>
<br/>

## Use middleWare like this :

```js
const store = createStore(rootReducer, middlewareEnhancer)

// Write a function that has `dispatch` and `getState` as arguments
const fetchSomeData = (dispatch, getState) => {
  // Make an async HTTP request
  client.get('todos').then(todos => {
    // Dispatch an action with the todos we received
    dispatch({ type: 'todos/todosLoaded', payload: todos })
    // Check the updated store state after dispatching
    const allTodos = getState().todos
    console.log('Number of todos after loading: ', allTodos.length)
  })
}

// Pass the _function_ we wrote to `dispatch`
store.dispatch(fetchSomeData)
// logs: 'Number of todos after loading: ###'
```

<br/>
<br/>

> Redux already has an official version of that "async function middleware", called the Redux "Thunk" middleware. The thunk middleware allows us to write functions that get dispatch and getState as arguments. The thunk functions can have any async logic we want inside, and that logic can dispatch actions and read the store state as needed.

<br/>
<br/>


# Configuring the Store

`npm install redux-thunk`

`npm install redux-thunk@2.3.0`

```js
import { createStore, applyMiddleware } from 'redux'
import thunkMiddleware from 'redux-thunk'
import { composeWithDevTools } from 'redux-devtools-extension'
import rootReducer from './reducer'

const composedEnhancer = composeWithDevTools(applyMiddleware(thunkMiddleware))

// The store now has the ability to accept thunk functions in `dispatch`
const store = createStore(rootReducer, composedEnhancer)
export default store
```
<br/>
<br/>
<br/>
<br/>


<br/>
<br/>


































# Preparation Materials References: 
- [async actions](https://redux.js.org/advanced/asyncactions)

- [thunk middleware](https://github.com/reduxjs/redux-thunk)

- [redux thunk](https://alligator.io/redux/redux-thunk/)



