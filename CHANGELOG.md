# Changelog

Published Driplist Android releases, newest first. Prereleases are marked explicitly.

## Driplist Android 1.3.0 (stable)

**Tag:** `v1.3.0`  
**Published:** 2026-11-13

Driplist Android 1.3.0 adds automatic checks for stable app updates.

- Checks the latest stable release when the app starts.
- Offers to download a newer signed APK and opens Android's installer after download.
- Android asks the user to confirm installation; sideloaded apps cannot update silently.
- If needed, Android asks the user to allow Driplist to open package installers in system settings.
- Includes pull-to-refresh and the existing Google sign-in, push notification, and keyboard layout improvements.
- Keeps the app ID and signing key unchanged. Install over the previous Driplist Android release.

This is the stable production release.

## Driplist Android 1.3.0-rc.3 (prerelease)

**Tag:** `v1.3.0-rc.3`  
**Published:** 2026-11-13

Driplist Android 1.3.0-rc.3 is a test build for prerelease update detection.

- An installed 1.3.0-rc.2 build should offer this newer prerelease at startup.
- Prerelease builds check for newer prereleases; stable builds check for newer stable releases.
- Offers to download the signed APK and opens Android's installer after download.
- Android asks the user to confirm installation; silent app updates are not available to sideloaded apps.
- Includes pull-to-refresh and the existing Google sign-in, push notification, and keyboard layout improvements.
- Keeps the app ID and signing key unchanged. Install over the previous Driplist Android release.

This is a prerelease test build. Install 1.3.0-rc.2 first to exercise the update prompt.

## Driplist Android 1.3.0-rc.2 (prerelease)

**Tag:** `v1.3.0-rc.2`  
**Published:** 2026-11-13

Driplist Android 1.3.0-rc.2 improves app update checks for both release channels.

- Prerelease builds check for newer prereleases at startup; stable builds check
  for newer stable releases.
- Offers to download a newer signed APK and opens Android's installer after download.
- Android asks the user to confirm installation; silent app updates are not
  available to sideloaded apps.
- If needed, Android asks the user to allow Driplist to open package installers
  in system settings.
- Includes pull-to-refresh and the existing Google sign-in, push notification, and keyboard layout improvements.
- Keeps the app ID and signing key unchanged. Install over the previous Driplist Android release.

This is a prerelease build with channel-aware update checking. Install it before
a later prerelease is published to exercise the update prompt; 1.3.0-rc.1 does
not yet check the prerelease channel.

## Driplist Android 1.3.0-rc.1 (prerelease)

**Tag:** `v1.3.0-rc.1`  
**Published:** 2026-11-12

Driplist Android 1.3.0-rc.1 adds automatic checks for stable app updates.

- Checks the public stable release when the app starts.
- Offers to download a newer signed APK and opens Android's installer after download.
- Android asks the user to confirm installation; silent app updates are not available to sideloaded apps.
- If needed, Android asks the user to allow Driplist to open package installers in system settings.
- Includes pull-to-refresh and the existing Google sign-in, push notification, and keyboard layout improvements.
- Keeps the app ID and signing key unchanged. Install over the previous Driplist Android release.

This is a prerelease build. Install it only if you want to preview the stable update prompt.

## Driplist Android 1.2.0 (stable)

**Tag:** `v1.2.0`  
**Published:** 2026-11-12

Driplist Android 1.2.0 adds pull-to-refresh to the mobile app.

- Pull down from the top of a page to reload the current Driplist page.
- Refresh is available when the page is at the top, and its native indicator
  stops when loading finishes or an error occurs.
- Includes the existing Google sign-in, push notification, and keyboard layout
  improvements.
- Keeps the app ID and signing key unchanged. Install it as an update over the
  previous Android release.

## Driplist Android 1.2.0-rc.2 (prerelease)

**Tag:** `v1.2.0-rc.2`  
**Published:** 2026-11-12

Driplist Android 1.2.0-rc.2 adds pull-to-refresh to the mobile app.

- Pull down from the top of a page to reload the current Driplist page.
- The native refresh indicator stops when loading finishes or an error occurs.
- Includes the existing Google sign-in, push notification, and keyboard layout
  improvements.
- Keeps the app ID and signing key unchanged. This is a prerelease and installs
  as an update over the previous Android release.

## Driplist Android 1.1.3 (stable)

**Tag:** `v1.1.3`  
**Published:** 2026-10-17

Driplist Android 1.1.3 fixes the remaining search/dialog bounce when opening
or minimizing the keyboard, following the partial improvement in 1.1.2.

- Removes the dialog's CSS size transition, which made its height trail the
  keyboard's viewport changes and briefly shift the dialog up or down.
- Preserves dialog opening/closing keyframe animations and input focus.
- Applies the correction before the page loads, with a fallback for older
  WebView providers.
