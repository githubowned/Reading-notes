
## Compare and Contrast Redux Toolkit with Redux “Ducks”

- Redux Toolkit’s goal is to help simplify common Redux use cases. It is not intended to be a complete solution for everything you might want to do with Redux, but it should make a lot of Redux-related code you need to write a lot simpler

<br/>

## What is the principle advantage of Redux Toolkit

- Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code. Redux Toolkit is beneficial to all Redux users regardless of skill level or experience.
<br/>
<br/>
<br/>

## Terms

- **redux toolkit slice** is a function that accepts an initial state, an object full of reducer functions, and a “slice name”, and automatically generates action creators and action types that correspond to the reducers and state. This API is the standard approach for writing Redux logic.

<br/>

- **namespace** is a declarative region that provides a scope to the identifiers (the names of types, functions, variables, etc) inside it. Namespaces are used to organize code into logical groups and to prevent name collisions that can occur especially when your code base includes multiple libraries.

<br/>


# Preparation material

## React Native
- Many different kinds of people use React Native: from advanced iOS developers to React beginners, to people getting started programming for the first time in their career. These docs were written for all learners, no matter their experience level or background.
<br/>


- To work with React Native, you will need to have an understanding of JavaScript fundamentals. If you’re new to JavaScript or need a refresher, you can dive in or brush up at Mozilla Developer Network.
<br/>


- With React, you can make components using either classes or functions. Originally, class components were the only components that could have state. But since the introduction of React’s Hooks API, you can add state and more to function components.
<br/>


- React Native is like React, but it uses native components instead of web components as building blocks. So to understand the basic structure of a React Native app, you need to understand some of the basic React concepts, like JSX, components, state, and props. If you already know React, you still need to learn some React-Native-specific stuff, like the native components. This tutorial is aimed at all audiences, whether you have React experience or not.
<br/>


## Example

```js
import React from 'react';
import { Text, View } from 'react-native';

const YourApp = () => {
  return (
    <View style={{ flex: 1, justifyContent: "center", alignItems: "center" }}>
      <Text>
        Try editing me! 🎉
      </Text>
    </View>
  );
}

export default YourApp;
```
<br/>
<br/>


## What is EXPO?
Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.
<br/>


## configuring React Native
`npm install --global expo-cli`

`expo init my-projec`
<br/>

<br/>

## Ejecting to ExpoKit
ExpoKit is an Objective-C and Java library that allows you to use the Expo platform and your existing Expo project as part of a larger standard native project -- one that you would normally create using Xcode, Android Studio, or `react-native init`.

<br/>
<br/>
<br/>







# References :
[getting started with react native](https://facebook.github.io/react-native/docs/getting-started)

[react native basics (Tutorial)](https://facebook.github.io/react-native/docs/tutorial)

[react native](https://facebook.github.io/react-native/)

[expo](https://expo.io/)

[expo snack](https://snack.expo.io/)

[ejecting](https://docs.expo.io/versions/latest/expokit/eject)
