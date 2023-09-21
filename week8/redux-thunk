1. Why use Redux middleware?

Handle async actions.
Log actions and state changes.
Crash reporting.
Intercept and modify actions.
Manage side effects like API calls.
2. Redux Async Data Flow Diagram:

User interacts, triggering an action creator.
Action creator returns an async operation (like a function).
Middleware catches and executes the async operation.
After completion, middleware dispatches a new action with results.
Reducer updates store based on new action.
UI updates based on store changes.
3. Accommodating async in Redux:

Use middleware like redux-thunk.
Write async action creators.
Handle loading, success, and error states in your state.
Connect React components to the Redux store.
thunk middlewareLinks to an external site.

1-Why would you need redux-thunk middleware?

to handle asynchronous actions and side effects in Redux application

Redux Thunk middleware allows you to write action creators that return a ____ instead of an action.

return a function instead of an action. This function can perform asynchronous operations
Describe how any return value from the inner thunk function will be made available.

Any return value from the inner function will be available as the return value of dispatch itself
