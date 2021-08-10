# Reading: Component Lifecycle / useEffect()

<br/>

> The Effect Hook lets you perform side effects in function components
<br/>
<br/>

<br/>


```js
import React, { useState, useEffect } from 'react';

function Example() {
  const [count, setCount] = useState(0);

  // Similar to componentDidMount and componentDidUpdate:
  useEffect(() => {
    // Update the document title using the browser API
    document.title = `You clicked ${count} times`;
  });

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```
<br/>
<br/>


## What does useEffect do? 
- It tells React that your component needs to do something after render.
<br/>

> so it will be called  later after performing the DOM updates.

<br/>
<br/>


## Why is useEffect called inside a component?
- Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect.

<br/>
<br/>

## Does useEffect run after every render?
- Yes! By default, it runs both after the first render and after every update. 

<br/>
<br/>
<br/>

# review:

1. Why do we not need more .html pages in a multi-page React app?
- React apps are single page app ,A React app consists of a single HTML file index.html. The views are coded in JSX format as components.
<br/>


2. If we wanted a component to show up on every page, where would we put it and why?
Outside the <BrowserRouter/>
Inside the <BrowserRouter />, outside a <Route />
Inside a <Route />

- Inside the <BrowserRouter />, outside a <Route /> ,no matter what the current route is .
<br/>


3. What does routing do with the components that were rendered when a new route is requested
- it goes to the new componetnt and remove the old one clean ups. 
<br/>



4. What does props.children contain?
- props. children represent the content between the opening and the closing tags when invoking/rendering a component and can have one element, multiple elements, or none at all, its value is respectively a single child node, an array of child nodes, or undefined.
<br/>


5. How do useState() and this.setState() differ?

- setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won’t touch the rest. 

- The useState’s updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging.
<br/>
<br/>
<br/>
<br/>


# Dfinitions: 

- **State Hook**: A Hook is a special function that lets you “hook into” React features. For example, useState is a Hook that lets you add React state to function components.
<br/>
<br/>



- **Mounting and Un-Mounting**: The main job of React is to figure out how to modify the DOM to match what the components want to be rendered on the screen. React does so by "mounting" (adding nodes to the DOM), "unmounting" (removing them from the DOM), and "updating" (making changes to nodes already in the DOM).

<br/>
<br/>



# Discussion
 Which 3 things had you heard about previously and now have better clarity on?
- Hooks.
<br/>


 Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- useEffect Hook.
<br/>


 What are you most excited about trying to implement or see how it works?
- Hooks.

<br/>

<br/>
<br/>
<br/>
<br/>

# References:
- [effects hook](https://reactjs.org/docs/hooks-effect.html)