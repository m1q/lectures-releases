# Lectures Dark — releases

Download the latest **LecturesDark.apk** from [Releases](https://github.com/m1q/lectures-releases/releases/latest) and open it on your Android phone (Android 8 or newer).

After installing, the app updates itself: when a new version is published here it shows **Update available** on the Today screen. Tap it, then confirm Android's prompt. Your group and settings are kept.

The timetable itself comes from [m1q/lectures-timetable](https://github.com/m1q/lectures-timetable).

## For maintainers

`latest.json` tells installed apps which version is newest. Don't edit it by hand. Publish with `android/release.sh` from the (private) app repository, which builds and signs the APK, creates the GitHub release and updates `latest.json`.

The app only installs APKs from this repository's release downloads whose SHA-256 matches `latest.json`, and Android only accepts them when they're signed with the original key.
