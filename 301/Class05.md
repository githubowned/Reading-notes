# Read: Class 05 - Readings: Putting it all together

---

## What is Json API?
JSON:API is a specification for how a client should request that resources be fetched or modified, and how a server should respond to those requests.



JSON:API is designed to minimize both the number of requests and the amount of data transmitted between clients and servers. This efficiency is achieved without compromising readability, flexibility, or discoverability.

<p>&nbsp;</p>
<p>&nbsp;</p>

## What is a Mock?
In object-oriented programming, mock objects are simulated objects that mimic the behavior of real objects in controlled ways, most often as part of a software testing initiative. 
<p>&nbsp;</p>

## What is the single component principle?
the single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

<p>&nbsp;</p>
<p>&nbsp;</p>

## How to break the user interface into a component hierarchy ?
- draw boxes around every component (and subcomponent) in the mock and give them all name.

-after having identified the components in our mock, let’s arrange them into a hierarchy.

<p>&nbsp;</p>
<p>&nbsp;</p>

## How do you know what should be its own component? 
- Use the single component principle.

<p>&nbsp;</p>

## What is A static Version website?
- A website that renders the user interface but has no interactivity.
<p>&nbsp;</p>
<p>&nbsp;</p>

> -  To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. 
props are a way of passing data from parent to child. 
> - Don’t use state at all to build this static version.
> - State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.


<p>&nbsp;</p>

- To make your UI interactive, you need to be able to trigger changes to your underlying data model. React achieves this with state.


<p>&nbsp;</p>
<p>&nbsp;</p>

 - ## Ask three questions about each piece of data:

1. Is it passed in from a parent via props? If so, it probably isn’t state.

2. Does it remain unchanged over time? If so, it probably isn’t state.

3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

<p>&nbsp;</p>
<p>&nbsp;</p>

## HOW to identify which component mutates, or owns, this state?
1. Identify every component that renders something based on that state.

2. Find a common owner component (a single component above all the components that need the state in the hierarchy).

3. Either the common owner or another component higher up in the hierarchy should own the state.

4. If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.












<p>&nbsp;</p>
<p>&nbsp;</p>

## Things I want to know more about:
---




<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>

<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>











# References:



- [React Docs - thinking in React](https://reactjs.org/docs/thinking-in-react.html)