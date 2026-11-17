# Hello Android

A small Flutter Android app used to verify CRA's Android build and observable
behavior checks on a real device. Its core task is tapping `+` and seeing the
counter increase.

## Check the app

From this repository root, with Flutter and an Android SDK installed:

```powershell
flutter pub get
flutter test --no-pub
flutter build apk --release --no-pub
```

The release APK is written to `build/app/outputs/flutter-apk/app-release.apk`.
With an authorized Android phone connected, install and launch it using the
package `com.example.hello_android`. Verify the counter changes from 0 to 1
after tapping `+`.

The release variant currently uses Flutter's debug signing configuration for
local device checks. This repository does not declare a public app release.
