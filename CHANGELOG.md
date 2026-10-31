# Changelog

What changed in StudioSpend, in plain language, newest first. Each release's section is also its release notes on GitHub. Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Versions: `MAJOR.MINOR.PATCH`.

## [0.3.0] - 2026-10-29

### Added
- **Use StudioSpend inside Claude.** Settings → Claude → *Add to Claude* installs a small extension in Claude Desktop (two clicks). Then ask Claude what you have left, what's about to expire, and where to make a video, image or voice track. It reads from your Mac only and can't change anything. Claude Code users get a one-line command. (Needs this version or newer.)
- **Move to another Mac.** Settings → Your data → *Move to another Mac* carries your plans, payments, recent balances and settings to your second Mac in one passphrase-locked file. Importing replaces what is on that Mac after saving a safety copy, which you can undo for 30 days. Platform sign-ins never travel: reconnect them on the new Mac from a checklist.
- **Updates inside the app (Mac).** About twice a day StudioSpend checks whether a newer version exists. If one does, it downloads quietly, checks the download is genuinely ours, and shows "StudioSpend X is ready" with a **Restart to update** button. Nothing installs or restarts until you click, and *Later* hides the note until next launch. Settings → General → Updates has *Check now* and a switch to turn the automatic check off. This build is the last one you need to install by hand.
- A new look (the "Exchange" design): slate and ultramarine, split-flap figures, a reversed-out *Spend* total and *Use these first* board, and a first-launch splash.
- Monthly recap and "no alerts yet" screens read more clearly; the mini dash follows Light/Dark.

- **Runway API wallet.** If you also buy Runway API credits (dev.runwayml.com), add them under Runway as a second wallet: they are a separate pool from your plan. Claude's answers now say when a platform has an API wallet StudioSpend is not reading.

### Changed
- **Make is the new home screen, and it leads with money.** It shows what you've paid for and haven't used yet, in dollars, how much of it could reset unused, and the one place to use first, with a button to open it. Below it, every plan in the order its credits reset; tap a job (video, image, voice…) and the same list shows where to make it and what each one costs in credits. The app now opens on Make once you've set up.
- **Spend shows how to pay less**: plans that would fit you better (savings per month), the same model cheaper on another plan you have, and what each plan's credits really cost.
- **Account bars now show what's left** (they showed what was used), with the part that could reset unused marked in yellow. API wallets say plainly that they aren't your plan.

### Fixed
- Runway credits you bought (which never expire) are no longer counted as money about to go unused; only the plan's own credits can.
- A fresh sign-in now clears its old error immediately, and an expired sign-in keeps the platform's own reason.
- VEED sign-in discovery no longer fails on the platform's address redirect.

## [0.2.0] - 2026-09-24

The first beta: spend ledger and renewals, Make tab (what your credits can still make), live balances from platforms' official sign-ins, alerts for credits about to expire, statement import, CSV export, trial and license.
