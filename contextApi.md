# Context API
Context provides a way to share data and state between components without having to explicitly pass a prop through every level of the tree.

Those values are normaly passed by what I like to call it props drilling; it is the way of passing state as props throug every level of the tree until we reach the desired component to deal with this data.

You can think of the context as a prodcast for the data and the functions and handlers associated with it.

## When to Use Context
Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.

Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

## how to create a context
At first, you will need to create a context, this is achievable by using the "React.createContext" method.

Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This default value can be helpful for testing components in isolation without wrapping them. Note: passing undefined as a Provider value does not cause consuming components to use defaultValue.

After that, we need to wrap everything in the app component inside a provider tag, inorder for all the wrapped components to be able to access the global state we called context.