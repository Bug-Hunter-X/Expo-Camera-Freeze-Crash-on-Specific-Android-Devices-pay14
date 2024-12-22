# Expo Camera Freeze/Crash on Android

This repository demonstrates a bug in the Expo Camera API that causes the camera preview to freeze or crash on certain Android devices.  The issue appears to be related to hardware/driver incompatibility and lacks consistent error messages, making debugging challenging.

## Bug Description

The camera preview intermittently freezes or causes the app to crash.  No specific error message is consistently reported.  The issue occurs sporadically and appears dependent on the Android device used.

## Reproduction Steps

1. Clone this repository.
2. Run the app using Expo Go on an affected Android device (specific devices prone to this issue are noted in the `cameraBug.js` file comments).
3. Observe the camera preview. The freeze/crash may occur after varying periods of operation.

## Solution

The solution involves adding error handling and potentially fallback mechanisms. While a complete fix is device-specific and relies on improved driver compatibility, we can improve the user experience by gracefully handling potential crashes and providing more informative feedback.

See `cameraBugSolution.js` for the improved implementation.