# `<Login />` and `<Auth />`

**Definition of Role-Based Access Control**

Role-based access control restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network. As a result, lower-level employees usually do not have access to sensitive data if they do not need it to fulfill their responsibilities. Using RBAC will help in securing your company’s sensitive data and important applications


**Best Practices for Implementing RBAC**

Implementing a RBAC into your organization shouldn’t happen without a great deal of consideration. A core business function of any organization is protecting data. Furthermore, it can secure key business processes, including access to IP, that affect the business from a competitive standpoint. Achieve a higher level of employee security awareness with this resource kit.


**react-cookies**

```
$ npm install react-cookies --save

npm install react-cookie
```

> To be able to access user cookies while doing server-rendering, you can use plugToRequest or setRawCookie.


`<CookiesProvider />`

Set the user cookies

On the server, the cookies props must be set using req.universalCookies or new Cookie(cookieHeader)

* useCookies([dependencies])
* setCookie(name, value, [options])
* removeCookie(name, [options])
* withCookies(Component)
* get(name, [options])
* getAll([options])


**Simple Example with React hooks**

```
// Root.jsx
import React from 'react';
import App from './App';
import { CookiesProvider } from 'react-cookie';

export default function Root() {
  return (
    <CookiesProvider>
      <App />
    </CookiesProvider>
  );
}
```



[Home](../README.md)
