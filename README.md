# Obriy

A Cmd+Tab that switches **windows**, not apps – plus a focus mode that keeps
the screen clear of everything else for as long as you set.

> **Early access.** Version 0.3.2 is usable day to day. It is not finished,
> and it is not yet for sale.

## Download

**[Download the latest version](https://github.com/Alex-Sancho/Obriy/releases/latest)**

Signed with a Developer ID certificate and notarized by Apple, so it opens
normally – no right-click tricks, no security warnings to click through.

## Requirements

- macOS 14 (Sonoma) or later
- Apple silicon or Intel (universal build)

## Install

1. Download the zip and unzip it.
2. Move the app to your **Applications** folder.
3. Launch it. Obriy has no Dock icon – it lives in the menu bar.
4. Grant the two permissions below when asked, then press **Cmd+Tab**.

## Permissions, and what they actually mean

Obriy asks for two of the most sensitive permissions macOS has. You should
know exactly why before you grant them.

**Accessibility** – required to intercept Cmd+Tab before the system handles
it, and to raise the window you pick. There is no other way for any app to
replace Cmd+Tab on macOS.

**Screen Recording** – required to draw the small live thumbnail on each card,
so you can tell three Finder windows apart. Without it, Obriy still works;
the cards just show icons instead of window previews.

And what Obriy does *not* do:

- **It makes no network connections.** Version 0.3.3 and earlier contain no
  networking code at all. Nothing you do is sent anywhere, because there is
  nowhere to send it.

  The next version adds one, and one only: Obriy will ask
  `obriy.dev` whether a newer version exists. Nothing about you travels with
  that question – no identifier, no usage, no list of your apps. It will never
  ask while a focus session is running, so an update can never become a way out
  of a session you set yourself.
- **It does not log keystrokes.** The event tap reacts to Cmd+Tab and to the
  shortcut you configure. It reads no text.
- **It does not read window contents.** Screen Recording is used to render
  thumbnails on screen and nothing else.

## Feedback

This is what early access is for. Open an
[issue](https://github.com/Alex-Sancho/Obriy/issues) – bugs, confusions, and
"I expected this to do X" are all equally useful.

## Updating

Version 0.3.3 does not update itself: check this page, or watch the repository
to be notified of new releases. Moving from 0.3.x to the next version is a
manual download – the update mechanism only exists from that version onward.

After that, Obriy checks on its own and asks before installing anything.

---

© 2026 Oleksandr Chernysh. All rights reserved.
This repository distributes the application. It is not open source, and no
source code is published here.
