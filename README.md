# MainSequence-BeltMerger

Three tiers of belt merger with three inputs, one output through the orange-marked face, and selectable input priorities.

## Release status

The existing private implementation and MSCore migration have been tested in game. **No public installable release is available yet.** Asset packaging is being revised to use the installed game assets without distributing extracted asset copies. Do not add this repository in Manager until a release is published.

The existing implementation already references the game's splitter actor, model, materials and icons. Its separate machine definitions and hologram arrows still require replacement or a verified runtime solution. Existing merger class paths and saved identities must remain compatible. No game-derived assets are included in this repository.

## Planned requirements and use

Main Sequence, single-player; MSCore 0.8.13, compatible UE4SS and MainSequence-Framework 0.3.3. Select Merger Mk. 1/2/3 from Build -> Logistics as the corresponding splitter technologies unlock. Configure input priorities with the interaction panel. The output is on the orange-marked face.

## Existing users

Keep your working private merger installation and saves while the public package is being prepared. Removing its custom definitions can affect placed mergers. This repository is documentation only and does not replace your installed assets.

## Credits and licence

Our original code and documentation are MIT-licensed (see LICENSE). Game assets and third-party software are excluded. Developed with OpenAI Codex; uses MSCore by xxalex3xx97 and UE4SS. Unofficial; not affiliated with the game developer. Private source, extracted data and user saves are not uploaded.
