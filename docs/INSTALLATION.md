# RyuLink Installation

RyuLink is currently in public beta. Installation details may change between releases, so always read the release notes for the version you are installing.

## Requirements

Before installing RyuLink, make sure you have:

- A Nintendo Switch with a supported homebrew environment, such as Atmosphère
- Access to the console's SD card
- A supported local-wireless or LAN multiplayer game
- A working Internet connection
- The same RyuLink release on consoles that will play together whenever possible

## Download

Download RyuLink only from the **GitHub Releases** section of the official `RyuLinkApp/RyuLink` repository.

Do not install packages redistributed by unknown third parties. If a release includes SHA-256 checksums, verify the downloaded package before installing it.

## Install or update

1. Back up any existing RyuLink files and configuration that you may want to keep.
2. Download the RyuLink package for the release you want to install.
3. Read that release's notes and any instructions included in the package.
4. Copy the packaged files to the SD card using the directory layout provided by that release.
5. If the release updates a sysmodule or other boot-time component, fully reboot the console before testing.
6. Start RyuLink and confirm that the application can connect before launching a multiplayer session.

Because the public-beta package layout may still evolve, this document intentionally does not hard-code SD-card paths that could become outdated. The instructions shipped with each release are authoritative for that version.

## Updating from an older version

Unless the release notes say otherwise:

- Back up your existing configuration first.
- Replace only the RyuLink files described by the new release.
- Do not mix binaries from different RyuLink versions.
- Fully reboot after updating boot-time components.

If a release contains a breaking configuration change, it will be called out in the release notes.

## First troubleshooting checks

If two consoles cannot find or join each other, first confirm:

- Both consoles are running the intended RyuLink version.
- Both consoles joined the same RyuLink room.
- Both consoles have working Internet access.
- The game and game version are compatible with the current RyuLink beta.
- Both consoles were fully rebooted after any sysmodule update.

For reproducible problems, open a GitHub Issue using the bug-report template and include the game name, RyuLink version, network type, system environment, and reproduction steps.

## Security and legal notice

RyuLink does not require or distribute ROMs, firmware, encryption keys, title keys, or copyrighted game content. Obtain game software and system components through lawful sources.

RyuLink is an independent community project and is not affiliated with, endorsed by, or sponsored by Nintendo.
