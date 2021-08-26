## Review

**Compare and Contrast Redux Toolkit with Redux “Ducks”**    
Redux Toolkit's goal is to help simplify common Redux use cases. It is not intended to be a complete solution for everything you might want to do with Redux, but it should make a lot of Redux-related code you need to write a lot simpler.     

**What is the principle advantage of Redux Toolkit**    
Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code. Redux Toolkit is beneficial to all Redux users regardless of skill level or experience.     


&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| redux toolkit slices   | A function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state. This API is the standard approach for writing Redux logic.   |
| namespace  | declarative region that provides a scope to the identifiers (the names of types, functions, variables, etc) inside it. Namespaces are used to organize code into logical groups and to prevent name collisions that can occur especially when your code base includes multiple libraries          |
|

&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- redux

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- react native

_What are you most excited about trying to implement or see how it works?_

- react native

&nbsp;

&nbsp;

## Preparation Materials

> getting started with react native

- With React, you can make components using either classes or functions. Originally, class components were the only components that could have state. But since the introduction of React's Hooks API, you can add stae and more to function components.    
- Props   Most components can be customized when they are created, with different parameters. These creation parameters are called props.   

- State   Unlike props that are read-only and should not be modified, the state allows React components to change their output over time in response to user actions, network responses and anything else.    

- 

&nbsp;

&nbsp;

> expo

- Expo is a framework and a platform for universal React applications. It is a set of tools and services built around React Native and native platforms that help you develop, build, deploy, and quickly iterate on iOS, Android, and web apps from the same JavaScript/TypeScript codebase.    
- There are two tools that you need to develop apps with Expo: a command line app called Expo CLI to initialize and serve your project and a mobile client app called Expo Go to open it on iOS and Android. Any web browser will work for opening the project on the web   
- If you use the tools we provide in the managed workflow to build your app, we try to handle as much of the complexity of building apps for you as we can. The tradeoff here is that this workflow won't be suitable for every possible app.   

- 

&nbsp;

&nbsp;

> Ejecting to ExpoKit

- ExpoKit is an Objective-C and Java library that allows you to use the Expo platform and your existing Expo project as part of a larger standard native project -- one that you would normally create using Xcode, Android Studio, or react-native init.   
- If you created an Expo project and you want a way to add custom native modules, this guide will explain how to use ExpoKit for that purpose.   
- You might want to eject if:
Your Expo project needs a native module that Expo doesn't currently support. We're always expanding the Expo SDK, so we hope this is never the case. But it happens, especially if your app has very specific and uncommon native demands.    
