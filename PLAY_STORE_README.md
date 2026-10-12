# Kipler Mathematics and Statistics — Android / Play Store Package

Prepared as an Android Studio WebView project around the current Kipler HTML app.

Package name: com.kipler.mathematics
Version: 1.0.0 (versionCode 1)
Target SDK: 35

Included:
- Current Kipler Mathematics and Statistics web app in app/src/main/assets/index.html
- Android launcher activity
- Camera and microphone permissions for the app's Camera/Voice features
- Portrait orientation
- Android Studio Gradle configuration
- Basic launcher icon

Build:
1. Open this folder in Android Studio.
2. Let Gradle sync and install the Android SDK required by compileSdk 35.
3. Test on a physical Android device.
4. Build > Generate Signed App Bundle / APK.
5. For Google Play, generate a signed Android App Bundle (.aab), not just an APK.
6. Upload the signed .aab in Google Play Console and complete the store listing, Data safety, content rating, privacy policy and testing requirements.

Important:
- This package is prepared for publication but has NOT been uploaded to Google Play.
- A Play Console developer account and a valid signing key are required.
- Before production release, verify camera/microphone behavior and all third-party/browser links on a physical device.
