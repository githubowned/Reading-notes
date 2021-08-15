# Reading: Context API


## what is Context API?
- Context provides a way to pass data through the component tree without having to pass props down manually at every level.

<br/>

## When to Use Context?
- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

<br/>
<br/>


## API
## React.createContext

`const MyContext = React.createContext(defaultValue);`
<br/>

- It Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.
<br/>
<br/>


## Context.Provider

`<MyContext.Provider value={/* some value */}>`
<br/>

- Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes.
<br/>
<br/>
<br/>


# Example:

```js
export const SnackBarContext = createContext()

export function SnackBarProvider({ children }) {
  const [alerts, setAlerts] = useState([])

  return (
    <SnackBarContext.Provider value={{ setAlerts }}>
      {children}
      {alerts.map((alert) => <SnackBar key={alert}>{alert}</SnackBar>)}
    </SnackBarContext.Provider>
  )
}
```
<br/>
<br/>


```js
import { useContext } from 'react'

import { SnackBarContext } from 'components/snack-bar-provider'

const useSnackBars = () => useContext(SnackBarContext)

export default useSnackBars
```

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>


# Review:

## Describe use cases useState() vs useReducer()

- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

<br/>

## Why do custom hooks need the use prefix?
- Custom hooks are normal JS functions, named with the prefix 'use', that can use hooks inside of it and contain a common stateful logic to be reused in other components.
<br/>

## What do custom hooks usually do?
- Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.
<br/>


## Describe how a hook that fetches API data might work
- The hook might take in a url, a method, and a body. Using axios or something similar, useState and possibly useEffect, an API call can be made based on and using the parameters passed in and then an objects state could be ‘set’ based on the results of the API call.
<br/>
<br/>


# Define :

- reducer: useReducer is one of the additional Hooks , An alternative to the useState Hook, it helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux or MobX .useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.

<br/>
<br/>

# Revision

Which 3 things had you heard about previously and now have better clarity on?
- hooks.

Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- useContext.

What are you most excited about trying to implement or see how it works?
- more hooks.

<br/>
<br/>
<br/>
<br/>


# References:

- [context api.](https://reactjs.org/docs/context.html)

- [hooks and context example.](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)

- [ react context links.](https://github.com/diegohaz/awesome-react-context)