# useReducer

## What is useReducer?
An alternative to useState. Accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method.source (Links to an external site.)

useReducer is a built in Hook in React is used to state management in React. useReducer is an alternative to useState. It is related to reducer functions. If you have clear idea about the Redux state management, then you already have enough knowledge how it works.

## Why we use useReducer over useState?
useState is used, when state values are primitives, state values are only used in a single component inside or logic is simple.

useReducer is used, when we have complex state like involves objects or arrays, next state is depend on previous one, data share among the components and update state more complex. useReducer is optimized performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

## How does the useReducer Hook work?
The useReducer Hook is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.

useReducer returns an array that holds the current state value and a dispatch function to which you can pass an action and later invoke it. While this is similar to the pattern Redux uses, there are a few differences.

For example, the useReducer function is tightly coupled to a specific reducer. We dispatch action objects to that reducer only, whereas in Redux, the dispatch function sends the action object to the store. At the time of dispatch, the components don’t need to know which reducer will process the action.

For those who may be unfamiliar with Redux, we’ll explore this concept a bit further. There are three main building blocks in Redux:

A store: An immutable object that holds the application’s state data A reducer: A function that returns some state data, triggered by an action type An action: An object that tells the reducer how to change the state. It must contain a type property and can contain an optional payload property