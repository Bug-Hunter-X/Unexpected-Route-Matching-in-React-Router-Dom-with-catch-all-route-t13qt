# React Router Dom Unexpected Route Matching Bug

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in `react-router-dom`. The catch-all route unintentionally overrides other routes, leading to unexpected routing behavior.  The solution shows how to correctly order routes to avoid this problem.

## Bug Description
The problem occurs when a catch-all route (`/*`) is placed before more specific routes.  React Router will match the catch-all route first, preventing other, more specific routes from ever being matched.  This results in the catch-all component rendering even when a more specific path should be matched.

## Solution
The solution involves correctly ordering the routes. More specific routes should always be declared before catch-all routes to ensure that they are matched correctly. 