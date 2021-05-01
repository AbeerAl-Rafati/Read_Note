# React   

## Forms  
HTML form elements work a little bit differently from other DOM elements in React, because form elements naturally keep some internal state.  

## Controlled Components  
 In React, mutable state is typically kept in the state property of components, and only updated with`setState()`.  

We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.  

Since the `value` attribute is set on our form element, the displayed value will always be `this.state.value`, making the React state the source of truth.  


### The textarea Tag  
In React, a `<textarea>` uses a `value` attribute instead. 


### The select Tag  
 React, instead of using this `selected` attribute, uses a `value` attribute on the root `select` tag.  


## Handling Multiple Inputs  
When you need to handle multiple controlled `input` elements, you can add a `name` attribute to each element and let the handler function choose what to do based on the value of `event.target.name`.


### Controlled Input Null Value  
If you’ve specified a value but the `input` is still editable, you may have accidentally set `value` to `undefined` or null.


## The Conditional Operator Explained  
Shorten your `if` statements into one line of code with the conditional operator  

>
> `person.driver = person.age >=16 ? 'Yes' : 'No';`  
>

## Nested Ternary  

>
> `let isStudent = false;`
> `let isSenior = true;`
> `let price = isStudent ? 8 : isSenior ? 6 : 10`
> `console.log(price);` // 6
> 
