# Redux Toolkit (RTK)

### 1-What concerns are addressed by Redux Toolkit?
Redux Toolkit was created to address three common concerns about Redux:

- "Configuring a Redux store is too complicated."
= "I have to add a lot of packages to get Redux to do anything useful."
= "Redux requires too much boilerplate code."

### 2-What does configureStore() do?
configureStore() is a function that wraps Redux's createStore method to provide simplified configuration options and better defaults. Specifically, it:

Can automatically combine your slice reducers.
Adds any Redux middleware you supply.
Includes redux-thunk by default.
Enables use of the Redux DevTools Extension.

### 3-How would I use createSlice()?
createSlice() is used to automatically generate a slice of the Redux store, along with its corresponding action creators and action types. To use it:

You provide an object of reducer functions, a slice name, and an initial state value.
The function will then automatically generate a slice reducer, corresponding action creators, and action types.
***
# MobX

### 1-What is MobX?
MobX is a battle-tested library that makes state management simple and scalable by transparently applying functional reactive programming (TFRP). It is mainly used with JavaScript and TypeScript, and it's especially popular with React applications. The primary idea behind MobX is that almost everything can be derived from the application state, automatically, using reactions that automatically update when relevant state changes.
### 2-How does MobX make it “impossible” to produce an inconsistent state?
MobX enforces a clear distinction between actions that update state and computations that derive information from the state.

### 3-How would we build a reactive user interface?
Building a reactive user interface with MobX generally involves the following steps:

-Define Observable State: Use MobX’s observable to create reactive state variables. These variables will automatically notify any derivations (like computed values or reactions) when they change.


*class TodoStore { @observable todos = []; }*


- Create Computations: If you have state that can be derived from other state, use computed to define it. This will create a value that automatically updates when its dependencies change.

*class TodoStore {  @observable todos = [];*
  
*@computed get unfinishedTodoCount() {*
*return this.todos.filter(todo => !todo.finished).length;*
  
  
- Build React Components: If using React, components can react to state changes by marking them with the observer function/decorator from mobx-react. This makes the component re-render whenever observable state it relies on changes.

import { observer } from 'mobx-react';

const TodoListView = observer(({ todoStore }) => (
  <div>
    {todoStore.todos.map(todo => <div key={todo.id}>{todo.text}</div>)}
  </div>
));


- Update State with Actions: State should be modified using actions. This makes state changes more predictable and structured.


class TodoStore {
  @observable todos = [];

  @action addTodo(text) {
    this.todos.push({ id: Date.now(), text: text, finished: false });
  }
}

- React to State Changes: You can use MobX’s autorun, when, or reaction to create side effects that run in response to state changes. For instance, you could save to local storage whenever a particular piece of state changes.
