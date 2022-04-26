# Component Lifecycle, UseEffect()


You can think of useEffect Hook as componentDidMount, componentDidUpdate, and componentWillUnmount combined.

**Effects Without Cleanup**

Sometimes, we want to run some additional code after React has updated the DOM. Network requests, manual DOM mutations, and logging are common examples of effects that don’t require a cleanup. In React class components, the render method itself shouldn’t cause side effects. React has updated the DOM.

This is why in React classes, we put side effects into componentDidMount and componentDidUpdate. Component { this. Note how we have to duplicate the code between these two lifecycle methods in class. This is because in many cases we want to perform the same side effect regardless of whether the component just mounted, or if it has been updated.

We could extract a separate method but we would still have to call it in two places. Now let’s see how we can do the same with the useEffect Hook.

By using this Hook, you tell React that your component needs to do something after render. Placing useEffect inside the component lets us access the count state variable right from the effect. React guarantees the DOM has been updated by the time it runs the effects.

If you use this optimization, make sure the array includes all values from the component scope that change over time and that are used by the effect. Otherwise, your code will reference stale values from previous renders. While passing as the second argument is closer to the familiar componentDidMount and componentWillUnmount mental model, there are usually better solutions to avoid re-running effects too often.

Example of react uesEffect()

![useEffect](https://miro.medium.com/proxy/1*0pnIR2eh8XBt-57kiA5dvQ.png)


[Home](../README.md)

