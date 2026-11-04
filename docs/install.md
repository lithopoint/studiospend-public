# Install and update StudioSpend

StudioSpend lives in your Mac's menu bar or your Windows system tray. On a Mac it has no Dock icon and no window until you click it. Windows is [further down](#windows).

## Install

1. Download **StudioSpend-macOS.dmg** from the [latest release](https://github.com/lithopoint/studiospend-public/releases/latest). One download covers Apple silicon and Intel Macs.
2. Open the file. A window shows the StudioSpend icon and your Applications folder.
3. Drag **StudioSpend** onto **Applications**.
4. Open **StudioSpend** from Applications (or Spotlight). Its icon appears in the menu bar. Click it.

The first time you open the app it asks to use your Keychain. That is where StudioSpend keeps the sign-ins you connect, and nowhere else. Choose **Always Allow** so it does not ask again.

Tested on macOS 26 (Tahoe).

<a id="first-open"></a>
## First open

StudioSpend is signed with an Apple Developer ID and notarized by Apple. macOS may say it is an app downloaded from the internet and ask you to confirm. Click **Open**.

## Check that your download is genuine

Compare the file's checksum with the one published on the release. Steps are in [verify.md](verify.md).

## Update

StudioSpend checks for updates itself and offers to install them. You can also download the newest release by hand and replace the app in Applications.

## Open at login

Settings → **Open at login** puts StudioSpend in your Login Items, so it is in the menu bar after a restart. Turn it off there, or in System Settings → General → Login Items.

## Remove it

See [uninstall.md](uninstall.md).

## Windows

1. Download **StudioSpend-Windows-x64-setup.exe** from the [latest release](https://github.com/lithopoint/studiospend-public/releases/latest). It runs on 64-bit Windows 10 and 11.
2. Run it. It installs for your user account and needs no administrator rights. The publisher it shows is **Michael Leonardo**.
3. While the app is new, Windows SmartScreen may say it doesn't recognize it. Choose **More info**, check the publisher, then **Run anyway**.
4. StudioSpend opens, and its icon sits in the system tray. If you don't see it, look under the **^** arrow beside the clock; you can drag it out to keep it visible.

StudioSpend keeps the sign-ins you connect in Windows Credential Manager. It checks for updates itself. Settings → **Open at login** starts it with Windows.
