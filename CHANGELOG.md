# Lunchtime Cozy Create and Cooking v2.6.0

A big quality-of-life update: a new storage system, a new map and claims mod, a Jobs rework where every job earns XP, better performance, and keybinds that don't clash. Boats are back to normal speed and villagers never run out of trades.

> [!WARNING]
> **Before updating:**
> - **Storage Drawers is removed.** Your drawers turn into Sophisticated Storage Limited Barrels when the world loads, with their items inside. Make a backup first just in case.
> - **Easy Villagers is removed.** Its blocks give their villagers back, and villager items become spawn eggs.
> - **Xaero's maps and Open Parties and Claims are removed.** Waypoints and claims don't carry over, so write down important coordinates and claim your land again with Ember's Teams and Claims.

## Storage: Sophisticated Storage
- **Storage Drawers → Sophisticated Storage.** Existing drawers become Limited Barrels.
- The Storage quest chapter is rewritten for Limited Barrels, Stack Upgrades, the Storage Controller and the Storage Link.
- **Carpenter unlocks** now cover Sophisticated Storage: compression upgrades at 10, stack upgrades at 15, the Storage Controller at 25, the tier 5 stack upgrade at 30.
- **Tom's Simple Storage is for everyone now:** terminals, cables, connectors, trims and inventory hoppers don't need a job. Builder still unlocks the filters, the level emitter and the Crafting Terminal.
- Crafting Terminal and Wireless Terminal: Builder 25 → 20.

## Maps and claims
- **Xaero's Minimap and World Map → Ember's Atlas.** The minimap is square, in the top left.
- **Open Parties and Claims → Ember's Teams and Claims.** Open the claims map with **'** (apostrophe). **Shift + '** opens your party and **Ctrl + '** shows claim borders.
- Map pings are on **mouse button 5**, so middle click still picks blocks.
- Walking into a claim shows its name in the action bar instead of a big title, and claim icons are half size.

## Jobs
- **Every job earns XP now.** You don't have to pick three active jobs any more. Abilities like Builder's Reach work as soon as you reach their level.
- **Lower levels for some unlocks:**
  - Brass casing and mixing brass: Engineer 20 → 10 (brass funnels, tunnels and smart chutes stay at 20)
  - Vein mining: Miner 40 → 15, bigger veins at 40
  - Furrow (3x3 tilling) at Farmer 15, Wide Furrow (5x5) at Farmer 40
  - Beekeeper: candles at 5, honey blocks at 10, honeycomb blocks at 15
- Bartender XP for brewing, pouring and tea brewing is doubled.
- Carpenter: a sapling you planted gives 10 XP when it grows into a tree.
- Quest texts are updated to match.

## Gameplay
- **Boats are normal speed again.** Small Ships no longer slows down vanilla boats. The ships themselves are unchanged.
- **Villagers never run out of trades.** This works for wandering traders too. Prices still go up and down with demand.
- Fewer zombies, skeletons, creepers and small critters, and no phantoms or mimics. These are the same rates as before, now set by the pack itself instead of Easy Mob Spawn Control. Non-op players no longer get "permission level is too low" errors from it.
- Phantoms can no longer be spawned with eggs or commands either.
- Plushies can only be earned from quests now. Sewing them is fully blocked.
- Villager spawn eggs can't be used on spawners any more. Villagers never spawned from them, so the egg was just lost.

## Miso
- The guide pages are updated for the new jobs, and there are new pages for the map and land claims.
- Miso has new tips the first time you open the map, the claim map, a waystone, the Selling Bin or a shop, and when jobs unlock vein mining, wide tilling or brass.

## Performance
- **New: Lunchtime Fixes.** It adds a performance profile switcher in the options screen (low, balanced, high, shaders), a warning for outdated graphics drivers and integrated graphics, and fixes for lag from Faunify silk moths, Punchy and Punchy Moves.
- Added **Immersive Optimization, Particle Core, Dynamic FPS and ServerCore**.
- Sodium Extras → **Chloride**. Sodium Dynamic Lights → **RyoamicLights**.

## New player setup
- **New installs start with our recommended settings:** render distance 10, simulation distance 8, GUI scale 3, FOV 90, master volume 70%, music 30%, all the pack's resource packs on, and the Lunchtime server in your server list.
- The accessibility screen and the multiplayer warning are skipped on first launch.
- This only happens on a brand-new install. Updating keeps your own settings.

