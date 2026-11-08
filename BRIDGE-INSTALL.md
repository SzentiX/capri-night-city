# Capri Night City: separate CET bridge

By NoxEterna. Version 1.9.4, wire protocol 1.

This is an external Cyberpunk 2077 download. It is separate from the Capri mod directory submission and has not been checked by that directory's reviewers. Source: https://github.com/SzentiX/capri-night-city .

1. Install Cyber Engine Tweaks (CET) for your Cyberpunk version from its official distribution.
2. Close Cyberpunk. Extract the archive and copy only `CapriNightCityBridge` to `<Cyberpunk 2077>/bin/x64/plugins/cyber_engine_tweaks/mods/CapriNightCityBridge`. That folder must contain `init.lua`, `core.lua`, `targets.lua`, `counter.lua`, `programs.lua` and `settings.json`. Back up an existing bridge folder first; preserve your customized settings when updating.
3. Install/enable **Capri Night City** from Capri's mod directory, approving the code mod in Capri.
4. In Capri, say/type `night city connect` and choose the installed **CapriNightCityBridge** folder containing `init.lua`.
5. Start Cyberpunk, load a save and close the menus. Check `night city status`. Short commands such as `scan` and `protect me` work only while the game link is live. Explicit `night city …` commands also work for setup and offline diagnostics.

This archive contains only the CET bridge, this guide and file hashes; no PowerShell execution or Capri client installation is needed from this archive. The full source repository also contains optional guarded install/rollback scripts and automated tests; those are external to the Capri mod directory review.

To remove: disable Capri Night City in Capri, close Cyberpunk and remove only the `CapriNightCityBridge` folder. Restore your backed-up bridge if applicable. Completed game consequences such as deaths or explosions are not undone.

Ordinary/group hacks share an eight-second cooldown; Blackwall has a separate 180-second cooldown. Default range is 35 m. Emergency rescue arms below 50 raw HP, with a 120-second cooldown; it is not a 50-percent-health trigger. Protected targets and V's occupied car are skipped. Commands operate on game-exposed eligible targets and native actions. Upload acknowledgements are requests, not proof of a rendered effect. Live gameplay and native HUD/effect behavior remain unverified by automated tests.
