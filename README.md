# GolGappe Date: APK build
Not built or tested by the author. The workflow is written to produce a debug APK.

## Easiest: build in the cloud (free)
1. Create a new GitHub repository and upload everything in this folder (keep the .github folder).
2. Open the Actions tab, run "Build APK" (it also runs on every push).
3. When it finishes, download the artifact "golgappe-date-apk", unzip it, and copy app-debug.apk to your phone.
4. Open it and allow "install unknown apps" when asked.

## Or build locally
Needs Node 20, JDK 17 and Android Studio.
npm install; npx cap add android; npx cap sync android; npx cap open android
Then Build > Build APK(s).

This is an unsigned debug APK for personal sideloading. Publishing to Google Play needs a signed release build.
