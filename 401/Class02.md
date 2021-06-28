## Deference between `Put` and `Patch`  
`PUT` is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely. PUT is similar to POST in that it can create resources, but it does so when there is a defined URI. PUT overwrites the entire entity if it already exists, and creates a new resource if it doesn’t exist.  

`PATCH` applies a partial update to the resource.This means that you are only required to send the data that you want to update, and it won’t affect or change anything else. So if you want to update the first name on a database, you will only be required to send the first parameter; the first name.  
&nbsp;

## Tools To Mock HTTP Requests  
1 – Nock  
2 – MockServer  
3 – Beeceptor  
4 – Postman Mock Server


## Compare and contrast SOAP and REST  

*SOAP*   
- Language, platform, and transport independent (REST requires use of HTTP)     
- Works well in distributed enterprise environments (REST assumes direct point-to-point communication)
- Standardized
- Provides significant pre-build extensibility in the form of the WS* standards
- Built-in error handling
- Automation when used with certain language products   

&nbsp;


*REST*  
- Uses easy to understand standards like swagger and OpenAPI Specification 3.0
- Smaller learning curve
- Efficient (SOAP uses XML for all messages, REST mostly uses smaller message formats like JSON)
- Fast (no extensive processing required)
- Closer to other Web technologies in design philosophy

&nbsp;
<span style="color:#39A2DB"><b>Which 3 things had you heard about previously and now have better clarity on? </b></span>


Express  
Nodejs  
npm   

&nbsp;
<span style="color:#39A2DB"><b>Which 3 things are you hoping to learn more about in the upcoming lecture/demo? </b></span>
 

TDD  
supertest   

&nbsp;
<span style="color:#39A2DB"><b>What are you most excited about trying to implement or see how it works?</b></span>    
TDD also   
http status   
Swagger and APIDoc.js 


 &nbsp;

*Terms*  
  

Web Server  
> It's a computer program that distributes web pages as they are requisitioned. The basic objective of the web server is to store, process and deliver web pages to the users. This intercommunication is done using Hypertext Transfer Protocol (HTTP)   

&nbsp;

Express  
> Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.   

&nbsp;

Routing  
> a process of selecting path along which the data can be transferred from source to the destination. Routing is performed by a special device known as a router.    

&nbsp;

WRRC  
> the request/response cycle is a useful guide to see how all the app’s files and folders fit together and traces how a user’s request flows through the app.
