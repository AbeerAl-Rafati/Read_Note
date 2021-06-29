## Questions  


*Name 3 real world use cases where you’d want to change the request with custom middleware*  
- API management     
- messaging  
- authentication   

&nbsp;

*The route handler is middleware?* 
<span style="color:#39A2DB"><b>True</b></span>   

&nbsp;

*In what ways can a middleware function end the process and send data to the browser?*  
it can do the following things in the end:
- Execute any code.  
- Make changes to the request and the response objects.  
- End the request-response cycle.  
- Call the next middleware in the stack.   

&nbsp;

*At what point in the request lifecycle can you “inject” middleware?*  
in the middle between the req and the res

&nbsp;

*What can cause express to error with “Request headers sent twice, cannot start a second response”*  
- when request handler function already sent a response to the client

&nbsp;

## Vocabulary   

| vocab  | definitions |
|--------|-------------|
| Middleware | software that provides common services and capabilities to applications outside of what’s offered by the operating system.  
| Request Object | The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.
| Response Object | The res object represents the HTTP response that an Express app sends when it gets an HTTP request.
| Application Middleware | Bind application-level middleware to an instance of the app object by using the app.use() and app.METHOD() functions, where METHOD is the HTTP method of the request that the middleware function handles  
| Routing Middleware | Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router().  
| Test Driven Development | software development approach in which test cases are developed to specify and validate what the code will do.    
| Behavioral Testing | The testing of external behavior of the program is known as Black Box Testing.  
|

&nbsp;

## Preview 
*Which 3 things had you heard about previously and now have better clarity on?*  
- middleware, 
- wrrc  


*Which 3 things are you hoping to learn more about in the upcoming lecture/demo?*  

- testing  
- app middleware and
- behavioral testing

*What are you most excited about trying to implement or see how it works?*
- authntication middleware 

&nbsp;


## Preparation Materials  

>  ES6 Classes  

- Classes are a template for creating objects.  
- class declarations are not hoisted  
- Class declarations  
```
ex:
class Rectangle {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
}
```
- Class expressions  
```
let Rectangle = class {
  constructor(height, width) {
    this.height = height;
    this.width = width;
  }
};
```
- This is where you define class members, such as methods or constructor.  

- The extends keyword is used in class declarations or class expressions to create a class as a child of another class.


&nbsp;

> Using Express Routing  

- Routing refers to how an application’s endpoints (URIs) respond to client requests.  
- Define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests.  
- the routing methods can have more than one callback function as arguments, With multiple callback functions, it is important to provide next as an argument to the callback function and then call next() within the body of the function to hand off control to the next callback.  

- There is a special routing method, app.all(), used to load middleware functions at a path for all HTTP request methods.   
- Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.   
- Route parameters are named URL segments that are used to capture the values specified at their position in the URL   
- ou can create chainable route handlers for a route path by using app.route().  
- Use the express.Router class to create modular, mountable route handlers. 

&nbsp;


> Express Routing  

- Express Router is mini express application with only  routing stuff. 
-  to set a default root for using these routes we just defined. If we use app.use('/app', router), then our routes would be http://localhost:8080/app and http://localhost:8080/app/about.  
- we can use that for basic routes, authenticated routes, and even API routes.   
- Route middleware in Express is a way to do something before a request is processed.
- used for checking if a user is authenticated, logging data for analytics, or anything else we'd like to do before we actually spit out information to our user.  

- The order you place your middleware and routes is very important.  
- Express's .param() middleware. This creates middleware that will run for a certain route parameter.   
- app.route is basically a shortcut to call the Express Router. Instead of calling express.Router(), we can call app.route and start applying our routes there.   




&nbsp;

## References   
[RedHat](https://www.redhat.com/en/topics/middleware/what-is-middleware)  
[expressjs](https://expressjs.com/en/guide/writing-middleware.html)
