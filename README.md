# React Redux JWT Demo

This is a simple React Native app demonstrating the usage of **Redux** for state management and **JWT (JSON Web Token)** for user authentication.

## Features

- Login screen where the user can enter a JWT token.
- Redux store to manage the token state.
- Home screen that decodes the JWT token (mock token used for demonstration).
- Logout functionality to clear the token from Redux state.

## Setup Instructions

### Prerequisites

1. **Node.js** installed (v14.x or later).
2. **React Native development environment** setup. If you don't have it set up, follow the instructions on the official React Native website: https://reactnative.dev/docs/environment-setup.

3. **Expo CLI** installed globally (optional but recommended):
   
   npm install -g expo-cli

## Steps to Run

1.  Clone this repository or create a new React Native project.

2. Install the necessary dependencies:

  npm install

3. If you're using Expo (recommended for simplicity):

  expo start

4. Alternatively, run the app directly with React Native:

  react-native run-android # for    Android

  react-native run-ios     # for iOS


## After the app launches, you will see the Login Screen. Enter a mock JWT token to test the login functionality. A sample JWT you can use:

  {
    
    "username": "DemoUser",
    
    "email": "demo@example.com"
  }

Example token (just base64 encoded for simplicity, use JWT libraries for real tokens):

```bash
eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6IkRlbW9Vc2VyIiwiZW1haWwiOiJkZW1vQGV4YW1wbGUuY29tIn0.SOME_RAND0M_SIGNATURE

``` 
After entering the token, you'll be directed to the Home Screen, where you will see a welcome message based on the decoded token. You can log out by clicking the Logout button.

## Notes
Dependencies worked on my local environment, but due to some issues with my setup, I used Expo.dev to run the app online.

## Dependencies
react-redux - State management.


redux - Redux core functionality.


jwt-decode - For decoding JWT tokens.
