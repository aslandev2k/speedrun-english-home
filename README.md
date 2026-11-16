# Speedrun English

A Mac app for learning English vocabulary by typing fast. Each run is
scored against your own records, the best minute and the longest combo,
and spaced reviews bring every word back before you forget it.
Everything stays on your Mac: no account, and Speedrun English connects
to the internet only to check for updates.

Needs macOS 27 or later on a Mac with Apple silicon.

**[Download the latest version](https://github.com/aslandev2k/speedrun-english-home/releases/latest)**

No version has been released yet.

## Install

1. Download `Speedrun-English-<version>.dmg` from the
   [latest release](https://github.com/aslandev2k/speedrun-english-home/releases/latest).
2. Open it and drag **Speedrun EN** onto **Applications**.
3. Open Speedrun EN from Applications. The first time, macOS stops it with
   a message that it could not check the app, because Speedrun English is
   not notarized by Apple. Click **Done** (not Move to Trash).
4. Open **System Settings > Privacy & Security**, scroll down to the
   message about Speedrun EN, and click **Open Anyway**. Confirm with your
   password or Touch ID, then click **Open**.

You only do this once. A new version may ask once more.

If you prefer, `Speedrun-English-<version>.zip` holds the same app. To
check a download, compare it with `SHA256SUMS.txt` in the release:

```sh
shasum -a 256 -c SHA256SUMS.txt
```

## Updates

Speedrun English checks for a new version once a day, the first time you
open it, then downloads it, verifies its signature, replaces the old
version, and relaunches. It never relaunches during a run: the update
waits until the run ends. Updates never touch your words, decks, history
or settings.

MENU > About (Command-I) shows the version you use, what is new in it, and
Check for Updates.

## This repository

This repository serves Speedrun English's downloads and its update feed:

- `appcast.xml` is the feed the app reads, at
  https://aslandev2k.github.io/speedrun-english-home/appcast.xml. Each
  entry is signed with the app's own update key.
- `notes/<version>.html` are the release notes of each version.
- Each release holds the disk image, a zip of the same app, and
  `SHA256SUMS.txt`.
