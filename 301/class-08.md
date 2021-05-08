# Web API design  

well-designed web API should aim to support:
* Platform independence.  
* Service evolution.  

### Introduction to REST   
is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST implementations use HTTP as the application protocol   




### main design principles of RESTful APIs using HTTP:  

* REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.  
* A resource has an identifier, which is a URI that uniquely identifies that resource.   
* Clients interact with a service by exchanging representations of resources. Many web APIs use JSON as the exchange format.  
* REST APIs use a uniform interface, which helps to decouple the client and service implementations. 
* REST APIs use a stateless request model. HTTP requests should be independent and may occur in any order, so keeping transient state information between requests is not feasible.  
* REST APIs are driven by hypermedia links that are contained in the representation.  


### Define operations in terms of HTTP methods  

* GET 
retrieves a representation of the resource at the specified URI.  


> A successful GET method typically returns HTTP status code 200 (OK). If the resource cannot be found, the method should return 404 (Not Found).  


* POST   
creates a new resource at the specified URI.  

> the method can return HTTP status code 200 and include the result of the operation in the response body. Alternatively, if there is no result to return, the method can return HTTP status code 204  


* PUT  
either creates or replaces the resource at the specified URI. 

>  it returns HTTP status code 201 (Created), as with a POST method. If the method updates an existing resource, it returns either 200 (OK) or 204 (No Content).  

* PATCH   
performs a partial update of a resource.


> | Error condition	                |HTTP status code                         |
> |---------------------------------|-----------------------------------------|
> |The patch document format isn't<br> supported.	 |  415 (Unsupported Media Type)           |
> |Malformed patch document.	      |  400 (Bad Request)                      |
> |The patch document is valid, but<br>, but the changes can't be applied to<br> the resource in its current state. | 409 (Conflict)                          |



* DELETE  
removes the resource at the specified URI.  

> the web server should respond with HTTP status code 204, indicating that the process has been successfully handled, but that the response body contains no further information. If the resource doesn't exist, the web server can return HTTP 404 (Not Found).  


# Regex 

Anchors — ^ and $  

> ^The        matches any string that starts with The  
> end$        matches a string that ends with end
> ^The end$   exact string match (starts and ends with The end)
> roar        matches any string that has the text roar in it  


Quantifiers — * + ? and {}  

> abc*        matches a string that has ab followed by zero or more c -> Try it!
> abc+        matches a string that has ab followed by one or more c
> abc?        matches a string that has ab followed by zero or one c
> abc{2}      matches a string that has ab followed by 2 c
> abc{2,}     matches a string that has ab followed by 2 or more c
> abc{2,5}    matches a string that has ab followed by 2 up to 5 c
> a(bc)*      matches a string that has a followed by zero or more copies of the sequence bc
> a(bc){2,5}  matches a string that has a followed by 2 up to 5 copies of the sequence bc


OR operator — | or []

> > a(b|c)     matches a string that has a followed by b or c (and captures b or c) 
> a[bc]      same as previous, but without capturing b or c

Character classes — \d \w \s and .

> \d         matches a single character that is a digit 
> \w         matches a word character (alphanumeric character plus underscore) 
> \s         matches a whitespace character (includes tabs and line breaks)
> .          matches any character 