# Megan module releases

Public download distribution for the private Megan desktop source project.

**No operational trainer modules have been released.** Three signed definitions
previews are available for ME1, ME2 and ME3 Legendary Edition. Each contains only
configuration and a text notice. No cheat works, no executable/build support is
claimed, and no worker is included. All cheat activation stays disabled.

Use Megan desktop **0.2.0-preview or newer** for schema-2 preview packages. An
older desktop's initial `catalogue-v1` channel is retained separately so a running
older app does not receive incompatible metadata.

## Downloads and trust

- [Signed catalogue](https://github.com/play0/Megan-Modules/releases/download/catalogue-v2/catalogue.json)
- `publisher.json` contains the public ECDSA-P256 key and its SHA-256 fingerprint.
- Megan pins this public key in the desktop application. A key from a download
  cannot replace the host's trust root.
- Per-game releases use `me1-vVERSION`, `me2-vVERSION`, `me3-vVERSION` tags,
  with `release.json` and `package.zip` assets.
- Packages are signed before publication and checked for integrity, compatible
  identity, archive safety and size by the host before installation. Publishing
  here grants no worker permissions and does not enable cheats.

Signing happens locally. Private keys, GitHub credentials, desktop source, game
files and personal settings do not belong in this public repository. No Actions
workflow has access to a signing key.

The catalogue expires 30 days after signing. Its publisher must renew it before
expiry, even when no new modules are available. Offline/expired checks do not
remove previously verified compatible local installations.
