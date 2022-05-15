# Context API - Behaviors

Before You Use Context

CreateContext o Context. Consumer o Context.

React components, such as the current authenticated user, theme, or preferred language. This can become painful // if every single button in the app needs to know the theme // because it would have to be passed through all components. // Create a context for the current theme . // Any component can read it, no matter how deep it is.

// In this example, we're passing «dark» as the current value. return // A component in the middle doesn't have to// pass the theme down explicitly anymore. // React will find the closest theme Provider above and use its value. // In this example, the current theme is «dark».

With this change, only the top-most Page component needs to know about the Link and Avatar components’ use of user and avatarSize. You’re not limited to a single child for a component.

Context lets you «broadcast» such data, and changes to it, to all components below. Common examples where using context might be simpler than the alternatives include managing the current locale, theme, or a data cache.

API

CreateContext const MyContext = React. The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This default value can be helpful for testing components in isolation without wrapping them. The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers.

>All consumers that are descendants of a Provider will re-render whenever the Provider’s value prop changes.

[React resources](https://github.com/diegohaz/awesome-react-context)


[Home](../README.md)