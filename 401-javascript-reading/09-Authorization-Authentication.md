# Authorization/Authentication


**What header(s) are used in authentication and authorization?**

**The HTTP Authorization request header** it used to provide credentials that authenticate a user agent with a server and header is usually, but not always, sent after the user agent first attempts to request a protected resource without credentials.

**The Authentication** The Authentication scheme that defines how the credentials are encoded, This header indicates what authentication schemes can be used to access the resource. 

**What is safe to put into a JWT?**

The RFC just shows you how you can structure a given message and how you can add layers of security, which will protect the integrity and, optionally, the content of the message. But JWTs are not secure just because they are JWTs, it's the way we use them that determines whether they are secure or not.



**How are JWTs validated?**

The entire point of signing the token is so that whoever receives the token can validate that this JWT contains data that hasn't been tampered with. And in order to validate a JWT, we should check some registered claims as well. The "iss" (issuer) claim identifies the principal that issued the JWT. 

The high-level overview of validating an access token looks like this:

* Retrieve and parse your Okta JSON Web Keys (JWK), which should be checked periodically and cached by your application.

* Decode the access token, which is in JSON Web Token format
* Verify the signature used to sign the access token
* Verify the claims found inside the access token



**Terms** 

**RBAC** Role-Based Access Control(RBAC) it give us rights to being access resourceses and its part of policy.

**User Roles** roles that give the users access based on their role in an organization.

**JWT Token** JSON Web Token structure it's compact form consist of three parts separated by dots are header, payload and signtures.

[Home](../README.md)