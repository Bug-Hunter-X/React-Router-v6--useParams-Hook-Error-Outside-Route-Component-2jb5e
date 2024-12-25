# React Router v6 useParams Hook Error Outside Route Component

This repository demonstrates a common error encountered when using the `useParams` hook in React Router v6.  The `useParams` hook requires a routing context, which is only available within components rendered by `<Routes>` or route elements like `<Route>`.

Using `useParams` outside this context will lead to unexpected behavior or confusing error messages.  This example shows the problematic code and a solution to fix it.

## How to reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the error in the console and the broken application behavior.

## Solution

The solution involves ensuring that the component using `useParams` is a child of a `<Route>` component or is part of the component tree rooted at the `<Routes>` component.