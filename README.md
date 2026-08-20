# Sirius

A Cmd+Tab that switches **windows**, not apps — plus a focus mode that keeps
the screen clear of everything else for as long as you set.

> **Early access.** Version 0.3 is the first build I consider genuinely usable
> day to day. It is not finished, and it is not yet for sale.

## Download

**[Download the latest version](https://github.com/Alex-Sancho/Sirius/releases/latest)**

Signed with a Developer ID certificate and notarized by Apple, so it opens
normally — no right-click tricks, no security warnings to click through.

## Requirements

- macOS 14 (Sonoma) or later
- Apple silicon or Intel (universal build)

## Install

1. Download `Sirius.zip` and unzip it.
2. Move `Sirius.app` to your **Applications** folder.
3. Launch it. Sirius has no Dock icon — it lives in the menu bar.
4. Grant the two permissions below when asked, then press **Cmd+Tab**.

## Permissions, and what they actually mean

Sirius asks for two of the most sensitive permissions macOS has. You should
know exactly why before you grant them.

**Accessibility** — required to intercept Cmd+Tab before the system handles
it, and to raise the window you pick. There is no other way for any app to
replace Cmd+Tab on macOS.

**Screen Recording** — required to draw the small live thumbnail on each card,
so you can tell three Finder windows apart. Without it, Sirius still works;
the cards just show icons instead of window previews.

And what Sirius does *not* do:

- **It makes no network connections.** Version 0.3 contains no networking code
  at all. Nothing you do is sent anywhere, because there is nowhere to send it.
  (A future version will add an update check — it will be announced here, and
  it will only ever ask "is there a newer version".)
- **It does not log keystrokes.** The event tap reacts to Cmd+Tab and to the
  shortcut you configure. It reads no text.
- **It does not read window contents.** Screen Recording is used to render
  thumbnails on screen and nothing else.

## Feedback

This is what early access is for. Open an
[issue](https://github.com/Alex-Sancho/Sirius/issues) — bugs, confusions, and
"I expected this to do X" are all equally useful.

## Updating

Version 0.3 does not update itself yet. Check this page, or watch the
repository to be notified of new releases. Automatic updates are the next
thing being built.

---

© 2026 Oleksandr Chernysh. All rights reserved.
This repository distributes the application. It is not open source, and no
source code is published here.
