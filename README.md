# MBBS Atlas 3D — Android Studio project

This is an Android Studio source project for a free MBBS anatomy/pathology learning app. It wraps the existing mobile-first Atlas 3D learning interface in a lightweight Android WebView shell.

## Current features
- Anatomy topics, search, quizzes, pathology learning cases and revision tools from `app/src/main/assets/index.html`.
- Label-friendly information panels in the included web app.
- 3D viewer is loaded from an external public viewer on demand; a working internet connection is required for that component.
- Android WebView enables JavaScript and local storage for quiz/revision state.

## Build an APK
1. Install Android Studio on a computer.
2. Open this `MBBSAtlasAndroid` folder as a project.
3. Allow Android Studio to download the Android Gradle Plugin and SDK components.
4. Choose **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
5. Find the debug APK under `app/build/outputs/apk/debug/`.

The project source is provided; an APK has **not** been built or tested in this environment because Android SDK/Gradle are not installed here.

## Important limitations
- The realistic 3D anatomy viewer is an external website, not bundled 3D assets. Its loading speed depends on internet connection, device, and the external viewer. The app shell itself is small, but cannot guarantee the external 3D viewer will be fast.
- This is an educational study aid, not a diagnostic tool. Verify medical details against your MBBS textbooks and faculty guidance.
- Z-Anatomy-derived models have CC BY-SA attribution/share-alike conditions and some referenced models have additional licence terms. This project links to the viewer instead of redistributing its model files. Review licences before bundling any model assets.
