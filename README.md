# Driplist Android releases

Official Android APK downloads and release history for Driplist.

## Download the latest stable version

[Download the latest stable APK](https://github.com/mr-mods-yg/driplist-android-releases/releases/latest).
The [Releases page](https://github.com/mr-mods-yg/driplist-android-releases/releases)
also lists prerelease builds.

## Install or update

1. Download `driplist.apk` from a release's Assets section.
2. Open the APK on your Android phone. If prompted, allow your browser or file
   manager to install apps.
3. Confirm the installation. Existing users can install it over their current
   Driplist app; keep the app installed so Android preserves its data.

Driplist Android supports Android 7 and newer and requires an internet
connection. It connects to [driplist.in](https://driplist.in). Google sign-in
is completed in your browser.

## Verify a download

Download `SHA256SUMS` from the same release and place it beside `driplist.apk`.
Then run:

```sh
sha256sum -c SHA256SUMS
```

On macOS, use `shasum -a 256 -c SHA256SUMS`.

## Release files

Each release includes the signed `driplist.apk`, its `SHA256SUMS`, build
metadata, and the Android signing certificate fingerprint record. The
[changelog](CHANGELOG.md) summarizes every published version.

Prereleases are marked on GitHub and may contain unfinished changes. For
regular use, install the latest stable release.

## About this repository

This repository contains public release downloads and release notes. It does
not contain the app's source code.

The Driplist Android application is distributed under the Apache License 2.0;
see [LICENSE](LICENSE).
