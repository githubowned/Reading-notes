# Reading: `<Login />` and `<Auth />`

## Preparation material:

## WHAT IS  ROLE-BASED ACCESS CONTROL (RBAC)?
- Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.
<br/>
<br/>
<br/>

## react-cookies

- Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them. To set or remove the cookies, we are going to use a third-party dependency of react-cookie.
<br/>
<br/>

- React-cookie provides a component that you wrap around your root component. This sets a cookies object, and allows us to start using cookies anywhere within this component. ... Import the component with import { CookiesProvider } from 'react-cookie'; . App.js. Now, within App.
<br/>
<br/>
<br/>

## RBAC implementation:

- Define the resources that you need to limit access to.

- Define what roles you need for which resources.

- Assign people to those roles.

- Be careful when changing roles or adding new ones.

- Audit your system.
<br/>
<br/>
<br/>

 ``` js
 npm install react-cookies --save
 ```
<br/>
<br/>

- universal-cookie - Universal cookies for JavaScript.
- universal-cookie-express - Hook cookies get/set on Express for server-rendering.
<br/>

<br/>


Example : 

``` js
// Root.jsx
import React from 'react';
import App from './App';
import { CookiesProvider } from 'react-cookie';

export default function Root() {
  return (
    <CookiesProvider>
      <App />
    </CookiesProvider>
  );
}
```
<br/>
<br/>

```js
// App.jsx
import React from 'react';
import { useCookies } from 'react-cookie';

import NameForm from './NameForm';

function App() {
  const [cookies, setCookie] = useCookies(['name']);

  function onChange(newName) {
    setCookie('name', newName, { path: '/' });
  }

  return (
    <div>
      <NameForm name={cookies.name} onChange={onChange} />
      {cookies.name && <h1>Hello {cookies.name}!</h1>}
    </div>
  );
}

export default App;
```


<br/>
<br/>
<br/>
<br/>


# Review: 

## Why is the Context API useful?
- Because it can change important values for many components at once from a centralized location, without all of the values having to be passed through many layers of props.
<br/>
<br/>

## Can a component outside of a provider get its context?
- To access a React context outside of the render function, we can use the useContext hook. We create the UserContext by calling the React. createContext method with a default context value. Then in the Users component, we call the useContext hook with UserContext to accxess the current value of UserContext .
<br/>
<br/>

## What are some common use cases for using the Context API?
- Some sample use cases where the Context API proves helpful are: Theming — Pass down app theme. i18n — Pass down translation messages. Authentication — Pass down current authenticated user.
<br/>
<br/>

## Describe “Context Hell”
- Like the callback hell, usual when jQuery was used for everything, the React Context hell is the nasty code you get taking advantage of the React Context API.

<br/>
<br/>
<br/>
<br/>


# Terms: 

- global state:	a set of local states which are all concurrent with each other. … A global state in the time domain is also a global state in the causal domain.
<br/>
<br/>

- global context: This is context that affects the entire application, and it will share data to everything in the React component tree.
<br/>
<br/>

- provider: 	The context provider accepts a value that will be passed to its children. All children components will re-render when the value changes.
<br/>
<br/>

- consumer: This is a React component that subscribes to context changes in value of the Provider.



<br/>
<br/>
<br/>
<br/>
<br/>
<br/>


# References: 

[what is role based access control?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)

[react-cookies component](https://www.npmjs.com/package/react-cookies)

[react-cookie library](https://www.npmjs.com/package/react-cookie)
