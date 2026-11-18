# 2.1 Testing Dimensions

**Artifact:** Frontend mock tests — [`index.test.ts`](https://github.com/grinnell-csc324-fall-2026/recycling/blob/main/recycle-api/grinncycleFrontEnd/src/api/index.test.ts)

## Context and purpose

- This was intended to test that, if the data was successfully called, the frontend UI behaves like I wanted it to.
- These tests included:
  - **Search bar**
    - Pressing Enter or clicking Search opens the results. A blank search does nothing.
  - **Results page**
    - Shows loading, error, and "No results" messages, counts the results, and groups weaker matches.
  - **Results card**
    - Says Recyclable or Trash.

## Evidence of mastery

- **Testing strategies:** I used unit tests with mock data to test the API functions and React hooks. I also used React Testing Library to test how `useApi` handles asynchronous requests.
- **Normal behavior, edge cases, and failure conditions:** I tested normal searches, empty queries, different capitalization, and searches with no results. I also tested invalid item IDs and failed API requests to make sure errors are handled correctly.
- **Evidence that tests work:** I used `expect()` to check whether the actual results matched what I expected. I also tested whether `useApi` updates its loading state correctly and ignores old results when a new search is made. I also used React Testing Library to check whether `useApi` correctly handles loading data, successful requests, and errors.

## My contribution

I did the front end tests.

## Reflection

I thought this was pretty straightforward conceptually as well because it was similar to assert tests that I have done in the past. I learned how to use `test()` to define individual test cases and `async` and `await` test functions that return promises. I compared the return values with the expected results, such as checking whether an array contained the correct items. To test `useApi`, I wasn't sure what to do at first because I had never tested React hooks before. Claude used `renderHook` to test the hook without having to create an actual component. One thing I found interesting was testing whether `useApi` ignores old results when a new search is made. This helped me understand how testing React hooks is different from the unit tests I had done before.
