## Reading: Application State with Redux


## What is REDUX?

- Redux is a predictable state container for JavaScript apps.

- It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test.

<br/>
<br/>

## REDUX CORE :

`npm install redux`
<br/>


> State management is absolutely critical in providing users with a well-crafted experience with minimal bugs. Redux provides a solid, stable, and mature solution to managing state in your React application. Through a handful of small, useful patterns, Redux can transform your application from a total mess of confusing and scattered state, into a delightfully organized, easy to understand modern JavaScript powerhouse.

<br/>
<br/>

> principles of Redux are packaged and presented for you in an easy to use a library that not only elevates your applications but also improves your general understanding of building JavaScript UIs.

<br/>
<br/>


## Testing redux reducers with Jest

- it starts with boilerplate setup and writing empty tests just to outline what needs to be tested. I like to to test the initial state and then every switch/case in the reducer to see if action.payload will produce expected store.

<br/>

```js
import reducer from './getPostsReducer';
import * as types from '../actions/posts/getPostsReduxAction';
import expect from 'expect';

describe('team reducer', () => {
  it('should return the initial state');
  it('should handle GET_POST_SUCCESS');
  it('should handle UPDATE_POST_SUCCESS');
  it('should handle GET_POST_FAIL');
  it('should handle GET_POST_START');
});
```
<br/>


## When to use Redux :
1. You have large amounts of application state that are needed in many places in the app.

2. The app state is updated frequently over time

3. The logic to update that state may be complex

4. The app has a medium or large-sized codebase, and might be worked on by many people.
<br/>
<br/>


## Principles of Redux (Redux Store):

- State Tree
- Action
- Reducer Function

<br/>
<br/>
<br/>

# Discussion:
## What are the advantages of storing tokens in “Cookies” vs “Local Storage”
- easier to retrive and edit.

- easier to clean or reset.

- cookies data will be sent over each request which is great to authentication and authorization.

<br/>


## Explain 3rd party cookies.
- Third-party cookies are cookies that are set by a website other than the one you are currently on. For example, you can have a "Like" button on your website which will store a cookie on a visitor's computer, that cookie can later be accessed by Facebook to identify visitors and see which websites they visited.

<br/>
<br/>

## How do pixel tags work?
- A tracking pixel (also called 1x1 pixel or pixel tag) is a graphic with dimensions of 1x1 pixels that is loaded when a user visits a webpage or opens an email. ... The tracking pixel URL is the memory location on the server. When the user visits a website, the image with the tag is loaded from this server.

<br/>
<br/>



# Term:
- cookies: small block of data saved in the browser.
<br/>

- authorization:is the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular.
<br/>


- access control: to give or deny the permission of accessing data/section/pages.

<br/>

- conditional rendering: Conditional rendering is a term to describe the ability to render different user interface (UI) markup if a condition is true or false.


<br/>
<br/>
<br/>


## How to use Redux in react (Links to an external site.)
1. create store as we create context

2. pass store and context to provider imported as context exactly.

<br/>
<br/>
<br/>

## How Redux works (Links to an external site.)
- “There is a central store that holds the entire state of the application. Each component can access the stored state without having to send down props from one component to another”.
<br/>


> “There are three building parts: actions, store, and reducers”.


<br/>
<br/>

<br/>
<br/>


<br/>
<br/>




## References: 

[Dan Abramov Redux Tutorials](https://egghead.io/courses/getting-started-with-redux)

[worlds easiest guide to redux](https://medium.freecodecamp.org/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6)

[testing reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)

[Redux Docs](https://redux.js.org/)