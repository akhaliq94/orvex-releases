# ORVEX releases

Public download and auto-update channel for ORVEX (Windows 10/11, x64).

## Install

1. Open the [latest release](https://github.com/akhaliq94/orvex-releases/releases/latest).
2. Download `ORVEX-Setup-<version>.exe`.
3. Run it. Windows SmartScreen will warn because the build is unsigned: choose
   **More info** then **Run anyway**.
4. The installer is per-user. Pick a folder if you want, then finish; it creates
   desktop and Start-menu shortcuts.

Prefer no installer? Download `ORVEX-Portable-<version>.exe` and run it
directly. A portable copy cannot replace itself when updating; the updater
reveals the new build for a manual swap instead.

## Verify a download (optional)

`SHA256SUMS.txt` lists the SHA-256 of both builds. In PowerShell:

```powershell
Get-FileHash .\ORVEX-Setup-1.0.0.exe -Algorithm SHA256
```

Compare the hash with the matching line in `SHA256SUMS.txt`. The in-app updater
also refuses any download whose hash does not match, so nothing runs unverified.

## Updates

Installed copies check this repository on launch (setting: Advisor → Updates).
A new build is only installed after you confirm, and only when the published
SHA-256 matches. Nothing installs silently.

## Honest notes

- Builds are **unsigned**. There is no code-signing certificate, so SmartScreen
  and some antivirus products will warn. Install at your own risk.
- Windows-first: input, OCR, volume and brightness integration target Windows.
  macOS/Linux adapters exist but are not live-tested in these builds.
- Model providers and API keys are configured by you in the app; nothing is
  bundled or preconfigured.
- The source repository is private. These release assets are the only public
  artifacts.
