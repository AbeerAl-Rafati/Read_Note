## Review

**Why is the Context API useful?**    
way to enable components to share some data without explicitly passing via each component manually.    

**Can a component outside of a provider get its context?**     
no   

**What are some common use cases for using the Context API?**   
Theming       
Pass down translation messages   
Authentication   

**Describe “Context Hell”**   
is the nasty code you get taking advantage of the React Context API.    






&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| global state  |  Context provides a way to pass data through the component tree without having to pass props down manually at every level          |
| global context | Context is designed to share data that can be considered “global” for a tree of React components            |
| provider  | React component that allows consuming components to subscribe to context changes.            |
|consumer  |    component that subscribes to context changes.        |
|

&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- context

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- context
- auth from front end prospective

_What are you most excited about trying to implement or see how it works?_

- auth from front end prospective

&nbsp;

&nbsp;

## Preparation Materials

> what is role based access control?

- Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.    


- BENEFITS OF RBAC:   
1. Reducing administrative work and IT support.   
2. Improving compliance.   
3. Maximizing operational efficiency   


&nbsp;

&nbsp;

> react-cookies component

How to use
- $ npm install react-cookies --save
- import cookie from 'react-cookies'
```
 componentWillMount() {
    this.state =  { userId: cookie.load('userId') }
  }
 
  onLogin(userId) {
    this.setState({ userId })
    cookie.save('userId', userId, { path: '/' })
  }
 
  onLogout() {
    cookie.remove('userId', { path: '/' })
  }
  ```


