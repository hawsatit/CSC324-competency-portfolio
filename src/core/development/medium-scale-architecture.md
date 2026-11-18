# 1.2 Medium-Scale Architecture

**Artifact:** Different pages in the front end — [`HomePage.tsx`](https://github.com/grinnell-csc324-fall-2026/recycling/blob/main/recycle-api/grinncycleFrontEnd/src/pages/HomePage.tsx)

## Context and purpose

- Main parts of the front end are routes and pages.
- This separates responsibilities, with pages being responsible for the content of a particular screen.

## Evidence of mastery

- I implemented a page-based, component-oriented structure.
- Each page has a clear job, and reusable components handle common interface elements. Data loading is kept separate from presentation through the API functions and `useApi`.
- They support the project's main user needs: searching for recycling guidance, viewing details for an item, and finding recycling centers.

## My contribution

This was done on the front end.

## Reflection

This concept was pretty straightforward to me conceptually, but I didn't really know how to implement the navigation between pages. I learned how routing allows different pages to be displayed without reloading the entire application. I learned how each page can have its own path, e.g. `/search` for `ResultsPage` and `/centers` for `CentersPage`. I also learned how dynamic routes work, such as `/items/:id`, which allows the same `ItemPage` component to display different items based on their IDs. `useNavigate` allows me to redirect users to another page after an action, like submitting a search, without reloading the entire website. I also learned how to pass information through the URL with parameters, e.g. `/search?q=plastic`, so that the `ResultsPage` can retrieve the search query and display the appropriate results. Lastly, I learned how shared components like `Navbar` can be placed outside `Routes` so they appear on every page.
