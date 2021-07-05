##  Review  

**When is Basic Authorization used vs. Bearer Authorization?**  

basic for authentication  but bearer for authorization used to permit access in several sources connected with server

**What does the JSON Web Token package do?**   

give accsse to other sources if it was identical

**What considerations should we make when creating and storing a SECRET?**   
not to send to client again





##  Vocabulary   

| voc                               | related to |
|-------------------------------------|--------------|
|encryption |is the method by which information is converted into secret code that hides the information's true meaning|
|token|are the thing that applications use to make API requests on behalf of a user. |
|bearer|The most common way of accessing OAuth 2.0 APIs is using a “Bearer Token”. This is a single string which acts as the authentication of the API request, sent in an HTTP “Authorization” header.  |
|secret|secret key is private to you which means you will never reveal that to the public or inject inside the JWT token.|
|JSON Web Token| is a proposed Internet standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims. |
|



## Preview  


*Which 3 things had you heard about previously and now have better clarity on?*  
- jwt
- 
- 

*Which 3 things are you hoping to learn more about in the upcoming lecture/demo?*  
-  jwt 
-  jwt token
- 

*What are you most excited about trying to implement or see how it works?*  
- ok only to do my lab in success way lol ...

&nbsp;

## Preparation Materials

> 5 steps to RBAC        

RBAC is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.   


- Benefits of RBAC?   
With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable.   

- RBAC vs. ABAC vs. ACL   

*Access control lists (ACL)*  An ACL is a means of defining access rights by a given user or user group, to a specific object, such as a document.   

*Attribute-based access control (ABAC)* — ABAC, sometimes known as policy-based access control, can use a variety of attributes, including user department, time of day, location of access, type of access required, etc.    


- RBAC implementation    
1. Inventory your systems   
2. Analyze your workforce and create roles   
3. Assign people to roles   
4. Never make one-off changes   
5. Audit   


&nbsp;

&nbsp;

> wiki - RBAC  

- *role-based security* is an approach to restricting system access to authorized users. It is an approach to implement mandatory access control (MAC) or discretionary access control (DAC).

- Three primary rules are defined for RBAC:   
1. Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.
2. Role authorization: A subject's active role must be authorized for the subject.
3. Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role.
 