# Uncaught Error in React Native useEffect Cleanup

This repository demonstrates a common but difficult-to-debug issue in React Native: an uncaught error thrown within the cleanup function of a `useEffect` hook.  The example uses an asynchronous operation (simulated here) with a subscription that might be unsubscribed multiple times, leading to an error.

The `useEffectBug.js` file showcases the problematic code.  The solution, presented in `useEffectSolution.js`, demonstrates how to handle potential errors within the cleanup function to prevent crashes and improve the application's stability.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run the application using your preferred React Native method (e.g., `npx react-native run-android` or `npx react-native run-ios`).
4. Observe the console for error messages (or lack thereof) with the initial example and then the solution.