## Keybinds
- **No more clashing keys:** 74 mod keybinds are sorted out on first launch. Most are unbound and a few are moved. If you change one, your choice sticks.
- **Traveler's Tool Belt** opens with **F** (Swap Offhand is on **;**)
- **Create Toolbox** wheel moved from Left Alt to **O**

## Bug fixes
- **Slow Falling potions** made on the crafting table now need an Awkward Potion. Before, any potion worked.
- **Elytra repair with leather** on the anvil is safer and can't break the anvil any more.
- Removed 4 broken coin recipes left over from an old mod (LibraryFerret). The pack now loads with 0 failed recipes.
- **Duckii paintings** and the Relics **Rage Glove, Reflection Necklace and Jellyfish Necklace** are disabled again. They came back by mistake, and their quests are removed.
- Ember's Questing no longer shows false "Unknown world" warnings when you join a server.
- The window title and crash reports show v2.6.0.

## Added
- Sophisticated Storage
- Ember's Atlas, Ember's Teams and Claims, Ember's Log Filtering
- Lunchtime Fixes
- Chloride, RyoamicLights
- Immersive Optimization, Particle Core, Dynamic FPS, ServerCore
- Croptopia (with EpheroLib)
- Bridging Mod
- ObsidianUI (library)

## Removed
| Mod | Why / replaced by |
|---|---|
| Storage Drawers and Smooth Drawers | Replaced by Sophisticated Storage |
| Easy Villagers | Villagers come back out of its blocks |
| Xaero's Minimap and Xaero's World Map | Replaced by Ember's Atlas |
| Open Parties and Claims and its PvP Support addon | Replaced by Ember's Teams and Claims |
| Easy Mob Spawn Control | Spawn rates are set by the pack now |
| Default Options | The pack sets up new players now |
| Sodium Extras and Sodium Dynamic Lights | Replaced by Chloride and RyoamicLights |
| Inventory Particles, Item Borders, Soul Fire'd, Icon Fresh | Cut to slim the pack down |
| Biome Replacer | It was already switched off |
| MossyLib | A library nothing used |

## Updated
<details>
<summary>23 mods updated</summary>

| Mod | Old | New |
|---|---|---|
| AllTheLeaks | 1.1.5 | 1.1.6 |
| Collective | 8.86 | 8.87 |
| Every Compat | 2.9.28 | 2.9.30 |
| FastALI | 2.1 | 2.2 |
| FastChunkGen | 0.43 | 0.44 |
| Field Guide | 1.24.0 | 1.25.0 |
| Gentle Seasons | 1.0.3 | 1.0.6 |
| Gnetum | 2.5.1 | 2.5.2 |
| Immersive Melodies | 0.8.2 | 0.8.4 |
| JEI | 15.74 | 15.75 |
| Kaleidoscope: Dimensions Wine | 1.1.9 | 1.1.11 |
| Kaleidoscope World Liquor | 1.1.13 | 1.2.0 |
| Lunch Worlds | 1.8.1 | 1.8.5 |
| Lunchtime's Little Cookbook | 1.0.5 | 1.0.6 |
| Miso Jobs & Careers | 1.0.7 | 1.0.12 |
| ModernFix | 5.27.93 | 5.28.0 |
| Pool Table | 1.7.0 | 1.7.1 |
| Punchy | 3.2a | 3.2b |
| Sophisticated Backpacks | 3.26.20 | 3.26.21 |
| Sophisticated Core | 1.5.33 | 1.5.37 |
| Supplementaries | 3.1.44 | 3.1.45 |
| Traveler's Tool Belt | 1.0.7 | 1.0.8 |
| Weaver's Paradise | 1.6.4 | 1.6.4.1 |

</details>

> [!NOTE]
> **Server owners:** update the mods and copy the new `config`, `defaultconfigs` and `kubejs` folders to your server. Remove Storage Drawers, Easy Villagers, Open Parties and Claims and Easy Mob Spawn Control there too. In `world/serverconfig/smallships-server.toml`, set `vanillaBoatSlowdownEnable = false` to get normal boat speed on an existing world.

Found a bug? [Open an issue](https://github.com/Miso-Studio/Lunchtime-Cozy-Create-Farming/issues).
