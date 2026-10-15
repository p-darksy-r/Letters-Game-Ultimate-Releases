<!-- Copyright (c) 2026 p-darksy-r. All rights reserved. -->

# Letters Game Ultimate Releases

Public playtest channel for **Letters Game Ultimate**. Versions below v1.0.0 are development builds, not the final Steam release.

## Download and Play

Open [Releases](https://github.com/p-darksy-r/Letters-Game-Ultimate-Releases/releases) and choose one of these assets:

- **Windows:** download `Letters-Game-Ultimate.exe` and double-click it. No Node.js, npm or administrator account is required. First launch extracts the portable runtime.
- **Browser:** download `Letters-Game-Ultimate-Web.zip`, extract the entire folder, and open `index.html` in Edge, Chrome or Firefox. No installer, executable or certificate is needed. Keep the folder in one place and export your progress in Profile & Save before moving or replacing it.

Native and browser progress are separate. Use profile export/import to transfer a save. The browser runtime's HTML/JavaScript/assets are included in the downloads; the development repository, build tools and private keys are not published here.

## Current Build and Limitations

Current build: **v0.19.1**, a Windows development playtest. Steam distribution is reserved for v1.x.x.

- 14 categories, eight difficulties up to 40x40, and Campaign, Daily and Custom modes.
- Eight languages, hints, coloured word selection, achievements, skins and milestone credits.
- Native profile recovery and profile export/import. Browser profiles are stored separately.

**Unfinished puzzles are not restored after closing the game.** Profile statistics, credits, unlocks and settings are saved; Continue only resumes the puzzle within the currently open session.

Resolution, FPS and VSync selections are stored but do not yet control the native window/renderer. Complete keyboard/controller play and Steam Deck compatibility are not validated. Automated checks do not replace human translation review or testing on independent PCs.

The next proposed development priorities are unfinished-puzzle recovery, safer shortcuts and full gameplay/save/reward tests, followed by effective video settings and broader accessibility. These are planned improvements, not features already shipped.

## Feedback

Report the game version, Windows/browser version, language, mode, difficulty and exact steps to reproduce. A screenshot is helpful. Do not upload private certificates, keys or your full Windows profile. Export a profile backup before changing versions or moving the web folder.

## Windows Security

The v0.19.1 executables use a personal **self-signed development certificate**, not a publicly trusted publisher identity. They passed launch tests on the developer's Windows PC, but SmartScreen, Smart App Control or managed policies may still warn or block on other computers.

**Do not disable Windows protections or install a developer certificate.** Use the browser package if the Windows executable is blocked. A publicly trusted signing solution remains a release-preparation task.

## Updates

`update-manifest.json` identifies the current portable build and its SHA-256. For the optional native updater, keep this layout, close the game, and run `update.exe`:

```text
update.exe
app/
  Letters-Game-Ultimate.exe
  update-manifest.json
```

Download the updater and manifest from the same release. The updater fetches the public manifest and verifies the downloaded application's SHA-256 before replacement.

<!-- End copyright (c) 2026 p-darksy-r. All rights reserved. -->