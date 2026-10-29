# CUTTO for macOS

CUTTO edits talking-head video in DaVinci Resolve: podcasts, interviews, courses, and expert content.
This repository distributes application binaries, release notes, and the Sparkle update feed. Application source is private.

## Download and install

No application release has been published yet. Future downloads will appear in
[Releases](https://github.com/AlekseySh/cutto-releases/releases).
Download the CUTTO macOS arm64 ZIP asset, extract `CUTTO.app`, and move it to its final location before installing
the Resolve Bridge hook. GitHub's automatic source archives contain only this distribution repository.

Requirements: Apple Silicon and DaVinci Resolve. Tested on macOS 26.6.2 with Resolve Free 21.0.2.4;
compatibility with older macOS versions and Resolve 21.1 remains unverified.
Python, FFmpeg, and ffprobe are included in the application.
Current builds use an ad-hoc signature; Developer ID signing and notarization remain unfinished.
First launch may require **System Settings → Privacy & Security → Open Anyway**. One observed installation required
a reboot after permission was granted; the cause remains unresolved.

## Updates

Configured builds offer **Settings → Check for Updates…**. Checks are manual, and downloaded archives require
a valid Sparkle Ed25519 signature. Stop CUTTO MCP and finish data cleanup before checking. If Resolve uses this app's
Bridge, save the project and close Resolve before installing, then reopen it afterward.

The permanent feed is [appcast.xml](https://raw.githubusercontent.com/AlekseySh/cutto-releases/main/appcast.xml).
Credentials and project data remain outside the application when it is replaced.
