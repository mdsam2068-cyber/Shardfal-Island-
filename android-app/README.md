# Shardfall Isle Android wrapper

This Android project wraps the Shardfall Isle web game in a WebView app for APK packaging.

## What it does
- Loads the live GitHub Pages version by default.
- Tries to load bundled local HTML if `assets/index.html` is added.
- Falls back gracefully if the network is unavailable.

## Build in Android Studio
1. Open `android-app/` in Android Studio.
2. Let Gradle sync.
3. Choose `Build > Build Bundle(s) / APK(s) > Build APK(s)`.
4. The generated APK will be under `app/build/outputs/apk/debug/` or `release/`.

## Best possible setup
For the best offline experience, copy the generated static game files into `android-app/app/src/main/assets/` and name the main file `index.html`. Then the app will load locally without internet.

## Live game URL
https://mdsam2068-cyber.github.io/Shardfal-Island-/
