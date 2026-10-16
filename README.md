# ScreenMonitor

A small Windows tool that watches a region of the screen and plays a sound alert when a specific color (`#007ad9`) appears there. It can also keep the session alive with an automatic mouse clicker until the alert fires.

## Features

- **Region monitoring** – drag to select any area on any monitor; the app checks it every second.
- **Sound alert** – loops until you press **Stop**.
- **Custom sound** – put a `sound.mp3` next to `ScreenMonitor.exe` and it will be used instead of the built-in sound.
- **Email alerts** – optionally get a *New game assigned* email when the alert fires (free, via [FormSubmit](https://formsubmit.co/), no account needed).
- **Mouse clicker** – left-clicks every 10.5–11.5 seconds (random) at the position of the first click (your own click after turning it on, or the first automatic one) – the cursor jumps there, clicks and returns to where it was, and focus goes back to the window you were using – and stops automatically when the alert fires.
- **Multi-monitor and display-scaling aware.**

## Download

**[Download the latest ScreenMonitor.exe](https://github.com/djolemc/ScreenMonitor-releases/releases/latest/download/ScreenMonitor.exe)** – or see all versions on the [Releases](https://github.com/djolemc/ScreenMonitor-releases/releases) page. No installation needed – it's a single portable file.

## Usage

1. Run `ScreenMonitor.exe`.
2. Click **Select region** and drag a rectangle over the area to watch (**Esc** cancels).
3. The status changes to *Waiting for changes...*.
4. Optionally start the clicker – press **Ctrl+F2**, then click where it should click (or just leave the mouse there until the first automatic click).
5. When the color appears, the alert plays and the clicker stops. Press **Stop** to silence it.

| Hotkey | Action |
|---|---|
| `Ctrl+F2` | Toggle mouse clicker |
| `Ctrl+F3` | Stop tracking, alert and clicker |

> The clicker always clicks at the first click position – to change it, turn the clicker off and on again and click the new spot.

## Email alerts

1. Enter your email in **Alert email** and click **Send test email**.
2. The first time, FormSubmit sends you a confirmation email – click **Activate Form** (check spam if it doesn't arrive).
3. Click **Send test email** again – you should receive a test message.

From then on, every alert also sends a *New game assigned* email. Activation is needed only once per address. Leave the field empty to disable email alerts. The address is stored in `config.ini` next to the exe. Click **?** next to the test button for these instructions in the app.

## Windows SmartScreen

The exe is not code-signed, so Windows may show *Windows protected your PC* on first run. Click **More info → Run anyway**.
