# 1-What is the first principle of Redux?
The first principle of Redux is that the entire application state is stored in a single immutable object called the "store."
# 2-what is a store and what do we use our reducers for within that store?
A store in Redux is a container that holds the entire application state. Reducers are used within the store to specify how the state should be updated in response to actions.
# 3-Name three Redux store methods given to us by createStore and describe their use.

- getState(): Returns the current state stored in the Redux store.
  
- dispatch(action): Dispatches an action to trigger a state change.
  
- subscribe(listener): Adds a listener function that will be called whenever the state in the store is updated.

# 4-Explain to a non-technical recruiter what combineReducers() does and why it is useful.
combineReducers() is a Redux utility function that combines multiple reducer functions into a single reducer. It is useful because it allows you to split your state management logic into smaller, more manageable pieces, each handled by a separate reducer function. This separation of concerns makes it easier to maintain and scale your Redux application.
