# Yak — releases

Update feed and downloads for **Yak**, a personal macOS dictation app.

This repository is public only so that installed copies can fetch updates
without authenticating. It contains no source code — just `appcast.xml`
(the update feed) and the signed, notarized disk images in `downloads/`.

Every build is signed twice: with an Apple Developer ID and notarized by
Apple, and separately with an EdDSA key whose signature appears in the
appcast. Yak refuses any update not signed by that key.
