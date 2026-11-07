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
3. Allow Gradle sync and install the - name: Install Android SDK
  run: |
    export ANDROID_HOME=/usr/local/lib/android/sdk
    export ANDROID_SDK_ROOT=$ANDROID_HOME
    yes | $ANDROID_HOME/cmdline-tools/16.0/bin/sdkmanager --sdk_root=$ANDROID_HOME --licenses
    $ANDROID_HOME/cmdline-tools/16.0/bin/sdkmanager --sdk_root=$ANDROID_HOME "platforms;android-35" "build-tools;35.0.0" "platform-tools" Platform 35 if prompted.
4. Connect an Android phone with USB debugging enabled, or use an emulator.
5. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.

The APK is normally created at `app/build/outputs/apk/debug/app-debug.apk`.

## Important
This ZIP contains Android source code, not a compiled or tested APK. Build it in Android Studio before installing. The database starts empty intentionally: historical case details have not been fully verified, so no missing case information is fabricated.
