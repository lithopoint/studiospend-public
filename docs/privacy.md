# Privacy: what StudioSpend stores and what leaves your Mac

Short version: your data lives on your Mac, there is no StudioSpend account and the app sends no analytics. The sections below say exactly what that means.

## What stays on your Mac

| What | Where |
|---|---|
| Your plans, payments, renewal dates, balance history and settings | A database in `~/Library/Application Support/com.lithopoint.studiospend` |
| The sign-ins you connect to platforms | One item in your Keychain named `com.lithopoint.studiospend` |
| Statements you import (CSV, OFX, QFX) | Read on your Mac and matched there. The file is not uploaded anywhere, and only the charges you confirm are saved |
| Platform logos | Bundled inside the app. StudioSpend does not load logos from the web, because a request per platform would tell a third party which tools you pay for |

## What leaves your Mac

1. **Balance requests to platforms you connect.** When you connect Runway, for example, StudioSpend asks Runway for your balance, the same way any app you sign in to would. It does this only for platforms you connected.
2. **A license check.** The app asks our license service whether your license is valid, about once a day. The request carries your license key and a fingerprint of your Mac used to count devices. It does not carry your spend data.
3. **The public price table.** The app downloads a public file of plans, prices and credits per job from `files.studiospend.com`, about twice a day. The request does not identify you or say what you use.

Nothing else is sent. There are no analytics, no crash reporting service and no advertising identifiers.

If you choose **Help & feedback**, your browser opens a form on a hosted form service. The form tells you what it sends (your message and, if you choose, the app version and macOS version). It goes only when you submit it.

## Sign-ins

StudioSpend uses each platform's official sign-in page, in your own browser. You enter your password there and never in StudioSpend. The platform then gives StudioSpend a limited permission, which the app keeps in your Keychain. Where a platform only offers an API key, you paste it into the app, and it goes to the same Keychain item.

You can end any connection from StudioSpend (Accounts → the platform → Disconnect) and from the platform's own connected-apps settings.

## The Claude connector

The optional connector for Claude runs on your Mac, reads the same data the app shows, and cannot change anything. It does not read your Keychain. Claude receives the answers you ask for in a conversation, under the terms of the Claude account you use.

## Payments

When you subscribe, payment is handled by our merchant of record. StudioSpend never sees your card number. You receive your license key by email.

## Deleting your data

Remove the app, the folder and the Keychain item listed in [uninstall.md](uninstall.md). That is all of it. We hold no copy of your ledger, so there is nothing for us to delete on our side except the license record tied to your purchase. Ask [support](../SUPPORT.md) if you want that removed too.
