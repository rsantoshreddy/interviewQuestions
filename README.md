# Interview Questions

## Basic:

### 1. What is the difference between state and props?

 Both *props* and *state* are plain JavaScript objects. While both of them hold information that influences the output of render, they are different in their functionality with respect to component. Props get passed to the component similar to function parameters whereas state is managed within the component similar to variables declared within a function.

### 2. What are synthetic events in React?

`SyntheticEvent` is a cross-browser wrapper around the browser's native event. Its API is same as the browser's native event, including `stopPropagation()` and `preventDefault()`, except the events work identically across all browsers.

## Advanced

### 1. What is Redux and explain how it works?

Redux is an open-source JavaScript library used to manage application state. React uses Redux for building the user interface. 

React Redux is the official React binding for Redux. It allows React components to read data from a Redux Store, and dispatch Actions to the Store to update data. Redux helps apps to scale by providing a sensible way to manage state through a unidirectional data flow model. React Redux is conceptually simple. It subscribes to the Redux store, checks to see if the data which your component wants have changed, and re-renders your component.

To use react redux we have to wrap our app with React Redux Provider and component has to be wrapped with connect method. Connect method is a higher order component which takes two methods and the component itself. 

`e.g connect(mapStateToPrps, mapDispatchToProps)(Component);`
