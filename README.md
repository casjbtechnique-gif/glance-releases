# Glance releases

Builds of **Glance**, one-hotkey screen sharing and file Sends between Macs on the same network. The source code is private; this repository only holds signed builds and the update feed.

## Install

1. Download the latest `Glance-<version>.zip` from [Releases](https://github.com/casjbtechnique-gif/glance-releases/releases/latest).
2. Unzip it and move **Glance.app** to **~/Applications**.
3. Open it. The first time, macOS says it can't verify the developer, because Glance is signed with our own certificate rather than Apple's. Go to **System Settings → Privacy & Security** and click **Open Anyway**.
4. Allow **Local Network** when asked. The first time you share, turn on **Screen & System Audio Recording** for Glance, then quit and reopen it.

Requires macOS 15 or later on Apple silicon.

## Updates

From 0.3.1 on, Glance updates itself. It checks this repository's `appcast.xml`, downloads in the background, and installs when you choose **Update and Restart**, or the next time it quits, but never during a Share. Every update is verified with our EdDSA key and must carry the same code signature as the installed app.
