# Frequently asked questions

## Getting started

**Do I need to connect my accounts?**
No. You can type in what you pay for, or import a bank or card statement, and the Spend tab works fully. Connecting a platform adds a live balance for it.

**What does StudioSpend cost?**
The first 30 days are free, with no card and no account. After that it is $5 a month or $45 a year.

**What happens when the trial ends?**
Your data stays and so do the Spend tab, adding and editing entries, and statement import. Live balance refresh, connecting new platforms, alerts and the Make tab pause until you add a license key. Nothing is deleted.

**Does it work on Windows?**
Not yet. StudioSpend is a Mac app for now.

**Which Macs and macOS versions?**
Intel and Apple silicon Macs, from one download. It is tested on macOS 26 (Tahoe). Older versions may work but have not been tested.

## Your accounts and your data

**Is it safe to connect my accounts?**
You sign in on each platform's own sign-in page, so StudioSpend never sees your password. What it receives is a permission the platform grants, and it keeps that in your Mac's Keychain. You can revoke it from the platform's own settings at any time. [Details](privacy.md).

**Can StudioSpend change my plan, spend my credits or cancel anything?**
No. It reads balances and nothing else. It cannot generate anything, buy anything or change a subscription.

**Where is my data?**
In a database on your Mac. There is no StudioSpend account and no cloud copy. Locations are listed in [uninstall.md](uninstall.md).

**Why does macOS ask about my Keychain?**
StudioSpend keeps your connected sign-ins in one Keychain item. macOS asks the first time the app reads it. Choose **Always Allow**.

**Can I use it on a second Mac?**
Yes, with the same license. **Settings → Your data → Move to another Mac** carries your plans, payments and settings in one passphrase-locked file. Sign-ins do not travel, so you reconnect them on the new Mac.

## Platforms

**Why can't it read my Midjourney (or Suno, or ChatGPT) balance?**
Those platforms have no official way for another app to read a balance. You can enter the plan by hand or import a statement, and StudioSpend still tracks the spend and the renewal date.

**Why does a balance say "estimate"?**
Platforms count credits differently, so StudioSpend turns them into jobs ("about 40 videos") using a price table it publishes with its sources and dates. A figure marked with ≈ is an estimate, and the table says how sure it is.

**A platform I use is missing.**
Tell us in **Settings → Help & feedback**. New platforms are added as they open official sign-in or a read-only balance.

## Trouble

**macOS says it cannot verify StudioSpend.**
This should not happen with a notarized build. Re-download the file from the [releases page](https://github.com/lithopoint/studiospend-public/releases/latest), then check it with [verify.md](verify.md). If it still happens, tell us.

**A connected platform shows "sign in again".**
The platform ended the session or you revoked it. Open **Accounts** and reconnect it.

**The menu-bar icon is missing.**
Open StudioSpend from Applications once. Menu bars on a notched MacBook can hide icons when they are full: quit a few other menu-bar apps and look again.

**Something else.**
See [SUPPORT.md](../SUPPORT.md).
