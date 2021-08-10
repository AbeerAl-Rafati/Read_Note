## Review

**Why do we not need more .html pages in a multi-page React app?**     
using routes   

**If we wanted a component to show up on every page, where would we put it and why?**  

Inside the <BrowserRouter />, outside a <Route />  


**What does routing do with the components that were rendered when a new route is requested**  
hide it   

**What does props.children contain?**  
any data passed from the parent   

**How do useState() and this.setState() differ?**
don't , one used in class and the other used in function components



&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| State Hook   | Returns a stateful value, and a function to update it.           |
| Mounting    |   (adding nodes to the DOM)          |
|Un-Mounting   |   (removing them from the DOM)          |
|

&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

hooks

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

hooks

_What are you most excited about trying to implement or see how it works?_

-hooks

&nbsp;

&nbsp;

## Preparation Materials

> Using the Effect Hook

- The Effect Hook lets you perform side effects in function components, Data fetching, setting up a subscription, and manually changing the DOM in React components are all examples of side effects.      

- `useEffect` Hook as `componentDidMount`, `componentDidUpdate`, and `componentWillUnmount` combined.   

- In React class components, the render method itself shouldn’t cause side effects. It would be too early — we typically want to perform our effects after React has updated the DOM.   

- Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect.    

- By default, it runs both after the first render and after every update. (We will later talk about how to customize this.) Instead of thinking in terms of “mounting” and “updating”, you might find it easier to think that effects happen “after render”.   

- Every effect may return a function that cleans up after it. This lets us keep the logic for adding and removing subscriptions close to each other.   

- The Effect Hook unifies both use cases with a single API.   

- Tips for Using Effects   
1. Use Multiple Effects to Separate Concerns   
2. Optimizing Performance by Skipping Effects   
3. 

&nbsp;

&nbsp;

