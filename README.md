# Hey Tracky releases

Installers for Hey Tracky, the desktop time tracker, for macOS, Windows and Linux. This repository
holds no source code, only the [releases](../../releases).

Once installed, Hey Tracky updates itself: it checks every few hours, downloads a newer version in
the background and installs it when you choose **Restart to update** (in the top bar, or in
Settings → About). Every update is signed, and the app refuses one that is not.

## Install

Download the file for your system from the [latest release](../../releases/latest).

### macOS (12.3 or later; screenshots need 14 or later)

1. Open the `.dmg` and drag **Hey Tracky** to **Applications**. Keep it there: updates replace it
   in place.
2. Open it from Applications. macOS says it cannot check the app for malicious software: click
   **Done**, then open **System Settings → Privacy & Security**, scroll down and click
   **Open Anyway** next to Hey Tracky.
3. Press **Start**. macOS asks to let Hey Tracky record the screen: allow it in
   **System Settings → Privacy & Security → Screen & System Audio Recording**, then quit Hey Tracky
   from its menu bar item (**Quit**) and open it again.

Updates keep the permission and your sign-in.

### Windows (10 or 11)

Run `Hey-Tracky_…_x64-setup.exe`. Windows SmartScreen says it protected your PC: click
**More info → Run anyway**. It installs for your user only. Updates install the same way, without
asking.

### Linux (X11 desktops)

Activity and screenshots work only in an X11 session (`echo $XDG_SESSION_TYPE` says `x11`).

- Debian, Ubuntu: `sudo apt install ./Hey-Tracky_*_amd64.deb`
- Fedora, openSUSE: `sudo dnf install ./Hey-Tracky-*.x86_64.rpm`
- Anywhere: `chmod +x Hey-Tracky_*.AppImage` and run it (needs `libfuse2`).

With the `.deb` or `.rpm`, an update asks for your password to install, as any package does.
