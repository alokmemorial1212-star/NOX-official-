# NOX — The Unknown Organization (Android source project)

A dark-themed Android case-file manager with local SQLite storage.

## Features
- Create, edit and delete case records
- Case number/name, victim, crime place, status, culprit, summary and closed-on date
- Search across case number, name, victim and place
- Filter by All / Active / Pending / Solved
- Status stamps: CLOSED / ACTIVE / PENDING
- Data stays locally on the device in SQLite

## Build
1. Install Android Studio (current stable) on a computer.
2. Open this folder as an existing project.
3. Allow Gradle sync and install the Android SDK Platform 35 if prompted.
4. Connect an Android phone with USB debugging enabled, or use an emulator.
5. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.

The APK is normally created at `app/build/outputs/apk/debug/app-debug.apk`.

## Important
This ZIP contains Android source code, not a compiled or tested APK. Build it in Android Studio before installing. The database starts empty intentionally: historical case details have not been fully verified, so no missing case information is fabricated.
