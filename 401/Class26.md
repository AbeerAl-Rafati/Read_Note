## Review

**Name 5 Javascript UI Frameworks (other than React)**
* Angular   
* Vue.js   
* jQuery   
* Backbone    
* Ember   

**What’s the difference between a framework and a library?**    
"Inversion of Control". When you call a method from a library, you are in control.    
But with a framework, the control is inverted: the framework calls you. 


&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| Rendering  |    is the process of React asking your components to describe what they want their section of the UI to look like, now, based on the current combination of props and state.         |
| templates   |     are sets of ready-to-use parts of code built using React technology for the development of dynamic user interfaces.         |
|state   |     is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component.         |
|


&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

state

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

templets
state

_What are you most excited about trying to implement or see how it works?_

templets
state
sass

&nbsp;

&nbsp;

## Preparation Materials

> Introducing JSX


- JSX produces React “elements”. We will explore rendering them to the DOM in the next section. Below, you can find the basics of JSX necessary to get you started.

- React doesn’t require using JSX, but most people find it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

- You may also use curly braces to embed a JavaScript expression in an attribute.



&nbsp;

&nbsp;

> Rendering Elements


- An element describes what you want to see on the screen.

- Unlike browser DOM elements, React elements are plain objects, and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

- Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

- React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.




