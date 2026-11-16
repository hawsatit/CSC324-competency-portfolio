# 1.1 Medium-Scale Abstraction

**Artifact:** `useApi.js`

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

