# Lunchtime Cozy Create and Cooking v2.5.1

A cleanup and bug-fix update: a faster recipe viewer, a fix for an item-duplication bug, fewer duplicate items between mods, and some Quark content turned back on.

**⚠️ Before updating: take your tools out of the Inventorio tool belt and utility belt, or you'll lose them.** Inventorio has been removed. Existing v2.5 worlds are otherwise safe to update.

## Recipe viewer: EMI → JEI
The pack now uses **JEI** instead of EMI. It loads much faster and feels lighter in game, and almost every mod in the pack supports JEI directly.

- EMI → **Just Enough Items (JEI)**
- EMI Ores → **Just Enough Resources**
- EMI Professions → **Just Enough Professions**
- EMIffect and EMI Enchants → **Just Enough Effect Descriptions**
- Create EMI, EMI Create Schematics, EMI Let's Do Compat, Distraction Free Recipes and TMRV are removed, because nothing needs them with JEI
- **New:** Just Enough Breeding shows what each animal eats to breed

## Bug fixes
- **Fixed items being duplicated or deleted by the tool belt.** Inventorio's tool belt could copy a tool into your selected hotbar slot and delete whatever was there. This is a known Inventorio bug with no fix available, so Inventorio is removed and **Traveler's Tool Belt** replaces it. It's an upgradeable tool belt in a Curios slot with quick-swap.
- **Fixed structures not spawning.** The biome replacer stopped IDAS, L_Ender's Cataclysm and other structures from generating, so it's switched off. Regions Unexplored biomes still generate normally.
- **Carry On** can no longer pick up corpses or rope blocks. Picking them up could break them or lose items.
- Crash reports and the window title now show the right version, v2.5.1.

## Less duplicate content
17 Quark features are back on, because no other mod in the pack adds them:
- **Building:** Gold Bars, Raw Metal Bricks, Industrial Palette, Rainbow Lamps, Celebratory Lamps, Duskbound Blocks, Wooden Posts, Nether Brick Fence Gate
- **Items:** Torch Arrow, Skull Pikes, Ambient Discs, Endermosh Music Disc, Pathfinder Maps, Bottled Cloud, Glass Shard, Dyeable Item Frames
- **Redstone:** Redstone Randomizer

Quark features that another mod already provides stay off: Framed Glass (Create), Soul Sandstone (BetterNether), crates (Farmer's Delight), extra brick, mud and stone variants (Chipped), Leaf Carpet (Regions Unexplored), Vertical Slabs (Supplementaries), Dragon Scales (Butchery and Dragon Loot), Totem of Holding (Corpse) and Iron Rod (Pantographs & Wires).

WI Zoom is replaced by **Ok Zoomer**, so the pack has a single zoom mod.

## Added
- Traveler's Tool Belt
- Straw Statues: player statues for your builds
- Windy: Configurable, for wind effects
- JEI, Just Enough Resources, Just Enough Professions, Just Enough Effect Descriptions, Just Enough Breeding
- Ok Zoomer

## Removed
- Inventorio: item dupe and delete bug
- EMI and its addons, and TMRV: replaced by JEI
- WI Zoom: replaced by Ok Zoomer
- Sodium Options API and TxniLib: libraries that no mod uses anymore

## Updated
- Ember's Questing 1.8.0 → 1.9.0
- Lunchtime's Little Cookbook 1.0.4 → 1.0.5
- Lunchtime Jobs 1.0.6 → 1.0.7
- Miso's Little Guide 1.7.3 → 1.7.4
- Fancy Tab Sections 6.2.3 → 6.3
- Structure Layout Optimizer 1.0.11 → 1.0.12
- Weather Glass 0.6.0 → 0.6.2

## Quests and UI
- The quest book button in your inventory is now a rose ribbon, between your player model and the crafting grid.
- Cleaned up duplicate and leftover files in the quest pack.
- The minimap moved to the top left of the screen, and the FPS counter moved to the right.

**Server owners:** update the mods and copy the new `config` folder to your server, and remove Inventorio and the EMI mods there too.
