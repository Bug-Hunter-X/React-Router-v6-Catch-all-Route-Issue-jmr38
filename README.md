# React Router v6 Catch-all Route Bug

This repository demonstrates a bug encountered with the catch-all route ("*") in React Router v6.  The `NotFound` component, intended to handle all non-matching routes, does not render as expected.  This issue arises despite other routes within the same `Routes` component working correctly.

## Bug Description

The `App.js` file contains a simple React application using `react-router-dom` v6.  Routes for '/' and '/about' work correctly. The catch-all route path="*" however, fails to display the `NotFound` component when navigating to a URL that doesn't match any other defined routes.

## Solution

The solution is provided in `AppSolution.js` and highlights how to correctly implement a catch-all route. The key was to ensure the catch-all route is placed as the last route in the `Routes` component.