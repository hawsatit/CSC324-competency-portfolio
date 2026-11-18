# 2.2 Testing Infrastructure

**Artifact:** Front end test workflow on GitHub for pull requests — [`ci.yml`](https://github.com/grinnell-csc324-fall-2026/recycling/blob/main/.github/workflows/ci.yml)

## Context and purpose

- These tests run every time there is a pull request.

## Evidence of mastery

- These tests are automated into our GitHub workflow so they run with every pull request.
- We see the errors and are able to fix them before we merge.
- This prevents us from merging branches that produce errors.

## My contribution

I implemented the front end part of this workflow.

## Reflection

I've never used GitHub workflows before, and I think it's very useful, especially in a team, to set up tests so that we can automate verification before we make changes to the project that would impact the whole group. I think this part is very important to set up and make clear at the start with your team, to identify what parts need to be "correct" for the project. This experience helped me understand that testing infrastructure is not just about finding errors, but also about establishing a consistent development process that allows everyone to contribute without unintentionally breaking other parts of the project.
