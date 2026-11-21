# Atlas Music — private builds

Sideload-only APKs of Atlas Music, kept here so they survive a rebuild of the
server. The source lives in the main Atlas-Music repository; this repo holds
release assets only.

Each GitHub Release carries one universal `app-release.apk`:

- signed with the **debug** keystore (no `android/key.properties` on the build
  machine), so it installs by sideload and cannot be used to update a build
  signed with a different key;
- built by `flutter build apk --release`;
- no source code is stored here — the APK is the artifact.
