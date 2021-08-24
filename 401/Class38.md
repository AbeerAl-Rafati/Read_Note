## Review

**How granular should your reducers be?**    
separeted reduces will be easier    

**Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched**    
  only by filtering it will prevent prone

**Name a strategy for preventing the above**    
redux thunk



&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| store   |    mmutable object tree in Redux        |
| combined reducers  |   helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore          |
|

&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- redux

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- redux

_What are you most excited about trying to implement or see how it works?_

async redux actions

&nbsp;

&nbsp;

## Preparation Materials

> async actions

- common kinds of side effects are things like:   

Logging a value to the console   
Saving a file   
Setting an async timer   
Making an AJAX HTTP request   
Modifying some state that exists outside of a function, or mutating arguments to a function   
Generating random numbers or unique random IDs (such as Math.random() or Date.now())   

- Redux middleware were designed to enable writing logic that has side effects.   

- We could have our middleware check to see if the "action" is actually a function instead, and if it's a function, call the function right away. That would let us write async logic in separate functions, outside of the middleware definition.   

- Once that dispatched value reaches a middleware, it can make an async call, and then dispatch a real action object when the async call completes.  

- Writing async logic as thunk functions allows us to reuse that logic without knowing what Redux store we're using ahead of time.   



&nbsp;

&nbsp;

> redux thunk

- Redux’s actions are dispatched synchronously, which is a problem for any non-trivial app that needs to communicate with an external API or perform side effects. Redux also allows for middleware that sits between an action being dispatched and the action reaching the reducers.  

- There are two very popular middleware libraries that allow for side effects and asynchronous actions: Redux Thunk and Redux Saga. In this post, you will explore Redux Thunk.   

- Thunk is a programming concept where a function is used to delay the evaluation/calculation of an operation.   

- Redux Thunk is a middleware that lets you call action creators that return a function instead of an action object. That function receives the store’s dispatch method, which is then used to dispatch regular synchronous actions inside the function’s body once the asynchronous operations have been completed.   

- The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data.     
- 
