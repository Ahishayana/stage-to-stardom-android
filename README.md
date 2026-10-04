# Stage to Stardom: Android app

This folder is a complete Android project. It wraps the game in a full-screen app with its own icon,
saves your careers on the phone, supports the Android back button, and stays in portrait mode.

## Build the APK for free on GitHub (no installs needed)

1. Create a free account at github.com and click **New repository**. Name it `stage-to-stardom` and create it.
2. On the new repository page, click **uploading an existing file**. Drag in **everything inside this
   folder**, including the hidden `.github` folder. Click **Commit changes**.
   - If your computer hides the `.github` folder, use **Add file → Create new file** instead, name it
     `.github/workflows/build-apk.yml`, and paste in the contents of that file.
3. Open the **Actions** tab. A build called **Build APK** starts on its own (about 5 minutes).
   If it does not, click **Build APK → Run workflow**.
4. When it shows a green tick, open the build and download **StageToStardom-APK** under **Artifacts**.
   Unzip it to get `app-debug.apk`.

## Install it on your phone

1. Copy `app-debug.apk` to your phone (or download it there directly).
2. Tap it. Android will ask you to allow installs from this source: allow it, then tap **Install**.
3. Stage to Stardom appears in your app drawer.

## Alternative: Android Studio

Install Android Studio, choose **Open**, and select this folder. Wait for it to finish syncing,
then use **Build → Build App Bundle(s) / APK(s) → Build APK(s)**.

## Updating the game later

Replace `app/src/main/assets/index.html` with a newer version of the game file, raise `versionCode`
in `app/build.gradle`, and build again. Install the new APK over the old one to keep your saves.