- Includes the Google sign-in improvements and native push notifications from
  the previous releases.
- The existing app ID and signing key remain unchanged. Install this as an
  update over the previous Android release.

## Driplist Android 1.1.2 (stable)

**Tag:** `v1.1.2`  
**Published:** 2026-10-17

Driplist Android 1.1.2 fixes layout jumps when opening search or input dialogs
and when showing or hiding the keyboard.

- Keyboard insets are handled once, preventing duplicate viewport adjustments.
- The page follows the keyboard animation and restores its full height after
  dismissal, including when the keyboard is quickly reopened.
- Includes the Google sign-in improvements and native push notifications from
  the previous releases.
- The existing app ID and signing key remain unchanged. Install this as an
  update over the previous Android release.

## Driplist Android 1.1.1 (stable)

**Tag:** `v1.1.1`  
**Published:** 2026-10-16

Driplist Android 1.1.1 improves Google sign-in when Cloudflare browser challenges
are enabled. Sign-in now opens directly in Chrome Custom Tabs so the browser can
complete the challenge before returning to the app.

- Existing PKCE and one-time session handoff protections remain in place.
- Account linking continues inside the app.
- The existing app ID and signing key remain unchanged. Install this as an
  update over the previous Android release.

## Driplist Android 1.1.0 (stable)

**Tag:** `v1.1.0`  
**Published:** 2026-10-16

Driplist Android 1.1.0 adds native push notifications to the Android WebView app. It can receive vote, comment, and reply alerts through Firebase Cloud Messaging and open the related page when an alert is tapped.

- Android 13 and newer ask for notification permission after sign-in.
- Push notifications require server-side Firebase Cloud Messaging configuration.
- The existing app ID and signing key remain unchanged. Install this as an update over the previous Android release.

## Driplist Android 1.0.0 (stable)

**Tag:** `v1.0.0`  
**Published:** 2026-10-15

Driplist Android 1.0.0 is the stable production release for driplist.in. It
replaces the browser-backed Trusted Web Activity with a native Android WebView
shell. The site opens without browser controls, while Google login and Google
account linking run in the user's browser.

- Google login returns through a PKCE-bound, single-use handoff and creates a
  separate app session. New Google accounts can complete profile setup in-app.
- Added Android photo picking and system sharing for exported images.
- The existing app ID and signing key remain unchanged, so install this APK as
  an update over 0.2.1.
- Google login requires the matching website routes and database migration to be
  deployed on driplist.in first.
- Built without an emulator. Google login and device-specific behavior still
  need a phone test.

## Driplist Android 0.2.1 (prerelease)

**Tag:** `v0.2.1`  
**Published:** 2026-10-15

Driplist Android 0.2.1 is a prerelease for testing mobile authentication before production. It replaces the browser-backed Trusted Web Activity with a native Android WebView shell. The site opens without browser controls, while Google login and account linking run in the user's browser.

- Google login returns through a PKCE-bound, single-use handoff and creates a separate app session. New Google accounts can complete profile setup in-app.
- Added Android photo picking and system sharing for exported images.
- The existing app ID and signing key remain unchanged, so install this APK as an update over 0.2.0.
- Built without an emulator. Google login and device-specific behavior still need a phone test.

## Driplist Android 0.2.0 (prerelease)

**Tag:** `v0.2.0`  
**Published:** 2026-10-15

Driplist Android 0.2.0 replaces the browser-backed Trusted Web Activity with a
native Android WebView shell. The site opens without browser controls, while
Google login and Google account linking run in the user's browser.

- Google login returns through a PKCE-bound, single-use handoff and creates a
  separate app session. New Google accounts can complete profile setup in-app.
- Added Android photo picking and system sharing for exported images.
- The existing app ID and signing key remain unchanged, so install this APK as
  an update over 0.1.1.
- Google login requires the matching website routes and database migration to be
  deployed on driplist.in first.
- Built without an emulator. Google login and device-specific behavior still
  need a phone test.

## Driplist Android 0.1.1 (prerelease)

**Tag:** `v0.1.1`  
**Published:** 2026-10-15

Fixes an immediate startup crash affecting Android 14: Browser Helper's required
`ManageDataLauncherActivity` is now registered in the application manifest.

- Built and signed by GitHub Actions, with Android 14 JVM regression tests, lint, and signature verification.
- Uses the same package ID and signing key as 0.1.0, so install this APK as an update.
- Google login continues through your browser and the existing live Driplist website.

Download **driplist.apk** under Assets and open it on your phone. Android 7+ is supported.
Until `assetlinks.json` is deployed at `https://driplist.in/.well-known/assetlinks.json`,
a browser toolbar is expected. Google account sign-in still requires manual testing.
