## ES6 Classes, Using Express Routing, Express Routing


### Name 3 real world use cases where you’d want to change the request with custom middleware?

* Error Handling
 * logging
 * Auth 

### True or false: The route handler is middleware?

***True***

### In what ways can a middleware function end the process and send data to the browser?
 
 * res.send()
 * res.render()
 * res.end()
 

### At what point in the request lifecycle can you “inject” middleware?
    
    

### What can cause express to error with “Request headers sent twice, cannot start a second response”



## Classes

It's template for creating objects and we can use by create an instances of it.

class syntax has two components: class expressions and class declarations

> class declarations: its define a class, write **class** keyword then the name of it.

> class expressions: is another way to define a class, it can be named or unnamed 

class example:

![class](https://www.codegrepper.com/codeimages/node-js-class.png)

## Routing

Its how the endpoints respond to client request

To defind it use the HTTP methods post, get, put or delete. and it specify a callback function.

### Route paths: 
define the endpoints at which requests can be made, can be string, tring patterns, or regular expressions.

### Route parameters
Its a named URL segments that are used to capture the values specified at their position in the URL.

### Route handlers 
its provide multiple callback functions that behave like middleware to handle a request.

![](https://www.codegrepper.com/codeimages/node.js-routes-order.png)


[Home](README.md)