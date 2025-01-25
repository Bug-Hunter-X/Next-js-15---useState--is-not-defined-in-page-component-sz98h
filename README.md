# Next.js 15: 'useState' is not defined in page component

This repository demonstrates a common error in Next.js 15 applications where the `useState` hook from React is used without being imported, leading to a runtime error.

## Problem

The `about.js` file attempts to use `useState` without importing `React`. This results in a runtime error because `useState` is not defined in the global scope.

## Solution

The `aboutSolution.js` file shows the corrected version. The `React` object is imported from `'react'`, making `useState` available.

## How to reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install`.
4. Run `npm run dev`.
5. Navigate to `/about` in your browser.  You'll see the error in the console.
6. Replace `about.js` with `aboutSolution.js` and re-run the dev server.  The error should be resolved. 

This example highlights the importance of correctly importing necessary modules in React components.