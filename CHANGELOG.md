# Lunchtime Cozy Create and Cooking v2.0

v2 is the biggest update yet. I wanted the pack to run smoother, feel cozier and lean more on our own mods. The quest, job and claim systems are new, a lot of mods that slowed the game down or didn't fit got cut, and there's more Create, cooking, building and exploration content.

> [!WARNING]
> **BACK UP YOUR WORLD, OR MAKE A NEW ONE FOR A BETTER AND SMOOTHER EXPERIENCE**
>
> Quests, jobs, claims, graves and several mobs were replaced, so v1.5 worlds will lose a lot of data. Back up first if you want to try anyway.

**Recommended RAM: 8 GB.** The pack uses about 6 GB of that (~75%), so there's room to spare.

## Performance
The pack starts faster, runs smoother and needs less memory than v1.5.

- Sinytra Connector and Forgified Fabric API are gone. They let Fabric mods run on Forge, but that extra layer added load time and caused most of the mod conflicts. Every mod in the pack now runs on Forge directly.
- C2ME (Forge port) is replaced by FastChunkGen, another multithreaded port of C2ME. It's faster and works better with the rest of the pack.
- Radium Reforged is now Radium Re-Reforged, the newer Forge port of Lithium. It speeds up general game logic.
- Farsight is replaced by Bobby Reforged, which caches chunks you've already seen so you can look past the server's view distance.
- Flerovium is new. It's an Embeddium add-on that speeds up item, particle and entity rendering.
- Krypton Reno is new and optimizes networking.
- Create: LazyTick is new and cuts lag from Create machines on servers.
- Dynamic FPS, FastBoot, Ksyxis, Immersive Optimization, AsyncParticles and Faster Iris Shadow Mapper were removed because they overlapped with the mods above or caused problems with them. Newer Iris versions already include the shadow mapper's speedup.
- A few heavy visual mods are out: Wakes (boat splashes), Subtle Effects (extra particles), Legendary Tooltips, Immersive UI and Chat Animation. They looked nice, but they cost FPS on mid-range PCs.
- In total the pack has 32 fewer mods and is 110 MB smaller to download.

## Quests and guides
- Ember's Questing replaces FTB Quests. Quest books are data-driven, progress is saved on the server, and resource packs can restyle the UI. It also replaces the rest of the FTB stack (Quests, UI Overhaul, Library, Teams, XMod Compat, Filter System).
- Miso's Little Guide adds welcome screens, tutorials and dialogue with Miso, the pack's mascot, to help new players get started.
- Lunchtime's Little Cookbook is an in-game cookbook that lists every food in the pack, its nutrition and every way to cook it.
- Patchouli is added for mods that ship their guides as Patchouli books.
- Bosses and quest enemies have double health. That covers the Ender Dragon, the Wither, the Warden and every L_Ender's Cataclysm boss, which went down too fast once you had good gear.
- Plushie Buddies used to be a crafting recipe and are now a collectible quest line.

## Jobs and economy
- Miso Jobs & Careers replaces Jobs+. You pick a job (Farmer, Miner, Chef or Rancher) and earn XP by doing that work. Leveling up unlocks recipes, tools and machines, so your job now decides how you progress.
- Create: Numismatics replaces Shoppy. It's a Create-style currency that works with redstone, and the coin recipes and exchange rates are balanced for survival.

## New mods
Create
- Numismatics: coins and currency
- Liquid Fuel: pipe liquid fuel into blaze burners
- Pantographs & Wires: catenary wires and pantographs for electric trains
- Create Cobblestone: a stress-powered cobblestone generator that doesn't lag like a lava-and-water one
- Schematic Checker: fixes broken schematics

