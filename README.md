# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router Dom v6. The catch-all route unintentionally overrides all other defined routes. 

## Problem
The provided `App.js` demonstrates how a catch-all route (`/*`) in `react-router-dom` v6 can incorrectly match all routes instead of only those that don't match any other routes. This leads to only the `NotFound` component being rendered regardless of the URL.

## Solution
The `AppSolution.js` file presents a solution by ensuring that the catch-all route is placed last within the routes array and that more specific routes are prioritized. This fixes the unintended behavior.