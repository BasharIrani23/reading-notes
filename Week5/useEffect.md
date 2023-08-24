# Component Lifecycle / useEffect Hook
## What is the main intended use case for the useEffect hook?
The useEffect hook's primary purpose is to handle side effects within functional components. This includes managing tasks that extend beyond rendering the user interface, such as connecting to external systems like APIs to fetch data.

## How does the effect’s logic interact with the component?
Once your component becomes part of the DOM, React executes your useEffect setup function. After each re-render involving changed dependencies, React triggers the cleanup function (if provided) with the previous values. Subsequently, it calls your setup function using the updated values. When your component is removed from the DOM, React initiates your cleanup function.

## What is the importance of the return value from the effect’s logic function?
The return value from the effect’s logic function serves the critical purpose of cleanup. This ensures that resources created by the effect are properly managed, preventing memory leaks or unintended behavior in your application. It's a fundamental aspect of maintaining the health and efficiency of your components.

