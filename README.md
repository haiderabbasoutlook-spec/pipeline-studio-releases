# Pipeline Studio — updates

This repository holds only the **signed update packages** of Pipeline Studio. There is no source code here.

How the app uses it:

- Pipeline Studio checks `releases/download/feed/latest-<channel>.json` about 20 seconds after it opens, then every 6 hours.
- That file is signed (Ed25519). The app installs only what the signature and the package checksum prove is genuine; anything else is refused.
- Each version's package sits in its own release (`v<version>`).

Questions about Pipeline Studio: contact the seller you bought it from.
