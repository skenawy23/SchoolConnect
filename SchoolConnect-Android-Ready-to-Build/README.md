# SchoolConnect demo (Android)

A thin Android wrapper around the clickable SchoolConnect prototype (all 53 screens, English and Arabic).
The prototype is bundled in `app/src/main/assets/index.html`, so the app works offline.

## Get the APK (no Android Studio needed)
1. Create a new empty repository on GitHub and upload everything in this folder
   (including the hidden `.github` folder).
2. Open the repository's **Actions** tab. The "Build APK" workflow starts by itself
   (or choose Run workflow).
3. When it turns green (about 3 to 5 minutes), open the run and download **SchoolConnect-APK**.
4. Unzip it and copy `app-debug.apk` to the phone, then open it.
   Android will ask you to allow installing from this source.

## Or build locally
Install Android Studio, choose Open, pick this folder, then Build > Build APK(s).

This is a debug-signed demo build for review, not a Play Store release.


## Build status
This project has NOT been compiled yet (the authoring sandbox cannot reach Google/Maven/Gradle servers).
Fastest route to an APK: push this folder to a GitHub repo -> Actions tab -> "Build APK" -> download the
`SchoolConnect-APK` artifact (app-debug.apk). Or open in Android Studio (Jdk 17) and run Build > Build APK(s).
Output path after a local build: app/build/outputs/apk/debug/app-debug.apk

## Upload to GitHub (no command line needed)
1. Create a new repository on github.com (private is fine).
2. Click "uploading an existing file" and drag in ALL the contents of this folder, including the hidden `.github` folder
   (unzip first; do not upload the zip itself). The files `settings.gradle` and `.github/workflows/build-apk.yml` must sit at the repository root.
3. Open the Actions tab. "Build APK" starts automatically on upload; you can also press "Run workflow".
4. When it turns green, open the run and download `SchoolConnect-APK` under Artifacts. Unzip it to get app-debug.apk.
