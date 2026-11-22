# WoW Forever fixes

Small fixes and tweaks to World of Warcraft: Forever addons, as Patch Keeper snippets.
Patch Keeper applies them to your installed addons and puts them back automatically
when an addon update wipes them.

| Snippet | Addon | What it does |
|---|---|---|
| `polestar-rare-fallback` | Polestar | Rare mobs are only used as a fallback drop source, so guide steps stop sending you to a rare when ordinary mobs drop the item (A Recipe For Death, Wild Hearts and about 70 other objectives). |
| `polestar-guide-rare-steps` | Polestar guides (Horde, Alliance) | Five written guide steps that named a rare now name the ordinary mobs. |
| `flbis-daylight` | Forever Leveling BiS | A "Daylight" theme: the Modern layout in DaylightUI's look, colors, accent, window frame and font. |
| `polestar-danger-roads` | Polestar (GPS) | In zones 4+ levels above you, walks keep to the roads: off-road ground costs 3 times more there, so the arrow follows a road and leaves it only for the last stretch to the target. Also applies in the zone you start in and the one you're heading to. |

## Using them

In Patch Keeper: **Add…**, paste this repo's link, pick the snippets you want.

Each snippet only changes files of the addon it targets. Patch Keeper shows the exact
change before installing anything, and can undo every snippet cleanly.

## Format

`patchkeeper.json` lists the snippets. Each one is a JSON file: what it targets, the
addon versions it was tested with, and its operations. Each operation edits the addon
at an exact piece of its code (an *anchor*). If an update changes that code, the snippet
is reported as needing an update and nothing is touched.
