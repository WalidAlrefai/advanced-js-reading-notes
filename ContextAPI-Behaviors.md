# Context API - Behaviors

## Why Context API and what is it?
The React Context exist so you don’t have to pass in data manually at every level. Context is about sharing data to many components. The reason we need the Context API is that it’s cumbersome to pass data from parent to child via props if there are many components requiring the same data. By using the Context API we no longer pass this kind of shared data with props.

## When to use /not use it
Things that belong in a context is data that is considered global like a user or a cart etc. So let’s try to list the different reasons for using a Context:

- data needed in many places , data that needs to be used by many components like a theme, user or a cart
- pass props through many components , sometimes it’s better to use composition over context when you want to pass 
a props value through many components

### Building blocks and API
The Context API consists of some building blocks that it is important that we know about what they are called but also what their role is:

- **context** , the context object is an object holding the current context value and can be subscribed to
- **provider** , This is a React component that provides the value in question, it grabs it from the context object
- **consumer** , This is a React component that is able to consume the value provided by the Provider and is able to show the value

This is all a bit theoretical and may sound a little confusing so let’s dive right into an example to clear any confusion.

## Context API in action
To utilize a Context in React we need to do the following:

create a context , we do this with a call to React.createContext(), this will return a Context object that exposes a Provider Component as well as a Consumer Component
declare a provider , this is us grabbing the Provider Component reference available in the context object we just created
declare a consumer , this is also a component that lives on the Context object and we use this to show the value to the user