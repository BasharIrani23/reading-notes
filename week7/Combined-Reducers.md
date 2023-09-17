# Multiple Reducers Example

### 1- Why create multiple reducers?

- Modularity: For large applications, it's easier to manage, understand, and maintain state logic when it's split into smaller, domain-specific reducers.
- Separation of Concerns: Each reducer can focus on a specific slice of the state, making the logic clear and concise.

### 2- How would you combine multiple reducers?

Use combineReducers from the Redux library. It allows you to merge multiple reducer functions into a single reducing function. Each reducer will manage its own part of the global state.

### 3- How will you manage state as an immutable object? Why?

- How: By never directly modifying the state. Instead, always return a new copy of the state with any changes. Common utilities include the spread operator (...), Object.assign(), or libraries like Immutable.js.
- Why: Ensures predictability, traceability, and helps with debugging and optimization (e.g., with PureComponent and memoization). Immutable state changes also allow for time-travel debugging and consistent behavior in your application.

*** 
# Redux Docs: Using Combined Reducers
### 1- combineReducers is a utility function to simplify the most common use case when writing ___ _____ *Redux reducers* 

Explain how combineReducers assembles the new state tree.

### 2-Explain how combineReducers assembles the new state tree.

Answer: combineReducers takes an object where each key corresponds to a specific "slice" of the state, and each value is a reducer function responsible for managing that slice. When an action is dispatched, combineReducers calls each of these slice reducers with the current slice of state and the dispatched action. Each slice reducer returns a new state (or the existing state if no changes are necessary). combineReducers then combines these slices into a single state object, which becomes the new state of the store.




### 3-How would you define initial state in an app using combineReducers?

Answer: There are two primary methods to define the initial state when using combineReducers:

Through Initial Values in Reducers: Each slice reducer can provide its own initial state by checking if the incoming state is undefined and returning the default state value for that slice.

Using preloadedState with createStore: When you create the Redux store using createStore, you can provide a second argument called preloadedState. This is particularly useful for initializing the store with state that was previously persisted elsewhere, such as server-side rendering or from local storage.

***

# Redux Docs: Combined Reducer Syntax



### 1-Why will you want to split your reducing functions as your app becomes more complex?
As your app grows more complex, splitting reducing functions helps in organizing and managing different parts of the state independently, making the codebase more maintainable and understandable.

### 2-The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.
 The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

### 3-What is a popular convention when naming reducers?
A popular convention is to name reducers after the state slices they manage, so you can use ES6 property shorthand notation. For instance, using combineReducers({ counter, todos }) is equivalent to writing combineReducers({ counter: counter, todos: todos }).


