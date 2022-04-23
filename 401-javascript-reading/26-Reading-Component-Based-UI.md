# Reading: Component Based UI

## JSX

JSX:  it is a syntax extension to JavaScript. we use it with React to describe what the UI should look like.


Why JSX? 

Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called «components» that contain both.

Embedding Expressions in JSX 

``` 
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>; 
```

Specifying Attributes with JSX 

``` 
const element = <a href="https://www.reactjs.org"> link </a>;
const element = <img src={user.avatarUrl}></img>;
```

Babel compiles JSX down to React.createElement() calls.

React.createElement() performs a few checks to help you write bug-free code


![jsx](https://miro.medium.com/max/1400/1*9zYuXj-zsH8cIOG7siEAww.png)

## **Rendering Elements**

To render a React element, first pass the DOM element to ReactDOM. CreateRoot, then pass the React element to root.

Even though we create an element describing the whole UI tree on every tick, only the text node whose contents have changed gets updated by React DOM.

![reactRender](https://res.cloudinary.com/practicaldev/image/fetch/s--mbs8xKqY--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/5uqd0mzte0iaa0p8lplt.png)



[Home](../README.md)
