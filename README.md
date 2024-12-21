# Expo CLI: Cannot find module error

This repository demonstrates a common error encountered when using the Expo CLI: the inability to find the main module due to issues within the `package.json` file.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides the corrected version. This issue usually arises from a missing or incorrect `"main"` field in `package.json`, causing the Expo CLI to fail during startup.

## How to Reproduce

1. Clone this repository.
2. Navigate to the directory containing `package.json` and `bug.js`.
3. Try running the project using `expo start`.  The error will be displayed.
4. Replace `bug.js` with `bugSolution.js` and run `expo start` again; the application should start successfully.

## Solution

The solution involves ensuring that the `"main"` field in `package.json` correctly points to the main entry point of your React Native application, usually `App.js` or `index.js`.