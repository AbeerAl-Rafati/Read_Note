##  Review  

**Explain what a “Singleton” is (in Computer Science terms)**  

node js pattern.   

**Explain how the Singleton pattern can be used with Node modules, specifically with classes**   

It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.  

**If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?**   
ok i am still learning how i should do that =/


##  Vocabulary   

| voc                               | related to |
|-------------------------------------|--------------|
|Router Middleware |the route it self we can consider it as a middleware|
|Dynamic Module Loading|is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory|
|Singleton Pattern| is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself|
|CRUD -> REST Method Matches|**Create** => PUT with a new URI/POST to a base URI returning a newly created URI/ **Read**   = GET/   **Update** = PUT with an existing URI/   **Delete** = DELETE|
|Mock Testing| approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules.|



## Preview  


*Which 3 things had you heard about previously and now have better clarity on?*  
- mocking testing
- patterns in general  
- router

*Which 3 things are you hoping to learn more about in the upcoming lecture/demo?*  
- patterns  
- testing   
- dynamic model loading

*What are you most excited about trying to implement or see how it works?*  
- patterns
## Preparation Materials

> Securing Passwords     


- Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.   

*PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM*
- Brute Force attack 
- Hash Collision attack   

&nbsp;


- To overcome such issues, we need algorithms which can make the brute force attacks slower and minimize the impact. Such algorithms are PBKDF2 and BCrypt, both of these algorithms use a technique called Key Stretching.   

&nbsp;

&nbsp;

> Basic Auth   

- HTTP Basic authentication (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.  


- The BA mechanism does not provide confidentiality protection for the transmitted credentials. They are merely encoded with Base64 in transit and not encrypted or hashed in any way. Therefore, basic authentication is typically used in conjunction with HTTPS to provide confidentiality.  



- Because the BA field has to be sent in the header of each HTTP request, the web browser needs to cache credentials for a reasonable period of time to avoid constantly prompting the user for their username and password. 


&nbsp;

&nbsp;

> bcrypt docs  

A library to help you hash passwords.

install using `npm install bcrypt`   

- Per bcrypt implementation, only the first 72 bytes of a string are used. Any extra bytes are ignored when matching passwords. Note that this is not the first 72 characters. It is possible for a string to contain less than 72 characters, while taking up more than 72 bytes (e.g. a UTF-8 encoded string containing emojis).   

- Usage   
example:   


```
bcrypt.genSalt(saltRounds, function(err, salt) {
    bcrypt.hash(myPlaintextPassword, salt, function(err, hash) {
        // Store hash in your password DB.
    });
});

```