### Summarize the five principles for structuring state.
- Group Related State: This principle encourages combining state variables that frequently change together into a single state variable to enhance organization and coherence.
- Avoid State Contradictions: Ensure that the state's structure doesn't lead to conflicting or contradictory information, reducing the potential for errors.
- Prevent Redundant State: If data can be computed from component props or existing state during rendering, avoid storing it redundantly in the component's state.
- Minimize State Duplication: Reduce the occurrence of identical data across multiple state variables or nested objects to prevent synchronization complexities.
- Simplify State Nesting: Keep the state structure relatively flat instead of deeply hierarchical, as deeply nested state can be challenging to update and manage efficiently

### Problem Solved by Contexts: Contexts address the issue of passing data from a parent component to deeply nested child components without the need to explicitly pass it through props at every level. They make information available to any component within a specific subtree, regardless of its nesting depth.


### Technique before useContext: One technique to consider before using useContext is "prop drilling," where data is passed as props from a parent component to its child components and potentially further down the tree. However, this can become verbose for complex scenarios.


### Hook Complementing useContext for Complex Applications: In complex applications, the useReducer hook can complement useContext. It allows for managing complex state in React applications and can be combined with context to provide a central place for managing and distributing state to components throughout the application. Other hooks may also be useful in different situations.
