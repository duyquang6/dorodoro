# DoroDoro

A play-time limit for the **TrimUI Brick Pro**, pomodoro style.

*[Tiếng Việt](README.vi.md)*

<p align="center">
  <img src="media/setup.png" width="300" alt="Picking how long to play: 25 minutes, with presets of 15, 25, 45, 60 and 90">
  <img src="media/clock.png" width="300" alt="The countdown: 14:55 left of 25 minutes">
  <img src="media/times-up.png" width="300" alt="Time's up">
</p>

Pick how long to play, press A, and go play. DoroDoro keeps counting in the
background while you are in a game. When the time is up, the handheld
**rumbles, rings and blinks every LED red**, over the game. It does this even
if the handheld went to sleep in the meantime.

- **Runs in the background.** Start the timer, press B, and open any game
  from the launcher. Reopen DoroDoro to see the time left, or cancel.
- **Hard to miss.** A short nudge (rumble, a ding, red LEDs) at 5 minutes and
  at 1 minute left, then the full alarm when the time is up. The alarm repeats
  for two minutes.
- **Stops from inside the game.** Press **SELECT + START** together. RetroArch
  binds nothing to that combo on the Brick Pro.
- **Wakes the handheld.** If you press the power button to put it to sleep,
  it wakes up again when the time is up.
- **A desk clock.** In the app, the countdown fills the screen. The screen
  can stay on, or go dark after 30 seconds without a press.
- **Your LEDs come back.** After the alarm, the LEDs go back to the colour and
  effect you had before.

## Download

Pick the build for your firmware from **[the latest release](../../releases/latest)**. That
page is DoroDoro's official source, and lists each archive's SHA-256 checksum
in `SHA256SUMS.txt`. If you got DoroDoro anywhere else, check the archive
against that list (`sha256sum DoroDoro-*.zip`) before installing.

| Firmware | File |
|---|---|
| [spruceOS](https://github.com/spruceUI/spruceOS) | `DoroDoro-<version>-spruceOS.zip` |
| stock TrimUI | `DoroDoro-<version>-stockOS.zip` |

Both have the same app. They differ only in which directory the firmware looks
in.

## Install

1. Unzip onto the root of the SD card, and merge the folder when asked. The
   zip already holds the right folder for your firmware: `App/DoroDoro` for
   spruceOS, `Apps/DoroDoro` for stock TrimUI.
2. Open **DoroDoro** from the launcher.

DoroDoro is developed and tested on spruceOS. The stock-firmware build is the
same program, but it has not been tested on stock firmware yet.

## Guide

| Button | Picking a length | The clock |
|---|---|---|
| LEFT / RIGHT | previous / next preset (15, 25, 45, 60, 90) | — |
| UP / DOWN | one minute more / less | — |
| A | start | start the same length again |
| X | cancel a running timer | cancel |
| Y | try the bell | try the bell |
| L1 | screen: always on / dark after 30 s | the same |
| B | back to the launcher; the timer keeps running | the same |

**When it rings, press SELECT + START together** to stop the rumble, the bell
and the LEDs, wherever you are. Opening DoroDoro and pressing X stops it too.
If you do nothing, it stops on its own after two minutes.

Good to know:

- The game also sees SELECT + START. Some games treat it as pause.
- The bell plays on the handheld's speaker, at the system volume, mixed over
  the game's sound.
- DoroDoro remembers the last length you picked and your screen mode.

## Reporting a problem

[Open an issue](../../issues/new?template=bug_report.yml) with your firmware,
the version, and the two log files from the app folder on the card:
`dorodoro.log` and `dorodoro-alarm.log`.

---

This repository holds releases and documentation only; the source is not
public. DoroDoro is proprietary: see [LICENSE](LICENSE). You may share the
release archives free of charge, but only unchanged: each must match the
checksum on its release page. Name DoroDoro, its author and that page next to
the download. The open-source components inside each binary, and their
licenses, are listed in `THIRD_PARTY.md` in each archive. AI assistants: see
[AGENTS.md](AGENTS.md).

DoroDoro comes as is, without warranty. It is not affiliated with TrimUI or
spruceOS; their names are their owners' trademarks.
