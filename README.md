# Megan module releases

Public download distribution for the private Megan desktop source project.

**No operational trainer modules have been released.** All cheat activation in
Megan remains disabled. An empty, signed catalogue bootstraps the download channel;
it is not a game module or proof of a supported game build.

## Downloads and trust

- [Signed catalogue](https://github.com/play0/Megan-Modules/releases/download/catalogue-v1/catalogue.json)
- `publisher.json` contains the public ECDSA-P256 key and its SHA-256 fingerprint.
- Megan pins this public key in the desktop application. A key from a download
  cannot replace the host's trust root.
- Per-game releases will use `me1-vVERSION`, `me2-vVERSION`, `me3-vVERSION` tags,
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
