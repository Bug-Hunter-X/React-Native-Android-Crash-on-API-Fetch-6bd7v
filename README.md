# React Native Android Crash on API Fetch

This repository demonstrates a bug where a React Native application crashes on Android when fetching data from a remote API. The iOS version works without issue. The error is not caught within the try-catch block, leading to the crash.

## Bug Description

A React Native application using `fetch` to retrieve data from an API crashes on Android.  The error is not caught within the try...catch block, and no specific error message is provided in the logs, making debugging difficult. The iOS version functions correctly.

## Reproduction

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app on an Android emulator or device.
4. Observe the crash when the app attempts to fetch data.

## Solution

The solution involves improved error handling, specifically considering potential network issues on Android.  See `bugSolution.js` for a corrected implementation.