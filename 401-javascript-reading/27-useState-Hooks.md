# Reading: useState() Hook

Hooks apply the React philosophy inside a component, rather than just between the components. That’s why I feel that Hooks are a natural fit for the React component model. Unlike patterns like render props or higher-order components, Hooks don’t introduce unnecessary nesting into your component tree.

Moving logic between functions takes the least amount of effort. However, functions can’t have local React state inside them. You can’t extract behavior like “watch window size and update the state” or “animate a value over time” from a class component without restructuring your code or introducing an abstraction like Observables. Since Hooks are regular JavaScript functions, you can combine built-in Hooks provided by React into your own “custom Hooks”

line service will become 100% free. Read more about it.

    Text example   Delete text

Only argumentative texts
https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889
 
Summary :
	
	Help

Text reduce to 52% ( 937 words / 2017 )

Hooks apply the React philosophy inside a component, rather than just between the components. That’s why I feel that Hooks are a natural fit for the React component model. Unlike patterns like render props or higher-order components, Hooks don’t introduce unnecessary nesting into your component tree.

Do Hooks Make React Bloated?

If the React community embraces the Hooks proposal, it will reduce the number of concepts you need to juggle when writing React applications. Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props. The Hooks proposal doesn’t include any breaking changes. Your existing code would keep on working even if you adopted Hooks in the newly written components.

Still, we’d appreciate if you could experiment with the 16.7 alpha to provide us with feedback on the Hooks proposal and report any bugs. To understand Hooks, we need to take a step back and think about code reuse. Today, there are a lot of ways to reuse logic in React apps. We can write simple functions and call them to calculate something.

We can also write components . Components are more powerful, but they have to render some UI. This is how we end up with complex patterns like render props and higher-order components. Functions seem to be a perfect mechanism for code reuse.

Moving logic between functions takes the least amount of effort. However, functions can’t have local React state inside them. You can’t extract behavior like “watch window size and update the state” or “animate a value over time” from a class component without restructuring your code or introducing an abstraction like Observables. Since Hooks are regular JavaScript functions, you can combine built-in Hooks provided by React into your own “custom Hooks”.

Note that custom Hooks are not technically a React feature.

Show Me Some Code!

Let’s say we want to subscribe a component to the current window width . They involve writing a class, setting up some lifecycle methods, or maybe even extracting a render prop or a higher-order component if you want to reuse it between components. We use the window width in our component, and React re-renders our component if it changes. Let’s look at how we could implement this custom Hook.

We can use them from our components directly, or we can combine them into custom Hooks like useWindowWidth. Using custom Hooks feels as idiomatic as using React’s built-in API. Each Hook may contain some local state and side effects. You can pass data between multiple Hooks just like you normally do between functions.

They can take arguments and return values because they are JavaScript functions.


> we might have a square brackets when we declare a state variable

example: It means that we’re making two new variables fruit and setFruit, where fruit is set to the first value returned by useState, and setFruit is the second.

``` React

import React, { useState } from 'react';

function Example() {
  // Declare a new state variable, which we'll call "count"  const [count, setCount] = useState(0);

```

We declare a state variable called count, and set it to 0. React will remember its current value between re-renders, and provide the most recent one to our function. If we want to update the current count, we can call setCount.

Sometimes, we want to reuse some stateful logic between components. Custom Hooks let you do this, but without adding more components to your tree. Earlier on this page, we introduced a FriendStatus component that calls the useState and useEffect Hooks to subscribe to a friend’s online status. Let’s say we also want to reuse this subscription logic in another component.

**useEffect => {**

It takes friendID as an argument, and returns whether our friend is online. Hooks are a way to reuse stateful logic, not state itself. Custom Hooks are more of a convention than a feature. If a function’s name starts with ”use” and it calls other Hooks, we say it is a custom Hook. 

[Home](../README.md)
