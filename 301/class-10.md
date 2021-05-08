# The JavaScript Call Stack  

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.  

In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.  

### What is the call stack?  
 * Last In, First Out (LIFO) 
 When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.  

 * Temporarily store: 
 When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.  

 * Manage function invocation (call):  
 The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.  


# JavaScript error messages && debugging  

### Types of error messages 

* Reference errors  
This is as simple as when you try to use a variable that is not yet declared you get this type os errors.  

* Syntax errors  
Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.  

* Type errors  
Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible  

###  Debugging
* `console.log()`  
by using chrome developer tools, open your page with your JS code (press cmd+o in macOS or Ctrl+o in Windows) and choose your file to debug, click the line you wanna debug and refresh your page again (F5).  


*  debugger statement  
The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.  


* conditional breakpoints  
by right-clicking a previous set breakpoint, which will make your program stop at that point only if a condition is met, this is awesome for when you want to debug huge cycles for specific values.   


### Tools to avoid runtime errors  
*quokka* to evaluate your code as you type  
*eslint* to make sure your style guide is consistency and it will grab you an error or two along the way and  
*TypeScript* For those of you looking to make JS a more strong typed experience you can check out stuff   