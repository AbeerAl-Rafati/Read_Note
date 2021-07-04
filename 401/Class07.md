##  Review  

**Write the following steps in the correct order:**  

Make a request to a third-party API endpoint
Redirect to a third party authentication endpoint
Receive authorization code
Receive access token
Make a request to the access token endpoint
Register your application to get a client_id and client_secret
Ask the client if they want to sign in via a third party

**What can you do with an authorization code?**   

give user access

**What can you do with an access token?**   

use to access only with token

**What’s a benefit of using OAuth instead of your own basic authentication?**  

i can handel it as well as i want

##  Vocabulary   

| voc                               | related to |
|-------------------------------------|--------------|
|Client ID |s on all documents you get from us. It is an eight or ten-digit number that looks like this: 0000-0000 or 00-0000-0000|
|Client Secret|secret known only to your application and the authorization server. It protects your resources by only granting tokens to authorized requestors.|
|Authentication Endpoint|authentication mechanism used to verify the identity of a network's external or remote connecting device |
|Access Token Endpoint|A token endpoint is an HTTP endpoint that clients can use to obtain an access token given an authorization code.
 |
|API Endpoint|is a point at which an application program interface (API) -- the code that allows two software programs to communicate with each other|
|Authorization Code| is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space.|
|Access Token|are the thing that applications use to make API requests on behalf of a user.|
|



## Preview  


*Which 3 things had you heard about previously and now have better clarity on?*  
- access token
- auth code
- 

*Which 3 things are you hoping to learn more about in the upcoming lecture/demo?*  
- auth code
- cliend secret 
- 

*What are you most excited about trying to implement or see how it works?*  
- auth in general

&nbsp;

## Preparation Materials


> Intro to JWT   

- JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.   

- Although JWTs can be encrypted to also provide secrecy between parties, we will focus on signed tokens. Signed tokens can verify the integrity of the claims contained within it, while encrypted tokens hide those claims from other parties.   

- **When should you use JSON Web Tokens?**   
Authorization   
Information Exchange   

- **What is the JSON Web Token structure?**   
Header  
Payload  
Signature   


- In authentication, when the user successfully logs in using their credentials, a JSON Web Token will be returned. Since tokens are credentials, great care must be taken to prevent security issues. In general, you should not keep tokens longer than required.   





&nbsp;

&nbsp;

> Are JWTs Secure?  

- JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.   

