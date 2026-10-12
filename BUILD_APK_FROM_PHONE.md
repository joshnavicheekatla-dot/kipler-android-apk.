# Build the Kipler APK using only an Android phone

This project contains the Kipler HTML app packaged in a WebView Android project. The workflow builds a **debug APK** in GitHub Actions and provides it as a downloadable artifact. It is not yet a Play Store-signed release.

## Phone-only steps
1. Download and extract this ZIP on your phone. Keep the `.github/workflows/build-apk.yml` file and all folders/files.
2. In Chrome, open https://github.com/new and create a **public** repository named `kipler-android-apk` (public is the simplest way to use Actions without private-repository minute limits; do not upload personal secrets).
3. Upload the extracted project files/folders to the repository root. Make sure `.github/workflows/build-apk.yml` is included. GitHub's mobile upload UI may be awkward; if it cannot upload folders, use a desktop browser mode or a trusted repository-upload method. Do not upload the ZIP itself as the only repository file.
4. Open the repository's **Actions** tab and choose **Build Kipler APK**. If GitHub asks, enable Actions. Run workflow if the workflow did not start automatically.
5. Wait for the workflow to finish. Open the completed run, scroll to **Artifacts**, and tap **Kipler-Android-APK** to download the artifact ZIP.
6. Extract that artifact ZIP. It contains `app-debug.apk`. Tap it to install; Android may ask you to allow installs from that source. Only install APKs you built from a source you trust.

## Important
- This is a **debug APK for testing**, not a signed Play Store release.
- The Android camera/photo picker must be tested on a real device.
- A successful cloud build has not been run yet. The APK will exist only after GitHub Actions succeeds.
- For Google Play, build and sign an Android App Bundle (AAB) with a private signing key; do not publish the debug APK.
