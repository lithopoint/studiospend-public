# Changelog

What changed in StudioSpend, in plain language, newest first. Each release's section is also its release notes on GitHub. Format: [Keep a Changelog](https://keepachangelog.com/en/1.1.0/). Versions: `MAJOR.MINOR.PATCH`.

## [1.0.1] - 2026-11-06

### Added
- **A way for AI platforms to ask to be added.** Settings → Help & feedback has a new choice, "I run an AI platform", for platform teams who want StudioSpend to read their plan. It sends nothing about your app or accounts.

### Changed
- Security and reliability improvements, including updated connection libraries and tighter limits on what the app's window can load and open.

### Fixed
- On Windows, an update could stop with "Error opening file for writing" if StudioSpend hadn't finished closing. The installer now waits for it.
- A license key already on two computers now says so plainly when you try it on a third, and tells you what to do.

## [1.0.0] - 2026-11-04

The first full release, for Mac and Windows. Free for 30 days, then $5 a month or $45 a year.

### Added
- **See what you can still make at a glance.** Each job on Make shows how many you can make with what you have left, and picking one turns the big figure into that count, still with what you've paid for and not used yet alongside it.
- **StudioSpend for Windows.** A signed installer for Windows 10 and 11 (64-bit), with the same app, the same license, and in-app updates.
- **Connected plans add themselves.** When you connect a platform that reports its plan, and StudioSpend knows that plan's price, it goes straight onto Spend ("Added Runway Pro to Spend · $35/mo", with Undo). Anything it can't price, a platform that reports no plan, and developer API wallets still wait for you as cards, which now appear as soon as you connect instead of after every account refreshes, and lead Spend until your first plan is added.

### Changed
- Tags such as "Trial ends", "Smaller plan" and "Pay as you go" are one size larger, so they're easier to read.
- **Pay less speaks in videos and images, not credits.** A plan that would fit you better now says how much you use and what the other plan covers in jobs ("You make about 15 videos a month; Standard covers about 22"), or in dollars when StudioSpend can't tell what the credits went on.
- **Make shows every plan you entered, in two lists.** *Paid plans* keeps the dollars that add up to the total at the top ("8 plans counted"). Under it, *Also tracking* lists everything else (free plans, a plan with no balance yet, one StudioSpend can't price): the credits each one last reported, never dollars, and a link to the one step that would count it (*Change plan* for a plan entered as free, *Connect* or *Add balance* for one with no balance yet). It's open; fold it from its heading and Make remembers. Their credits still count when you pick a job. A plan with under a dollar left reads "< $1" instead of "≈ $0".

### Fixed
- Signing back in is needed less often. A platform that renews your sign-in can no longer lose the renewal to a slow answer or a failed save, and a Reconnect you don't finish no longer signs you out.
- A platform that stops answering no longer holds up that platform's balance until you restart, and Connect no longer spins forever if the sign-in page never returns.
- Warnings on Accounts now say what actually happened and offer only what can help, with the error details right there. Account details in a platform's reply are removed before they're shown.
- Clicking the "Plan" caption in the plan form no longer sets the plan to Free at $0.
- A very long error reply from a platform can no longer crash the app.
- A mistyped license key no longer ends your free trial. It's turned down with the reason, and the trial carries on.
- A license whose subscription has ended now offers Subscribe again, instead of only "Open License".
- A Mac clock that was once set ahead no longer locks a paid license or ends the trial for good; it's corrected once the clock is right again.
- If the app's data folder is deleted but your license key is still in the keychain, StudioSpend checks the key instead of showing the trial.
- A slow or stuck update download no longer holds up balances, alerts and the daily license check.
- When the Claude connector is paused, Claude now says why (trial over, a license that needs attention, or a build that stopped), instead of always "your trial has ended".
- The Ideogram API row on Accounts says what you were billed once ("$11.60 billed this month · API account, not your plan"), instead of "Usage-billed", a "Billed usage" tag and "USD billed billed".
- A free trial's credits no longer count as money that could reset unused. Alerts, the monthly recap and Claude's answers now say nothing is at risk while a plan is on trial, as the Make tab already did.
- A trial in Spend's "Coming up" list is no longer cut off in a narrow window: the full name shows, with a "Trial ends" tag beside it.
- Small tags such as "Trial ends", "Few left" and "Pay as you go" no longer disappear when you point at their row.
- *What it really cost* no longer treats a plan on a free trial as paid for: it says nothing has been paid yet, instead of claiming each job really cost several times its price.

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
