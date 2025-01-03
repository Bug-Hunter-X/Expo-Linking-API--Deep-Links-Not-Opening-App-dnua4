# Expo Linking API: Deep Links Not Working

This repository demonstrates a common issue with Expo's Linking API where deep links fail to open the application or trigger the expected event listener.  The problem often stems from misconfigurations in `app.json` or incorrect handling of URL schemes within the application's code.

The `bug.js` file shows the problematic implementation, while `bugSolution.js` provides a corrected version.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Attempt to open a deep link (as specified in `bug.js` and `bugSolution.js`) in a web browser.  Observe the behavior in both the original and corrected versions.

## Solution

The solution involves carefully reviewing and correcting the URL scheme declaration within `app.json` and ensuring consistent handling of URL schemes within the application logic, specifically how the Linking API is used and how the scheme is handled in the app's URL handling code