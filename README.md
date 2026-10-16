# SafeTrack

Flutter starter project for SafeTrack. The current app is the Flutter counter
demo, with a widget test that checks the increment button. Tracking features
have not been implemented yet.

## Run locally

Install the [Flutter SDK](https://docs.flutter.dev/install), then run:

```sh
git clone https://github.com/antonykiragundirangu/safetrack.git
cd safetrack
flutter pub get
flutter run -d chrome
```

The automated checks use Flutter 3.44.8. Run `flutter doctor` to check your local
toolchain and `flutter devices` to list available targets. Android, iOS, desktop,
and web platform folders are included; native builds require their platform
toolchains and have not been validated by the checks below.

## Check changes

```sh
dart format --output=none --set-exit-if-changed lib test
flutter analyze
flutter test
```

GitHub Actions runs these checks for pull requests and pushes to `main`. Start
each improvement on a branch and open a pull request with a description of the
change and its test results.

Local SDK paths, build output, environment files, and signing credentials are
excluded from Git. Commit `pubspec.lock` when dependency resolution changes so
other contributors can use the same package versions.
