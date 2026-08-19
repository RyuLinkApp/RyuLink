# RyuLink Release Policy

This document defines the public release conventions for the `RyuLinkApp/RyuLink` repository.

## Versioning

RyuLink releases should use semantic-style version numbers:

- `v0.x.y` while the project remains in public beta
- Increment `y` for compatible fixes and small improvements
- Increment `x` when a beta release introduces meaningful behavior, protocol, packaging, or compatibility changes

Pre-release builds may use identifiers such as `-beta.1` or `-rc.1` when additional validation is needed before a normal public release.

## Official release location

Official public builds are distributed through this repository's **GitHub Releases** page by the `RyuLinkApp` account.

A release should not be considered official merely because a file has been copied to a third-party mirror.

## Release assets

A normal public release should include:

- The RyuLink installation package
- `SHA256SUMS.txt` containing SHA-256 hashes for downloadable binary assets
- Release notes describing changes, compatibility information, upgrade notes, and known issues

Recommended package naming:

```text
RyuLink-vX.Y.Z.zip
SHA256SUMS.txt
```

If multiple platform-specific packages are introduced later, include the platform and architecture in the asset name rather than reusing an ambiguous filename.

## Release notes

Release notes should clearly separate the following where applicable:

- Added
- Changed
- Fixed
- Compatibility
- Upgrade notes
- Known issues

Breaking configuration, protocol, or package-layout changes must be called out prominently.

## Asset integrity

Published release assets must be treated as immutable.

Do not silently replace an already-published binary while keeping the same version number or asset name. If a published build is wrong, unsafe, corrupted, or materially different from what was intended:

1. Mark the affected release or asset as withdrawn / deprecated where appropriate.
2. Explain the problem in the release notes.
3. Publish a new version with corrected binaries.
4. Generate new SHA-256 checksums for the new assets.

Users should be able to trust that a version number refers to one specific published build.

## Tags

Release tags should match the release version, for example:

```text
v0.1.0
v0.1.1
v0.2.0-beta.1
```

Published release tags should not be moved to point at unrelated content after publication.

## Beta releases

While RyuLink is in public beta:

- Compatibility may differ between games and network environments.
- Known limitations should be stated instead of hidden.
- A release that has not completed normal validation should be marked as a pre-release.
- Users should be encouraged to include exact version information in bug reports.

## Security

Never publish secrets in release assets or release notes, including access tokens, server credentials, private keys, signing secrets, or production configuration containing credentials.

RyuLink release packages must not include ROMs, firmware, encryption keys, title keys, or copyrighted game content.

## Source code

This public repository is currently intended for product documentation, public-beta feedback, and official binary releases. Publication of release binaries here does not imply that the RyuLink source code is included in this repository.
