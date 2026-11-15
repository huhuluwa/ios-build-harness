# macOS / Xcode iOS build harness

This public harness builds an unsigned IPA from an encrypted source archive.
The source archive is not stored in Git; the build job decrypts it only on the
macOS runner using the repository secret `SOURCE_KEY`.

The resulting IPA is unsigned. Installing it on a device still requires the
user's own Apple signing and provisioning identity.
