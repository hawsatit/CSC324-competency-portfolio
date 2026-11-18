# 1.1 Medium-Scale Abstraction

**Artifact:** [`useApi.ts`](https://github.com/grinnell-csc324-fall-2026/recycling/blob/main/recycle-api/grinncycleFrontEnd/src/api/useApi.ts)

## Context and purpose

- React hook for loading data and keeping track of whether the request is still running, succeeded, or failed.
- Takes in `load`, which is a function (e.g., in `ResultsPage`, it uses `searchItems(query)`).
- Takes in `key`, which is a value identifying what's being loaded (e.g., the search query when using `searchItems`).
- Every time the key changes, the load runs again.

## Evidence of mastery

- Combines the common steps of loading data and tracking its state.
- It hides the details of making an asynchronous request and tracking its state (data, error, and loading).
- Takes in `load` and `key`, giving components a consistent way to work with different requests.
- It's a custom React hook, which packages reusable stateful behavior.

## My contribution

This was part of the front end.

## Reflection

This was mostly vibe coded with Claude because I wasn't familiar with how to do API calls and how to make this abstract. At first it was pretty hard to understand `useState` and `useEffect`, and how they are used to manage state and respond to changes in dependencies. I learned that React can automatically update components when state changes, rather than having to manually update the UI. I now have a better understanding of how common functionality can be abstracted into reusable components and hooks. The `useApi` hook showed how different parts of an application can share the same logic for loading data and handling errors without repeating code. This helped me understand the importance of abstraction in making code more organized, maintainable, and easier to reuse.