Food and drink
- [Let's Do] HerbalBrews: new flowers and tea brewing
- [Let's Do] Brewery: beer brewing and pretzels
- Pizza Delight: pizzas for Farmer's Delight

Building and decor
- Effortless Building: mirror, array and build-mode tools
- Every Compat (Wood Good and Stone Zone): other mods' blocks in every wood and stone type
- Fairy Lights: string lights, bunting and garlands
- Pool Table: a playable 8-ball table with real ball physics
- Vista: TV and camera blocks

Storage
- Tom's Simple Storage: a vanilla-style storage network, a cheap early-game option before Create logistics. The Create: Better Tom's Storage GUI resource pack restyles it to match Create.

Exploration and world
- MVS (Moog's Voyager Structures): 160+ vanilla-style structures with loot
- Explorify: vanilla-friendly dungeons and structures
- YUNG's Better Witch Huts: reworked swamp witch huts
- Spelunkery+: Spelunkery support for other mods' ores
- Mining Utility: Reforged: mining helpers like the Escape Rope and mining helmets
- Biome Replacer: swaps biomes at the pack level
- Lunch Worlds: custom Lunchtime content, a hound boss with its own summon item and trophy

Mobs
- Naturalist: new overworld wildlife with its own behaviors

Atmosphere
- Gentle Seasons: longer days, shorter nights and more rewarding rain
- ATMOSPHERICS: an in-game editor for fog, sky, clouds and stars (press B)
- Weather Glass: rain, frost and sand show up on glass
- Soul Fire'd: soul fire gets its own damage and enchantments

Player and QoL
- Punchy! Moves: third-person animations, a shoulder camera and emotes, built on Punchy
- Weavers Paradise: make thread and fabric, then dyeable clothing
- Corpse (with Curios compat): your items stay in a corpse when you die, Curios slots included
- Open Parties and Claims (with PvP Support): parties, chunk claims and forceloading, shown on Xaero's map
- Snail Mail: send packages to friends with envelopes and stamps
- Ok Zoomer: configurable zoom
- Auto Stack Refill: refills an empty hotbar slot from your inventory
- e4mc: open your world to friends over the internet without port forwarding

Resource packs
- Soft Weather: rain and snow get in the way less
- Alternative Rain Sounds: new rain and thunder sounds

## Replaced
| Old | New | Why |
|---|---|---|
| Better Days (day length, faster sleep) | Gentle Seasons | Longer days and shorter nights, and rain is worth having |
| GraveStone and the Better Gravestones resource pack | Corpse with Curios compat | Also keeps items in Curios slots |
| FTB Chunks (with Xaero compat) | Open Parties and Claims | Parties, claims and forceloading in one mod, with Xaero's map support and optional PvP |
| Mighty Mail | Snail Mail | Packages, envelopes and stamps fit the cozy style better |
| WI Zoom | Ok Zoomer | Configurable zoom |
| e4all (unofficial fork) | e4mc | The official version |
| Shoulder Surfing, Not Enough Animations, Touch'n Motion | Punchy! Moves | One mod covers the animations and the camera |
| Alex's Mobs (with Alex's Delight, Relics compat and the Sweety's Items resource pack) | Naturalist | Calmer, vanilla-style wildlife for a cozy pack |
| Create: Easy Stone Generators | Create Cobblestone | A stress-powered generator that fits Create progression |

## Removed
- Creeper Overhaul and Enderman Overhaul added biome variants of creepers and endermen, and they added a lot of lag.
- Bosses'Rise is an MCreator mod. It didn't fit the pack and it caused lag.
- Dungeon Now Loading was cool, but too buggy to keep.
- Bosses now come from Cataclysm and the quests, with double health.
- Goblin Traders and Chef's Delight (Chef and Cook villagers for Farmer's Delight).
- Create: Misc & Things, Realm RPG Treasure Balloons, Jumpy Boats, Bridging Mod, Underlay, Visual Workbench, RightClickHarvest, Villager Names and Item Restrictions were small features, cut to slim the pack down.
- Streams Reflowing (world-generation rivers and streams) caused lag.
- Cool Rain is replaced by the Alternative Rain Sounds resource pack.
- Fresh Animations and its Player Extension animated every entity and cost too much FPS.
- No Chat Reports, Resource Pack Overrides and Cubes Without Borders aren't needed anymore.
- Insanity Shader.
- Libraries nothing uses anymore: Arc Lib, Majrusz Library, Modonomicon, Lithostitched, Blueprint, CorgiLib and others.

## Updated
- Forge 47.4.28 to 47.4.29
- 30 mods, including Sophisticated Backpacks and Sophisticated Core, ModernFix, Punchy (2.8 to 3.2), Too Many Bows, Kaleidoscope Chinese Food and Immersive Eating, FancyMenu, Exposure, Field Guide, Moonlight and Collective.

## Config and balance
- Phantoms are gone, because they punished long building and cooking sessions. Recipes that used phantom membrane now use other items.
- Artifacts mimics are disabled. Losing loot to a surprise chest isn't cozy.
- Zombies, skeletons and creepers spawn 30% less, so nights are calmer.
- MVS replaces vanilla desert and jungle temples with its own versions.
- Elytra can be repaired at an anvil, since there are no phantoms to farm membrane from.
- The Mining Utility mining helmet has a new crafting recipe.
- Fairy Lights can't be crafted. All of their recipes were removed.
- Waystones, Easy Villagers and Numismatics recipes are rebalanced, so fast travel and automation show up at a fair point in progression.
- Recipes and tags are unified across mods. Each ingredient is one item, which gets rid of duplicates and broken recipes.
- Fixed broken Kaleidoscope furniture textures from Every Compat, an Ember's Questing world-loading issue, and Punchy keybinds resetting to defaults.
- Particular's waterfall particles (cascades) are off, for FPS.
- New main menu, loading screen and update screen.
