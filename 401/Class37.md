## Review

**Why choose Redux instead of the Context API for global state?**    
Redux works around the idea of having a central state called a store. To change the state, a component has to dispatch an action. The action is then passed on to the reducer, which changes the state of our application.    


**What is the purpose of a reducer?**    
a reducer is a pure function that takes an action and the previous state of the application and returns the new state.    

**What does an action contain?**    
Actions are the only source of information for the store as per Redux official documentation. It carries a payload of information from your application to store.   

**Why do we need to copy the state in a reducer?**    
the reducer must create new object, and making a copy is a way to describe the unchanged part.    




&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| immutable state   |   (unchangeable object) is an object whose state cannot be modified after it is created.          |
| time travel in redux   |  the ability to move back and forth among the previous states of an application and view the results in real time.          |
| action creator   |  to define an action in Redux is to separately declare an action type constant and an action creator function for constructing actions of that type.           |
| reducer   |  pure function that takes an action and the previous state of the application and returns the new state.          |
| dispatch   |  when we invoke dispatch and pass in an action object, the dispatch function calls our reducer and passes in the current state and the action object          |
| 






&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- martial ui

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- martial ui
- redux

_What are you most excited about trying to implement or see how it works?_

- redux

&nbsp;

&nbsp;

## Preparation Materials

> Redux Docs: Using Combined Reducers

- Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.   
- Redux provides the combineReducers utility to implement that behavior. It is an example of a higher-order reducer, which takes an object full of slice reducer functions, and returns a new reducer function.    
- here are two ways to define the initial shape and contents of your store's state. First, the createStore function can take preloadedState as its second argument.    
- 

&nbsp;

&nbsp;

> Redux Docs: Combined Reducer Syntax

- The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.   
- The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers()   
- You can control state key names by using different keys for the reducers in the passed object. For example, you may call combineReducers({ todos: myTodosReducer, counter: myCounterReducer }) for the state shape to be { todos, counter }.    
- You may call combineReducers at any level of the reducer hierarchy. It doesn't have to happen at the top. In fact you may use it again to split the child reducers that get too complicated into independent grandchildren, and so on.   
