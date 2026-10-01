---
title: Kyouka Privacy Policy
---

# Kyouka Privacy Policy

**Last updated: 2026-10-01**

Kyouka ("the app") is a utility app that shows one kanji a day via its Home Screen and Lock Screen
widgets. This page states, plainly, what the app does and does not do with your data, kept consistent
with the app's actual code and architecture — no custom backend, no third-party analytics, and a privacy
manifest declaring exactly what's described below — rather than a generic template.

## The short version

- **No account.** Kyouka has no sign-up, no login, and no user ID of its own.
- **No server.** Kyouka has no backend of any kind. There is nothing for the developer to run, and
  nothing the developer's own infrastructure ever receives.
- **No analytics, no tracking, no third-party SDKs.** Kyouka does not use advertising identifiers, does
  not track you across apps or websites, and links no analytics or advertising service.
- **Your marks and notes sync only through your own iCloud account**, directly between your own devices,
  via Apple's CloudKit. The developer cannot read this data — it lives in your **private** CloudKit
  database, which only you can access, the same way Notes or Reminders data does.
- **Crash reports, if any, go straight to Apple**, via Xcode Organizer / App Store Connect's own built-in
  crash collection. Kyouka contains no crash-reporting code of its own.

## What data exists, and where it lives

| Data | What it is | Where it's stored | Who can read it |
| --- | --- | --- | --- |
| Your kanji marks (bookmarked / known / confusing / excluded) | Which kanji you've tagged, and how | On your device, and mirrored to your own private iCloud database if you're signed in to iCloud | Only you, on your own devices |
| Your per-kanji notes | Short free-text notes you optionally add to a kanji (up to 140 characters) | Same as marks, above | Only you |
| Your daily selection state | Which kanji you've been shown, your reroll history, and your widget field preferences | On your device (and your App Group, so the widget can read it), mirrored the same way as marks | Only you |
| Purchase/subscription status | Whether you've unlocked the full kanji pool | Resolved directly from Apple via StoreKit; Kyouka stores only a local cache of the resulting yes/no state | Apple and you; the developer receives standard App Store sales reporting, like any paid app, but no per-user purchase data |

Kyouka's bundled kanji dictionary data (readings, example words) is static content shipped inside the app
— it never changes based on anything about you, and nothing about your usage of it is sent anywhere.

## What Kyouka does not do

- It does not collect your name, email address, location, contacts, photos, or any other data not listed
  above.
- It does not use your data for advertising, does not sell your data, and does not share your data with
  any third party — there is no third party in this app's data flow to share it with.
- It does not track you across other apps or websites, and does not use the Advertising Identifier (IDFA).

## Children's privacy

Kyouka does not knowingly collect any personal information from anyone, including children, beyond the
on-device/private-iCloud data described above, which the app itself never reads back in identifiable form.

## Changes to this policy

If Kyouka's data handling ever changes, this page will be updated in the same change that ships the new
behavior — the project's own engineering process requires it (see the "Update docs when architectural
behavior changes" rule in the project's `CLAUDE.md`).

## Contact

Questions about this policy or your data: see the [Support page](support.html), or email
<kyouka@gmail.com>.
