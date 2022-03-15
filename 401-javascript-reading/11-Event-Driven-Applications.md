# Event Driven Applications


## 1- Event Driven Programming

**is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision**


* An Event Handler is a callback function that will be called when an event is triggered.
* A Main Loop listens for event triggers and calls the associated event handler for that event.

**EventEmitter**

that allows us to get started incorporating Event-Driven Programming in our project, if we want to use it so we need to import it once imported we’ll need to create a new object from the class to start using it.
And EventEmitter has an emit method that we we use to trigger the event.

**Removing Listeners** 

Also you can remove event listener after use it or when you don't need it by using the removeListener or removeAllListeners method.


## 2- Node docs: events

Node.js core API is built around an idiomatic asynchronous event-driven architecture in which certain kinds of objects


The eventEmitter.emit() method allows an arbitrary set of arguments to be passed to the listener functions. Keep in mind that when an ordinary listener function is called, the standard this keyword is intentionally set to reference the EventEmitter instance to which the listener is attached.

>The EventEmitter calls all listeners synchronously in the order in which they were registered

>Using the eventEmitter.once() method, it is possible to register a listener that is called at most once for a particular event. Once the event is emitted, the listener is unregistered and then called.

>If an EventEmitter does not have at least one listener registered for the 'error' event, and an 'error' event is emitted, the error is thrown, a stack trace is printed, and the Node.js process exits.

>The captureRejections option in the EventEmitter constructor or the global setting change this behavior

> emitter.getMaxListeners() Returns the current max listener value for the EventEmitter, set by emitter.setMaxListeners(n) or defaults to events.defaultMaxListeners.

> emitter.listenerCount(eventName) Returns the number of listeners listening to the event named eventName.

> emitter.once(eventName, listener) Adds a one-time listener function for the event named eventName

> emitter.rawListeners(eventName) Returns a copy of the array of listeners for the event named eventName include any wrappers

and there's a lot of event methods we can use like event.composedPath(), event.currentTarget and etc..

[Home](../README.md)



