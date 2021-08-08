## Review

**How does React differ from vanilla JS/HTML/CSS?**
rendering is easier than pure js
more flexible

**What is the primary difference between a function component and a class component?**
no this in function component 
function is shorter
function is more flexable
class more tidy it think 
life cycle in class but useEffect in function


&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| Functional Components   |  These are simply JavaScript functions. We can create a functional component to React by writing a JavaScript function. These functions may or may not receive data as parameters. In the functional Components, the return value is the JSX code to render to the DOM tree.          |
| Children / Child Components  |  special property of React components which contains any child elements defined within the component          |
| 



&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- hooks

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- hooks

_What are you most excited about trying to implement or see how it works?_

- also hooks we keep hearing about since 3 months ago xD

&nbsp;

&nbsp;

## Preparation Materials

> making sense of hooks

- Hooks let us organize the logic inside a component into reusable isolated units   
- it will reduce the number of concepts you need to juggle when writing React applications.    
- In terms of the implementation size, the Hooks support increases React only by ~1.5kB (min+gzip). While this isn’t much, it’s also likely that adopting Hooks could reduce your bundle size because code using Hooks tends to minify better than equivalent code using classes.    
- Since Hooks are regular JavaScript functions, you can combine built-in Hooks provided by React into your own “custom Hooks”.    
- 

&nbsp;

&nbsp;

> the state hook

- importing `useState` :
```
import React, { useState } from 'react';
```

- `useState` is a Hook that lets you add React state to function components.
```
function Example() {
  // Declare a new state variable, which we'll call "count"
  const [count, setCount] = useState(0);

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
>  previously you had to convert it to a class. Now you can use a Hook inside the existing function component. 

- `useState` is a new way to use the exact same capabilities that `this.state` provides in a class.   

- Unlike with classes, the state doesn’t have to be an object. We can keep a number or a string if that’s all we need.   
- It returns a pair of values: the current state and a function that updates it.    
- In a function, we can read it directly:
```
  <p>You clicked {count} times</p>
```
- In a function, we already have setCount so we can update it as following:
```
 <button onClick={() => setCount(count + 1)}>
    Click me
  </button>
```





&nbsp;

&nbsp;

> hooks api
- Hooks are backwards-compatible.  

- You can use the State Hook more than once in a single component.   

- The array destructuring syntax lets us give different names to the state variables we declared by calling useState.    

-  Hooks don’t work inside classes.    

- The Effect Hook, `useEffect`, adds the ability to perform side effects from a function component. It serves the same purpose as `componentDidMount`, `componentDidUpdate`, and `componentWillUnmount` in React classes, but unified into a single API.   


- Rules :

1. Only call Hooks at the top level.  
2. Only call Hooks from React function components.   


&nbsp;

&nbsp;

> hooks api reference

* Basic Hooks

1. useState   
Returns a stateful value, and a function to update it.


2. useEffect   
Accepts a function that contains imperative, possibly effectful code.



3. useContext   
Accepts a context object (the value returned from React.createContext) and returns the current context value for that context.   


* Additional Hooks

1. useReducer   
An alternative to useState. Accepts a reducer of type `(state, action) => newState`, and returns the current state paired with a dispatch method.   

2. useCallback   
Returns a memoized callback.


3. useMemo   
Returns a memoized value.


4. useRef   
returns a mutable ref object whose .current property is initialized to the passed argument (initialValue.The returned object will persist for the full lifetime of the component.   

5. useImperativeHandle   
useImperativeHandle customizes the instance value that is exposed to parent components when using ref.    

6. useLayoutEffect   
The signature is identical to useEffect, but it fires synchronously after all DOM mutations.    

7. useDebugValue   
useDebugValue can be used to display a label for custom hooks in React DevTools.



