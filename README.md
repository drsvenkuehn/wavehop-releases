# Wavehop

**Stream your Windows PC's sound to AirPlay speakers.** Wavehop lives in the system tray, captures what your PC plays and sends it to HomePods, AirPlay speakers and soundbars on your network, alone or as a synchronized multi-room group. No drivers, no virtual audio devices.

Wavehop is **free** (closed source). [Download the newest release](https://github.com/drsvenkuehn/wavehop-releases/releases) | [Buy me a coffee](https://buymeacoffee.com/drsvenkuehn)

> **Beta.** Wavehop is in public beta. Expect rough edges and please report what you find (see below).

## What it does

- Streams all system audio to one or more AirPlay speakers (AirPlay 1 and AirPlay 2).
- Multi-room: pick several AirPlay 2 speakers and they play in sync. AirPlay 1 receivers play one at a time.
- Volume control, low-latency mode (single speaker), start with Windows, automatic reconnect after a lost connection.
- Automatic update checks, if you allow them (can be turned off).
- Available in English, German, French, Spanish, Japanese, Simplified Chinese and Korean.

## System requirements

- Windows 11 (64-bit). Windows 10 version 1903 or later may work but is untested.
- A speaker or receiver with AirPlay on the same network (wired or Wi-Fi, same subnet)
- Windows firewall: Wavehop's installer adds a rule for **Private** networks. On a "Public" network, set the network to Private or Wavehop will show guidance.

## Tested speakers

| Speaker | Protocol | Status |
|---|---|---|
| Apple HomePod mini (several, as a synced pair) | AirPlay 2 | Tested |
| JBL BAR 300 | AirPlay 2 | Tested |
| AirPlay 1 receivers (tested with the open-source shairport-sync receiver) | AirPlay 1 | Tested |

Other AirPlay speakers should work but are untested. If yours works or fails, tell us (see "Report a problem").

## Install

1. Download `Wavehop-<version>-win64-setup.exe` from the newest entry on the [releases page](https://github.com/drsvenkuehn/wavehop-releases/releases).
2. Run it. Windows may show a SmartScreen warning, see below.
3. Wavehop appears in the system tray (click the `^` if hidden). Click it and choose a speaker.

### "Windows protected your PC" (SmartScreen)

Beta builds are **not code-signed yet**. A signing certificate costs money and builds reputation only over time, so Windows shows a blue SmartScreen warning for unknown, unsigned downloads. It does not mean the file is infected. To continue:

1. Click **More info**.
2. Click **Run anyway**.

You can check the download is the one published here: it comes only from this repository's Releases page.
## Known issues (beta)

- Long-duration (multi-hour) stability and some speaker models have not been tested yet.
- AirPlay 1 timing numbers were not measured in detail.
- Mixed AirPlay 1 and AirPlay 2 groups are not supported.
- Windows on ARM is not supported.
- Unsigned beta installers trigger SmartScreen (see above).

This list is updated with each release.

## Report a problem

- In Wavehop: tray menu, **Report a Problem...**. You can send the report (only if you opt in to reporting) or save it as a ZIP and attach it to an issue.
- Or open an [issue](https://github.com/drsvenkuehn/wavehop-releases/issues). Say which speaker, your Windows version and what happened.

## Privacy and legal

- [End-User License Agreement](legal/EULA.txt)
- [Privacy policy](legal/PRIVACY.md): update checks, and opt-in crash reports (Sentry, EU region)
- [Third-party notices](legal/THIRD-PARTY-NOTICES.txt)

## Support Wavehop

Wavehop is free and stays free. If it is useful to you: [buymeacoffee.com/drsvenkuehn](https://buymeacoffee.com/drsvenkuehn).

AirPlay, HomePod and Apple are trademarks of Apple Inc. Wavehop is not affiliated with Apple.
