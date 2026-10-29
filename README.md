# Sigurado for Android

Sigurado keeps the laboratory stockroom secure with fingerprints: a scan at the door times you
in, a scan at the cabinet unlocks it, and every borrow and return is recorded against the person
who opened it. The app shows your time-ins, what you have borrowed, and notifications as they
happen.

This repository only hosts the **Android app downloads and updates**. The website is at
[sigurado-lab.vercel.app](https://sigurado-lab.vercel.app).

## Download

| | |
|---|---|
| **Newest release page** | [Latest release](https://github.com/adam-ctrlc/sigurado-releases/releases/latest) |
| **All releases** | [Releases](https://github.com/adam-ctrlc/sigurado-releases/releases) |
| **Requirements** | Android 7.0 or newer |

Not every release contains an APK: most updates are delivered inside the app (see
[Updates](#updates)). To install Sigurado for the first time, use the newest release that lists a
`sigurado-vX.Y.Z.apk` file under **Assets**.

## Install

1. On your Android phone, open the newest release that has an APK and tap the `sigurado-vX.Y.Z.apk` file.
2. When the download finishes, tap the file to open it.
3. The first time, Android asks to allow installs from your browser. Tap **Settings**, switch on
   **Allow from this source**, then go back and tap **Install**.
4. Open Sigurado and sign in with your account, or create one and wait for an admin to approve it.

## Updates

Sigurado checks for a new version every time you open it. Updates are required: when one is out,
an **Update required** screen lists what's new.

- **Most updates download inside the app.** Tap **Update now**, wait a few seconds, and Sigurado
  restarts on the new version. Only the changed files are downloaded, with no reinstall.
- **Occasionally a new app version (APK) is needed**, when Android-level parts of the app change.
  The update screen then offers a **Download** button for the new APK; install it over the old one.

If a new version ever fails to start, Sigurado goes back to the last version that worked by itself.

## What's in a release

- `latest.json`: what the app reads to find updates (version, release notes, file list).
- `f-<hash>` files: the app's files, each named by its content hash, so phones only download
  what changed.
- `sigurado-vX.Y.Z.apk`: the Android app, on releases that need one.
