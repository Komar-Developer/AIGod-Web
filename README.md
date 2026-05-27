# AI GOD — Direct Download

Direct-download (Developer ID, Apple-notarized) builds of **AI GOD**, the
native macOS AI chat client.

Looking for the website / privacy / support pages? They live in the
AIGod branch and are deployed at https://komar-developer.github.io/AIGod-Web/

## Download

Always grab the latest version from the Releases tab:
https://github.com/Komar-Developer/AIGod-Web/releases/latest

Direct link (auto-updates to the newest release):
https://github.com/Komar-Developer/AIGod-Web/releases/latest/download/AI-GOD.dmg

## What you get

- Universal binary (Apple Silicon + Intel), macOS 12 Monterey or later.
- Signed with Developer ID Application: Adelio Falco Marti (F3CVAK9DV2).
- Notarized by Apple (no Gatekeeper warnings).
- 15-day free trial. After that, paste a license bought on Gumroad
  (https://aigodpro.gumroad.com/l/hlogk) to unlock forever.
- All future minor updates included.

## Install

1. Download AI-GOD.dmg.
2. Open the DMG and drag AI GOD to your Applications folder.
3. Launch from Launchpad or Spotlight.

If macOS refuses to open the app with "damaged" error (rare, usually means
the download was corrupted), run in Terminal:

    xattr -dr com.apple.quarantine /Applications/AI\ GOD.app

## Verify your download

Each release ships a SHA256.txt next to the DMG. To check:

    shasum -a 256 ~/Downloads/AI-GOD.dmg

The output must match the value in SHA256.txt.

## Want the Mac App Store version instead?

Open AI GOD on the Mac App Store (39.99 EUR, lifetime, Family Sharing).

## Changelog

See CHANGELOG.md for what changed in each release.

## Support

- Bug reports & feature requests:
  https://github.com/Komar-Developer/AIGod-Web/issues
- Email: aigod.pro2026@gmail.com
- Privacy policy: https://komar-developer.github.io/AIGod-Web/privacy.html
- Terms: https://komar-developer.github.io/AIGod-Web/terms.html

---

(c) 2026 Adelio Falco Marti . AI GOD
