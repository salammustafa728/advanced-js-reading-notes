#  Context API

**Context**

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

> All consumers that are descendants of a Provider will re-render whenever the Provider’s value prop changes.


The management of that state (adding, removing) needs to be globally accessible.

The **useContext** and **useReducer**, the combination of these two hooks means we can have a global state and use Redux-like reducers, actions, and dispatchers to mutate that global state. To an extent, it’s possible.

[Tutorials about context](https://github.com/diegohaz/awesome-react-context)


[Home](../README.md)