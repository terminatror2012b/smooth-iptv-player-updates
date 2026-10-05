# Smooth IPTV Player Updates

Public APK release channel for Smooth IPTV Player.

## Required release format

For every new app version:

1. Build the APK with the same Android package and signing certificate as the installed app.
2. Create a GitHub Release tagged with the app version, for example `v0.15.32`.
3. Attach the APK using this exact filename:

   `SmoothIPTVPlayer.apk`

4. Publish the release as a normal release, not a prerelease.

Smooth IPTV Player checks the GitHub `latest release` endpoint, compares the release tag with the installed app version, downloads `SmoothIPTVPlayer.apk`, verifies GitHub's SHA-256 release digest when available, verifies the Android package name and signing certificate, and then opens Android's package installer.

## Repository

This repository is for update APK releases only. Do not store IPTV credentials, provider URLs, usernames, passwords, Firebase secrets, keystores, or private source archives here.
