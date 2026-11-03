# SizeKeeper

A private clothing size vault. Runs as a website/PWA and as an Android app.

## Where things live

The app itself is the files at the top of this repo:
`index.html`, `sw.js`, `manifest.json`, `sizekeeper-privacy.html`, and `icons/`.
That one copy is used for both the website and the Android app. There is no separate copy to keep in sync.

## Getting the Android app

1. Push (or upload) any change to `main` and GitHub builds the app automatically.
   You can also start it by hand: **Actions** tab > **Build SizeKeeper Android APK** > **Run workflow**.
2. Wait about 5 minutes, then open the finished run and download **SizeKeeper-debug-apk** under Artifacts.
3. Unzip it and send `app-debug.apk` to your Android phone.
4. Open it to install. The first time, Android asks you to allow installs from that app (Files, Chrome, etc.).

## Updating the app

Change the web files at the top of the repo and commit. A new APK builds on its own.
Each build gets a higher version number automatically.

## App details

| | |
|---|---|
| App name | SizeKeeper |
| App ID | `com.sizekeeper.app` (permanent once published to the Play Store) |
| Build type | Debug, for testing on your own phone |

## Publishing to the Play Store (later)

The Play Store needs a *signed release* build (an AAB), which needs a signing key.
That is a separate step; the debug APK above cannot be published.
