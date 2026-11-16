# VICORA SMS Intelligence — Public Releases

This repository is the public update channel for **VICORA SMS Intelligence**.

The application source code is maintained separately in a private repository. This repository contains only public release notes and signed Android release packages.

## Release asset contract

Every stable release must be published as a GitHub Release with:

- A semantic version tag, for example `v1.0.1`.
- One release APK named `vicora-sms-intelligence-v1.0.1-release.apk` (replace the version).
- A `SHA256SUMS.txt` asset containing the APK SHA-256 checksum in standard format:
  ```text
  <64-character-lowercase-sha256>  vicora-sms-intelligence-v1.0.1-release.apk
  ```
- Release notes describing changes, fixes, and any migration or permission notes.

## Important release rules

1. Keep the Android application ID unchanged: `com.veehicee.vicorasms`.
2. Increase Android `versionCode` for every release. Never reuse a version code.
3. Sign every release with the same protected Android signing key. Never commit the keystore or its passwords to Git.
4. Test the APK before publishing it.
5. Do not publish SMS content, personal records, credentials, signing keys, or private source code here.
6. The app checks this repository's GitHub Releases feed. It does not upload SMS data.
7. Android requires the user to approve installation. Updates are never silently installed.

## Current status

The public release channel is prepared. The first tested, consistently signed APK has not yet been published.
