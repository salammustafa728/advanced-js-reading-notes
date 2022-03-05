# Authentication

1. **Securing Passwords with Bcrypt Hashing Function**

passwords are stored using a hashing algorithm. Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3. Hashing is a way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

and there's a lot of problems with cryptographic HASH ALGORITHM: 
 * Brute Force attack
 * Hash Collision attack
 

2. **Basic Auth**

Basic access authentication is a method for an HTTP user agent ex: web browser and it's a technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages. it uses standard fields in the HTTP header.

Microsoft Internet Explorer offers a dedicated JavaScript method to clear cached credentials:

```
<script>document.execCommand('ClearAuthenticationCache');</script>
```

3. OWASP auth cheatsheet

**Authentication:** is the process of verifying that an individual. 

**Session Management** is a process by which a server maintains the state of an entity interacting with it.

And it's a way for securing the password and username
by using some mechanizsm lik: Store Passwords in a Secure Fashion or Compare Password Hashes Using Safe Functions. 

| Attack Type |	Description |
|------------ | ----------- |
| Brute Force |	Testing multiple passwords from a dictionary or other source against a single account. |
| Credential Stuffing |	Testing username/password pairs obtained from the breach of another site. |
| Password Spraying   |	 Testing a single weak password against a large number of different accounts. |

Use of authentication protocols that require no password ex: OAuth, OpenId, SAML, and FIDO.


4. bcrypt docs

**node.bcrypt.js** A library to help you hash passwords.

>node-gyp only works with stable/released versions of node

The migration should be a bump in the package.json and the Dependencies NodeJS and node-gyp. 

And you should install bcrypt:

> npm install bcrypt

bcrypt uses whatever Promise implementation is available.

**To hash a password:**

1.  (generate a salt and hash on separate function calls)

2. (auto-gen a salt and hash)




[Home](README.md)