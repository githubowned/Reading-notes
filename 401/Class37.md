# Readings: Redux - Combined Reducers



Why choose Redux instead of the Context API for global state?
- Context API is great for small applications where state changes are minimal but Redux is better for large applications where there are many changes to state. Redux also offer time-travel and single source of truth for state.

-To manage huge applications with complex state management, in a large scale application, Redux is a better way to control state.

- In a large scale application, Redux is a better way to control state.


What is the purpose of a reducer?
- We need reducers to tell the application how to change state in response to an action. The action does not do anything except describe what happened and it is up to the reducer to respond to this.

What does an action contain?
- An action contains a type and whatever payload you want it to have. There is flexibility in what there is besides the type. (Its an object basically).

Why do we need to copy the state in a reducer?
- The reducer needs to be a pure function without any side-effects. It should only take in an action and return the new state, but it should not mutate the state, so we need to copy it to update it.


## Terms:

- immutable state: is a state that cannot be modified, reducers must make copies of existing state to make updates.

- time travel in redux:s the ability to move back and forth among the previous states of an application and view the results in real time. With Redux, given a specific state and a specific action, the next state of the application is always exactly the same.

- action creator: is merely a function that returns an action object.

- reducer: A reducer is a function that determines changes to an application’s state. It uses the action it receives to determine this change.

- dispatch: The only way to update the state is to call store.dispatch() and pass in an action object.


 ## Combined Reducers :

 - Reducers are a great concept in Redux, because they allow your react application to have specific pieces of data that all update synchronously. 
 
 - All reducers run against your Redux store, and then the store triggers a change event and your entire React.js application re-renders.

- The most common state shape for a Redux app is a plain Javascript object containing “slices” of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have “slice reducer” functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. 

- Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

- There are two ways to define the initial shape and contents of your store’s state. First, the createStore function can take preloadedState as its second argument. This is primarily intended for initializing the store with state that was previously persisted elsewhere, such as the browser’s localStorage. 

- The other way is for the root reducer to return the initial state value when the state argument is undefined. These two approaches are described in more detail in Initializing State, but there are some additional concerns to be aware of when using combineReducers.

- combineReducers takes an object full of slice reducer functions, and creates a function that outputs a corresponding state object with the same keys. This means that if no preloaded state is provided to createStore, the naming of the keys in the input slice reducer object will define the naming of the keys in the output state object. 

- The correlation between these names is not always apparent, especially when using ES6 features such as default module exports and object literal shorthands.

 - Any reducer passed to combineReducers must satisfy these rules:

1. For any action that is not recognized, it must return the state given to it as the first argument.

2. It must never return undefined. It is too easy to do this by mistake via an early return statement, so combineReducers throws if you do that instead of letting the error manifest itself somewhere else.

3. If the state given to it is undefined, it must return the initial state for this specific reducer. According to the previous rule, the initial state must not be undefined either. It is handy to specify it with ES6 optional arguments syntax, but you can also explicitly check the first argument for being undefined.



## Example

reducers/todos.js#
```js
export default function todos(state = [], action) {
  switch (action.type) {
    case 'ADD_TODO':
      return state.concat([action.text])
    default:
      return state
  }
}
```

reducers/counter.js#

```js
export default function counter(state = 0, action) {
  switch (action.type) {
    case 'INCREMENT':
      return state + 1
    case 'DECREMENT':
      return state - 1
    default:
      return state
  }
}
```
reducers/index.js#

```js
import { combineReducers } from 'redux'
import todos from './todos'
import counter from './counter'

export default combineReducers({
  todos,
  counter
})
```
<br/>

## App.js
```js
import { createStore } from 'redux'
import reducer from './reducers/index'

const store = createStore(reducer)
console.log(store.getState())
// {
//   counter: 0,
//   todos: []
// }

store.dispatch({
  type: 'ADD_TODO',
  text: 'Use Redux'
})
console.log(store.getState())
// {
//   counter: 0,
//   todos: [ 'Use Redux' ]
// }
```


## References:
- [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

- [Redux Docs: Using Combined Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)

- [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)
