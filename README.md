# SFM-GameRefs
Reference-only SecretFlasherManaka / BepInEx 6 assemblies for CI builds of the SFM mods: every method body replaced by
`throw null`, resources removed - the API surface only, no game code. Made with sfm-modkit's `./tools/dev.ps1 gamerefs` and
attached to releases as `SFM.GameRefs.<version>.nupkg`; the mods' `build/ci.py gamerefs` downloads it without a token.

Only for compiling mods; to play, you need the game itself.

Also included: the API of the Custom Missions v2 plugin (`BepInEx/plugins/SFM_custom_mission_v2.dll`, stripped the same way),
so mods with an optional Custom Missions integration (RestraintHub's phone app) build in CI.
