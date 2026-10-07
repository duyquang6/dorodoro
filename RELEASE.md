# DoroDoro 2026.10.07

*Tiếng Việt: [hướng dẫn cài đặt và cách dùng](https://github.com/duyquang6/dorodoro/blob/main/README.vi.md)*

A play-time limit for the TrimUI Brick Pro, pomodoro style. This is the first
release.

<p align="center">
  <img src="https://github.com/duyquang6/dorodoro/raw/main/media/setup.png" width="300" alt="Picking how long to play">
  <img src="https://github.com/duyquang6/dorodoro/raw/main/media/clock.png" width="300" alt="The countdown">
  <img src="https://github.com/duyquang6/dorodoro/raw/main/media/times-up.png" width="300" alt="Time's up">
</p>

Pick how long to play, press A, and go play. DoroDoro keeps counting in the
background while you are in a game. When the time is up, the handheld
**rumbles, rings and blinks every LED red**, over the game. It does this even
if the handheld went to sleep in the meantime.

- **Stops from inside the game:** press **SELECT + START** together.
- **A nudge first:** rumble, a ding and red LEDs at 5 minutes and at 1
  minute left.
- **A desk clock:** in the app, the countdown fills the screen, always on or
  dark after 30 seconds without a press.

## Download

| Your firmware | File |
|---|---|
| spruceOS | `DoroDoro-2026.10.07-spruceOS.zip` |
| stock TrimUI | `DoroDoro-2026.10.07-stockOS.zip` |

Both have the same app. They differ only in which directory the firmware looks
in. Check an archive against `SHA256SUMS.txt` if you got it anywhere but here.

## Install

1. Unzip onto the root of the SD card, and merge the folder when asked. The
   zip already holds the right folder for your firmware: `App/DoroDoro` for
   spruceOS, `Apps/DoroDoro` for stock TrimUI.
2. Open **DoroDoro** from the launcher, pick a length, press A.
3. Press B to go back to the launcher and start a game. It keeps counting.

## Known issues

- **Not yet tested on stock TrimUI firmware.** The build is the same program
  as the spruceOS one.
- The game also sees SELECT + START. Some games treat it as pause.

Free. DoroDoro is proprietary: you may install it on your own handheld, and
share these archives unchanged and free of charge (see
[LICENSE](https://github.com/duyquang6/dorodoro/blob/main/LICENSE)).
