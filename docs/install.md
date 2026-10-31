# Install and update StudioSpend

StudioSpend is a Mac app that lives in your menu bar. It has no Dock icon and no window until you click it.

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

StudioSpend does not update itself yet. To update, download the newest [release](https://github.com/lithopoint/studiospend-public/releases/latest), quit StudioSpend (**Settings → Quit StudioSpend**) and drag the new app onto Applications, replacing the old one. Your data stays where it is.

## Open at login

Settings → **Open at login** puts StudioSpend in your Login Items, so it is in the menu bar after a restart. Turn it off there, or in System Settings → General → Login Items.

## Remove it

See [uninstall.md](uninstall.md).
