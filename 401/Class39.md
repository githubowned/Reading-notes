# Readings: Redux - Additional Topics


### What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

- The most ‘redux-like’ way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.

<br/>
<br/>

### When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

- You export the actual action from the reducer.

<br/>
<br/>


# Terms :
## middleware: 
- Middleware is a type of computer software that provides services to software applications beyond those available from the operating system. It can be described as "software glue".
<br/>
<br/>

## thunk:
-  Redux Thunk is a middleware that allows you to call the action creators that return a function(thunk) which takes the store's dispatch method as the argument and which is afterwards used to dispatch the synchronous action after the API or side effects has been finished.
<br/>
<br/>

# Preparation Materials

The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

1. "Configuring a Redux store is too complicated"

2. "I have to add a lot of packages to get Redux to do anything useful"

3. "Redux requires too much boilerplate code"

<br/>
<br/>

##  Redux Toolkit is available as a package on NPM for use: 

<br/>

- `npm install @reduxjs/toolkit`


```js
import { createApi } from '@reduxjs/toolkit/query'

/* React-specific entry point that automatically generates
   hooks corresponding to the defined endpoints */
import { createApi } from '@reduxjs/toolkit/query/react'
```
<br/>
<br/>

## RTK Query

<br/>


- RTK Query is provided as an optional addon within the @reduxjs/toolkit package. It is purpose-built to solve the use case of data fetching and caching, supplying a compact, but powerful toolset to define an API interface layer for your app. 

<br/>

- It is intended to simplify common cases for loading data in a web application, eliminating the need to hand-write data fetching & caching logic yourself.

<br/>


- RTK Query is built on top of the Redux Toolkit core for its implementation, using Redux internally for its architecture.

<br/>

- Although knowledge of Redux and RTK are not required to use RTK Query, you should explore all of the additional global store management capabilities they provide, as well as installing the Redux DevTools browser extension, which works flawlessly with RTK Query to traverse and replay a timeline of your request & cache behavior.

<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>



# References:
1. [Redux Toolkit (RTK)](https://redux-toolkit.js.org/)

2. [Tutorial](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)