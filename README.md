# Capri Night City

Source and separate Cyber Engine Tweaks bridge for Capri's Cyberpunk 2077 integration, by **NoxEterna**. Version **1.9.4**.

## Separate game-side download

[Download the CET bridge](https://github.com/SzentiX/capri-night-city/releases/tag/v1.9.4), then follow [BRIDGE-INSTALL.md](BRIDGE-INSTALL.md). The ZIP contains only the game bridge, a manual installation guide and checksums. Install the Capri client through Capri's mod directory; connect it using `night city connect`.

**This external download and this repository's Lua/PowerShell files are separate from the Capri mod directory review and have not been checked by its reviewers.** The directory submission contains only the `.capri-code` client, README and preview. Do not infer approval of the game-side files from a directory listing.

## Features and commands

Nearby/group NPC hacks, native scanner tags, vehicles/devices/access points, eight custom NPC programs, Protect Me, stealth, optional chaos, silent incoming-netrunner defense and rescue below 50 raw HP. See [COMMANDS.md](COMMANDS.md) and [HACKS.md](HACKS.md) for targeting, aliases, cooldowns and limits.

General phrases such as `stop it`, `open it`, `scan`, `calm down`, `go quiet`, `protect me` and `do your thing` are owned by this mod only with a fresh, loaded, unpaused game link. They pass through to Capri while the link is absent, stale, waiting for a save or in a menu. Use an explicit `night city` prefix for offline controls, such as `night city status`, `night city connect`, `night city help` or `night city quiet`. Namespaced game commands can also be written as `night city scan` or `night city protect me`; an offline action reports the unavailable link.

Contextual reports use your configured Capri brain/provider, which receives the selected game facts if it is a cloud provider. No API key or separate telemetry service is bundled. The separate ElevenLabs agent route may bypass Capri's code-mod commands; typing or Capri's normal local-brain voice dispatch can be used. Internal Capri reporting interfaces can change between versions.

## Source and validation

`Build.ps1` runs Lua syntax/game mocks, C#/protocol and C#/Lua cross-process fixtures, optional compilation against installed Capri, and guarded installer/rollback fixtures. It produces the separate CET-only ZIP in `out`. `Install.ps1` and `Uninstall.ps1` are optional source utilities, with explicit game selection, backups and hash-guarded rollback; they are not needed for manual bridge installation.

See [VALIDATION.md](VALIDATION.md) for the evidence and live-runtime limits. Automated results do not establish gameplay, native HUD effects, voice quality or leak-free operation.

Credit: [Capri Desktop by lachydotmcg and contributors](https://github.com/lachydotmcg/capri-desktop). Unofficial fan integration; no game assets or credentials are included.