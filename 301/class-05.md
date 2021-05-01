# React  

## Thinking in React  
One of the many great parts of React is how it makes you think about apps as you build them. In this document, we’ll walk you through the thought process of building a searchable product data table using React.  


 
### Step 1: Break The UI Into A Component Hierarchy  
How do you know what should be its own component? Use the same techniques for deciding if you should create a new function or object. One such technique is the single responsibility principle, that is, a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.  

### Step 2: Build A Static Version in React  
To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.  


### Step 3: Identify The Minimal (but complete) Representation Of UI State  
To build your app correctly, you first need to think of the minimal set of mutable state that your app needs. The key here is DRY: Don’t Repeat Yourself. Figure out the absolute minimal representation of the state your application needs and compute everything else you need on-demand. For example, if you’re building a TODO list, keep an array of the TODO items around; don’t keep a separate state variable for the count. Instead, when you want to render the TODO count, take the length of the TODO items array.  


### Step 4: Identify Where Your State Should Live   
For each piece of state in your application:  

* Identify every component that renders something based on that state.  
* Find a common owner component (a single component above all the components that need the state in the hierarchy).  
* Either the common owner or another component higher up in the hierarchy should own the state.  
* If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.  


### Step 5: Add Inverse Data Flow  
React makes this data flow explicit to help you understand how your program works, but it does require a little more typing than traditional two-way data binding.  




## And That’s It




