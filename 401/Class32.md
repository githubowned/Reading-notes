# Read: Class 32

# Reading: Context API - Behaviors

## When to Use Context ?
- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

> If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.


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

## Review, Research, and Discussion

###  When you have multiple contexts, what component type should you use (class/function) and why?


- The static contextType property won't work if you need more than one, so instead you need to use a context consumer.
<br/>
<br/>


###  How can you best test context?
- The best way to test Context is to make our tests unaware of its existence and avoiding mocks. We want to test our components in the same way that developers would use them (behavioral testing) and mimic the way they would run in our applications (integration testing).
<br/>
<br/>
<br/>
<br/>

## Terms: 
- context : ontext is related to objects. It refers to the object to which a function belongs. When you use the JavaScript “this” keyword, it refers to the object to which function belongs.
<br/>
<br/>

- useContext() : “useContext” hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level.
<br/>
<br/>


- static context : Static context defines items that are needed to prepare executables, items such as the names and types of external variables and functions that will be available at run time as well as compilation modes like backwards compatibility, math mode, and so on. 


<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

# References:

- [context api](https://reactjs.org/docs/context.html)

- [hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)

- [react context links](https://github.com/diegohaz/awesome-react-context)