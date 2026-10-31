# Remove StudioSpend

## The app

1. Quit StudioSpend: open **Settings → Quit StudioSpend**, or press ⌘Q while its window is in front. Closing the window alone leaves it running in the menu bar.
2. Drag **StudioSpend** from Applications to the Trash.
3. If you turned on **Open at login**, open System Settings → General → Login Items and remove it there if it is still listed.

That leaves your data in place, which is useful if you reinstall later.

## Your data (optional)

To remove everything StudioSpend stored, delete these. In Finder choose **Go → Go to Folder** (⇧⌘G) and paste each path.

| What | Where |
|---|---|
| Your plans, payments and balances | `~/Library/Application Support/com.lithopoint.studiospend` |
| Caches and web data | `~/Library/Caches/com.lithopoint.studiospend` and `~/Library/WebKit/com.lithopoint.studiospend` (either may not exist) |
| Settings | `~/Library/Preferences/com.lithopoint.studiospend.plist` (may not exist) |

Before you delete the first folder, use **Settings → Export your data** if you want a copy of your spend as spreadsheets.

## Your sign-ins

StudioSpend keeps one item in your Keychain, named **com.lithopoint.studiospend**, which holds the access it was granted by the platforms you connected.

1. Open **Keychain Access** (Spotlight → "Keychain Access").
2. Search for `studiospend`.
3. Select the item and press Delete.

That removes the saved sign-ins from your Mac. To end each platform's side of the connection, sign in to the platform and revoke StudioSpend under its connected apps or integrations settings.

## Early betas

If you tried a beta before the public release, its data may sit in a second folder under `~/Library/Application Support` whose name starts with `com.`. StudioSpend copies it forward the first time it starts and leaves the old folder as a backup. [Ask support](../SUPPORT.md) if you want help finding and removing it.

## Your license

Removing the app does not cancel a subscription. Manage billing from your receipt email, or contact [support](../SUPPORT.md).
