# Zygor-CoA — Conquest Reborn Quest Guides & Reference Tools

**Current integration package: v1.0.10 (research integration; in-game validation pending).**

> **[Download](https://github.com/uncle-bone/Zygor-CoA/releases/latest)**

Zygor-CoA adapts **Zygor Guides Viewer Remastered** for **Ascension Conquest of Azeroth / Conquest Reborn**, based on the WoW 3.3.5a client. It retains Zygor's native guide browser, step tracker, waypoint arrow and settings while adding CoA-specific quest research, custom-class support and reference tools.

## Guide scope

The **new guide development scope is Vanilla Azeroth and Conquest Reborn custom content only**. **Outland/TBC and Northrend/Wrath guides are not part of the new CoA guide-development scope.** Existing upstream files may remain in the distribution for compatibility; their presence is not a promise of current CoA support.

The current Pale Reach research integration includes **237 quest records**, **134 recorded prerequisite relationships**, and **41 coordinate records reported for 32 quests**. These figures describe research data, **not** 237 verified live-realm quests or a fully routed leveling guide. The generated Pale Reach guide remains experimental: objective and turn-in routing, waypoint coverage, quest availability and mid-zone resume behavior require additional verification. Pale Reach's **18–60 scaling range applies only with level scaling enabled**.

## Features

- Native Zygor guide browser, quest-step display, automatic advancement and waypoint system; no separate CoA guide-manager window.
- Existing bundled guide content plus experimental Conquest Reborn guide integration.
- CoA custom-class stat weights, talent-advisor integration and Gear Finder support.
- CoA map translations and observed quest/NPC/reward/spellbook data.
- Searchable historical quest, NPC, item, spell and talent reference archive.
- Optional bounded `ZGCOA1` contact sharing on LootCollector's existing channel **only if already joined**; the addon does not join, leave or replace channels.
- Existing Blizzard UI, DragonUI and ElvUI compatibility is a goal; combinations require in-game testing.

## Installation

1. Back up `Interface/AddOns/ZygorGuidesViewerRM` and your `WTF` SavedVariables.
2. Download the latest **verified release asset** from [GitHub Releases](https://github.com/uncle-bone/Zygor-CoA/releases). The v1.0.10 integration ZIP was prepared separately; **do not assume it is published on GitHub until a matching release asset appears**.
3. Extract the single `ZygorGuidesViewerRM` folder into `Interface/AddOns`. Do not rename the folder.
4. If upgrading from an older multi-addon archive layout, back up and remove obsolete `ZygorCoAArchive_items`, `_npcs`, `_quests`, `_spells`, and `_talents` addon folders if they are still installed separately.

## Commands (diagnostics and reference lookups)

- `/zcoa` — help/version; `/zcoa log` — quest observations; `/zcoa peers` — received contacts.
- `/zcoa quests <ID or name>`, `/zcoa npcs <ID or name>`, `/zcoa items <ID or name>`, `/zcoa spells <ID or name>` — reference lookups.
- `/zcoa talents <tree name>` — historical talent references.
- `/zcoa sharing off`, `/zcoa tooltips off` — disable optional functions; use `on` to restore.
- `/zcoa export`, `/zcoa import <ZGCOA1 line>` — contact-record exchange.

## Development status

**Experimental, not a certified complete-zone guide library.** Source/ZIP integrity and guide registration checks do not establish in-game correctness. Some historical records may not match current Conquest Reborn content; quest coordinates and NPC contact sightings may be approximate. The guide's arrow requires actionable coordinates and valid Zygor steps. Do not interpret an accepted guide registration as proof of a playable route.

Research inputs include [Questie-X](https://github.com/downingwow/Questie-X), [CoA-Research](https://github.com/downingwow/CoA-Research), and archived Ascension datasets. See bundled provenance and licensing files. Original viewer by **Sinus Pi**; third-party credits and license requirements remain in force. No affiliation with the upstream projects is implied.

## Support

Target client: **Conquest Reborn / WoW 3.3.5a (Interface 30300)**. When reporting an issue, include the addon version, exact Lua error, active UI/map addons, and the guide/quest ID.

**Maintainer:** Uncle Bone · [GitHub contact](https://github.com/downingwow) · [Repository](https://github.com/uncle-bone/Zygor-CoA)
