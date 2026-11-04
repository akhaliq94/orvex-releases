# ORVEX releases

Public download and auto-update channel for ORVEX (Windows x64).

The app checks this repository's latest release, downloads the build that matches
the installed copy (NSIS setup or portable exe) and installs only after you
confirm. Every download must match the published `SHA256SUMS.txt`; a mismatch is
refused before anything runs.

## Builds are unsigned

There is no code-signing certificate, so Windows SmartScreen will warn. Install
at your own risk.

The source repository is private. These release assets are the only public
artifacts.
