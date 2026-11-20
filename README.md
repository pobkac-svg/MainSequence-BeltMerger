# MainSequence Belt Merger

Adds Merger Mk. 1/2/3 to Build -> Logistics: three belt inputs combine into one output through the orange-marked face. Set a preferred input or use balanced flow.

## Requirements

- Main Sequence, single-player.
- [MSCore 0.8.13](https://github.com/xxalex3xx97/MSCore/releases/tag/v0.8.13) and compatible UE4SS.
- [MainSequence-Framework 0.3.3](https://github.com/pobkac-svg/MainSequence-Framework).

Tested with UE4SS 4.0.0 and the user's current game update. Other builds and multiplayer are not verified.

## Install and update

Save and close the game. Install Framework first, then add `pobkac-svg/MainSequence-BeltMerger` in MSCore Manager and install. Fully restart after updates. Disable the old standalone merger mod.

The ZIP contains `Mods/MSF_BeltMerger` and the matching `.pak/.utoc/.ucas` triple in `Paks/~mods`. Manager places these under the game's `ue4ss/Mods` and `Content/Paks/~mods` respectively. Keep the three files together; do not install another copy in the parent Paks directory. Do not install the editor project, stand-in classes/material, global container or development tools.

## Use

Choose a tier in Build -> Logistics. Each tier unlocks with its corresponding splitter technology. Feed three inputs and route the merged output away from the orange-marked face. Press F while looking at the merger to configure priorities; F6 also cycles input preferences. Rates and costs come from the corresponding installed splitter tier. Ordinary splitters retain their original behavior and filters.

## Assets and compatibility

Version 0.3.0 replaces the private cloned definitions with original authored merger definitions and a simple original arrow mesh. The merger inherits the installed splitter tier classes and references the game's model, materials and icons. The game assets themselves are not bundled. No vanilla registry/research overrides, shader maps, native editor module, source templates or global container are shipped.

Legacy and current merger identities/paths are retained for existing saves. Integration with our Machine Blueprints and Walk Through Logistics addons is preserved. Existing mergers, build menu, priorities and behavior were accepted in game by the user on 20 November 2026; startup logs confirm all four definitions registered and native preflight passed. Independent container/asset inspection and Lua regression checks also passed. Normal cost metadata is copied from the installed splitter tier; this replacement test was in Creative mode, so a separate post-replacement non-Creative purchase was not recorded.

## Removal and troubleshooting

Keep a save backup and remove placed mergers before uninstalling their custom definitions. Close the game before Manager removal and fully restart after changes. Removing a mod does not undo construction already saved. Keep Designs and underground companion files when updating other addons.

Check `ue4ss/UE4SS.log` and `Mods/MSCore/selfcheck.log`. MSCore 0.8.13 has a known missing unused ship-renaming helper, and its executable-size check reports the installed game update; this mod does not use ship renaming.

## Credits and licence

Original mod code, documentation and the procedural arrow mesh are MIT-licensed; see LICENSE. Developed with OpenAI Codex. MSCore by xxalex3xx97 and UE4SS are external dependencies. Authored/cooked with Unreal Engine 5.7.4; installed game models/materials/icons are referenced under their own terms and excluded from our MIT grant. Unofficial; not affiliated with the game developer.

This repository contains release documentation. Runtime files are attached to releases; private development history, extracted data and user saves are excluded.
