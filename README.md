# Voice Dictate — downloads

Voice Dictate is a local push-to-talk dictation app for Windows: hold a key, speak, and the text is typed into whatever window you're using. Speech recognition runs on your own PC.

This repository contains **only the installers and update packages**. It is what the app's built-in updater reads, so updates can be downloaded without signing in to anything.

## Install

1. Open the [latest release](../../releases/latest).
2. Download **`VoiceDictate-Setup-<version>.exe`** and run it. It installs for your user only (no administrator rights needed) and keeps your settings when upgrading an older version.
3. Prefer no installer? **`VoiceDictate-<version>-portable.zip`** is a folder you can unzip anywhere.

Windows may show a "Windows protected your PC" notice, because the installer isn't code-signed. Choose **More info → Run anyway**.

## Updating

From version 0.9.0 on: **Settings → Advanced → Updates → Check for updates**. It only checks when you click.

Older versions have no update button, so install the latest version once by hand as above — it installs over the old one.

## Verifying a download

Each release lists the SHA-256 of its files in `SHA256SUMS.txt`, and the in-app updater checks every download against it before running anything.

| File | What it is |
|---|---|
| `VoiceDictate-Setup-<version>.exe` | Installer (full) |
| `VoiceDictate-<version>-portable.zip` | Portable folder |
| `VoiceDictate-<version>-app.zip` | Small code-only update used by the in-app updater |
| `update-manifest.json` | What the updater should download and how to verify it |
| `SHA256SUMS.txt` | Checksums |
