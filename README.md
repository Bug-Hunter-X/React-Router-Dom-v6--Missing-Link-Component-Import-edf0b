# React Router Dom v6: Missing Link Component Import

This repository demonstrates a common, yet subtle, error in React Router v6: forgetting to import the `Link` component.  While the application might seem to render correctly, navigation between routes will fail silently unless this import is added.

## Bug
The bug lies in the `Home` component, where a `Link` component is used to navigate to the `/about` route without importing the component.

## Solution
Adding the missing `import { Link } from 'react-router-dom';` statement resolves this issue.  This ensures the `Link` component is correctly defined and allows for proper navigation within the application.
