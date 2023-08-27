# Advanced State with Reducers
1- What is the motivation for adding a reducer?

To reduce this complexity and keep all your logic in one easy-to-access place. The motivation for adding a reducer is to allow you to manage state in a more controlled and predictable way, especially when state updates involve complex logic.

2- What are actions in the context of a reducer? How are they different from setting state directly?

Instead of telling React “what to do” by setting state, you specify “what the user just did” by dispatching “actions” from your event handlers. The useReducer Hook is similar to useState—you must pass it an initial state and it returns a stateful value and a way to set state (in this case, the dispatch function). But it’s a little different.

The useReducer Hook takes two arguments:

A reducer function
An initial state
And it returns:

A stateful value
A dispatch function

3- What common list operation is useReduce named for, and why?

Although reducers can “reduce” the amount of code inside your component, they are actually named after the reduce() operation that you can perform on arrays. The name "useReducer" comes from the idea of combining actions in a similar way that you combine items in a list using the "reduce" operation. Just like "reduce" combines values to get a single result, useReducer combines actions to get a new state.

4- When should you switch from useState to useReducer?

If state management requirements become more complex, involve shared logic, or require better predictability, switching to useReducer. You should switch from useState to useReducer when your component's state management becomes complex or involves multiple interacting state values.
