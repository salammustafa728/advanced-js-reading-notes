# Advanced State with Reducers

Basic Hooks useState

It accepts a new state value and enqueues a re-render of the component. During subsequent re-renders, the first value returned by useState will always be the most recent state after applying updates. This is why it’s safe to omit from the useEffect or useCallback dependency list.

useState does not automatically merge update objects.

batched Starting with React 18, batching is enabled for all updates by default.

The function passed to useEffect will run after the render is committed to the screen. And the function passed to useEffect may return a clean-up function.


This is different than useLayoutEffect, which fires the function and processes the updates inside of it immediately. Even in cases where useEffect is deferred until after the browser has painted, it’s guaranteed to fire before any new renders.

> Don’t forget that the argument to useContext must be the context object itself

A component calling useContext will always re-render when the context value changes. If re-rendering the component is expensive, you can optimize it by using memoization.

**useReducer**

Accepts a reducer of type => newState, and returns the current state paired with a dispatch method. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

**useCallback**

Returns a memoized callback. Pass an inline callback and an array of dependencies. useCallback will return a memoized version of the callback that only changes if one of the dependencies has changed. UseCallback is equivalent to useMemo.

The array of dependencies is not passed as arguments to the callback.

**useMemo**

Returns a memoized value. Pass a “create” function and an array of dependencies. useMemo will only recompute the memoized value when one of the dependencies has changed. Remember that the function passed to useMemo runs during rendering.

useLayoutEffect

The signature is identical to useEffect, but it fires synchronously after all DOM mutations. Prefer the standard useEffect when possible to avoid blocking visual updates. However, we recommend starting with useEffect first and only trying useLayoutEffect if that causes a problem. If you use server rendering, keep in mind that neither useLayoutEffect nor useEffect can run until the JavaScript is downloaded.

To fix this, either move that logic to useEffect , or delay showing that component until after the client renders .


Defer formatting debug values

UseDeferredValue useDeferredValue accepts a value and returns a new copy of the value that will defer to more urgent updates. 


**{isPending && }**

Updates in a transition yield to more urgent updates such as clicks. Updates in a transitions will not show a fallback for re-suspended content.

**useInsertionEffect**

Since this hook is limited in scope, this hook does not have access to refs and cannot schedule updates. UseInsertionEffect should be limited to css-in-js library authors.

## UseReducer


UseReducer is one of the additional Hooks that shipped with React v16.8. An alternative to the useState Hook, useReducer helps you manage complex state logic in React applications. When combined with other Hooks like useContext, useReducer can be a good alternative to Redux, Recoil or MobX


**How does the useReducer Hook work?**

The useReducer Hook is used to store and update states, just like the useState Hook. UseReducer returns an array that holds the current state value and a dispatch function to which you can pass an action and later invoke it. For example, the useReducer function is tightly coupled to a specific reducer.


[Home](../README.md)
