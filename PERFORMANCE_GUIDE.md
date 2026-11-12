# Lunchtime Performance Guide

Lunchtime Cozy Create and Cooking v2 is a large Forge modpack for Minecraft 1.20.1, with 372 mods, resource packs and shaders. v2 is lighter than v1.5: it has 32 fewer mods, no Fabric compatibility layer, and new defaults tuned for Create bases. This guide covers RAM, settings, shaders and how to find the cause when the game slows down.

## Quick fixes

If the pack feels slow, try these in order:

1. **Let the first launch finish.** The first start after installing or updating takes the longest. On an Apple M1 Pro with 16 GB of RAM, v2 takes about 80 seconds to reach the main menu.
2. **Use Java 17 (64-bit).** Let CurseForge or your launcher use its bundled Java.
3. **Allocate 8 GB of RAM.** See [RAM and Java](#ram-and-java).
4. **Turn shaders off** while you test. Shaders are the biggest FPS cost in the pack.
5. **Keep the default distances** (render 10, simulation 8), or lower them if you still lag.
6. **Don't add extra optimization mods or JVM flags.** The pack already includes the ones below, and replacements can conflict with them.

## RAM and Java

**Allocate 8 GB.** In normal play the pack uses about 6 GB of that (around 75%), so the rest leaves room for busy moments like exploring new terrain.

| Your total system RAM | Allocate to Minecraft |
|---|---|
| 8 GB | Not recommended. Try 6 GB with shaders off and low distances |
| 16 GB | 8 GB (recommended) |
| 32 GB or more | 8 to 10 GB |

- Don't give Minecraft all of your RAM. Your system, the launcher, Discord and your browser need memory too.
- More RAM isn't always faster. Above about 10 GB, garbage-collection pauses can get longer and cause stutter.
- Use your launcher's memory slider instead of copying JVM flags from other guides.
- After changing RAM, restart the game completely before you test again.

## Default settings in v2

v2 ships with these defaults. They give steady TPS in big Create bases on mid-range PCs.

| Setting | v2 default | Notes |
|---|---:|---|
| Render distance | 10 chunks | Bobby Reforged keeps chunks you've already seen visible farther out |
| Simulation distance | 8 chunks | The biggest factor for tick lag with Create contraptions and farms |
| Shader shadow distance | 6 chunks | Set in Oculus. Shadows cost a lot of GPU time |
| Default shader | Complementary Reimagined | Complementary Unbound and Photon are also included |

On a low-end PC, try these:

| Setting | Try | Why |
|---|---:|---|
| Render distance | 6 to 8 chunks | Fewer chunks to draw |
| Simulation distance | 5 to 6 chunks | Fewer chunks ticking around you |
| Entity distance | 50 to 75% | Draws entities over a shorter range |
| Particles | Decreased | Less work in busy scenes |
| Shaders | Off | Shaders can cost more than everything else combined |
| Clouds | Off | One less layer to draw |

Change one setting at a time and test in the same place in the same world. Moving into new terrain makes the game generate chunks, which isn't a fair FPS comparison.

## Shaders

Lunchtime includes three shader packs. Pick one in **Options → Video Settings → Shader Packs**.

- **Complementary Reimagined** is the default, with a vanilla-like look.
- **Complementary Unbound** is the other Complementary style.
- **Photon** is a separate shader pack with its own lighting.

If your FPS drops with shaders on, lower the shader profile in its settings first, then lower the shadow distance. Turn shaders off completely when you're troubleshooting.

## Performance mods in the pack

These mods are already in Lunchtime v2. You don't need to add anything.

**Rendering (client)**

| Mod | What it does |
|---|---|
| Embeddium | Faster terrain rendering. Most other rendering mods build on it |
| Flerovium | Embeddium add-on that speeds up item, particle and entity rendering |
| ImmediatelyFast | Speeds up immediate-mode rendering like the HUD, text and items |
| Entity Culling | Skips drawing entities and block entities you can't see |
| More Culling Reforged | Skips drawing block faces and objects you can't see |
| Gnetum | Spreads HUD updates over several frames |
| Bobby Reforged | Caches chunks you've seen so you can view past the server's view distance |
| BadOptimizations | Small client-side optimizations outside of rendering |

**Memory and loading**

| Mod | What it does |
|---|---|
| ModernFix | Memory, loading and bug fixes. v2 turns on its dynamic resources option to lower RAM use |
| FerriteCore | Lowers memory use of game data |
| AllTheLeaks | Fixes memory leaks in Minecraft and some mods |
| Jasione | Reduces garbage-collection pressure |
| quick pack | Loads zipped datapacks and resource packs faster |
| Async Logger | Moves logging off the main thread |

**World generation and ticking**

| Mod | What it does |
|---|---|
| FastChunkGen | Multithreaded chunk generation, loading and saving |
| Radium Re-Reforged | Forge port of Lithium, speeds up general game logic |
| Fast Noise | Faster world-generation noise |
| Structure Layout Optimizer | Faster structure placement |
| Feature Recycler | Prevents crashes between world-generation mods |
| Create: LazyTick | Cuts lag from Create machines |
| Mobtimizations | Cheaper mob AI |
| Let Me Despawn | Lets more mobs despawn so they don't pile up |
| Alternate Current | Faster redstone dust |
| FastFurnace, FastWorkbench, FastSuite | Faster furnace, crafting table and recipe lookups |
| Fast Item Frames, Fast Paintings | Cheaper item frames and paintings |
| Fastvancements, FastALI | Faster advancements and loot info |

**Network and tools**

| Mod | What it does |
|---|---|
| Krypton Reno | Optimizes the network stack |
| Chunky | Pre-generates terrain on servers |
| spark | Profiles lag so you can see what's causing it |
| MixinTrace Resmithed | Adds mixin details to crash reports |

### What changed from v1.5

- **Sinytra Connector and Forgified Fabric API were removed.** All mods now run on Forge directly, so loading is faster and there are fewer conflicts.
- **C2ME was replaced by FastChunkGen**, and **Radium Reforged by Radium Re-Reforged**.
- **Farsight was replaced by Bobby Reforged.**
- **Dynamic FPS, FastBoot, Ksyxis, Immersive Optimization, AsyncParticles and Faster Iris Shadow Mapper were removed.** They overlapped with the mods above or caused problems with them.
- **Heavy visual mods were removed:** Fresh Animations, Wakes, Subtle Effects, Legendary Tooltips, Immersive UI and Chat Animation.
- **Creeper Overhaul, Enderman Overhaul, Bosses'Rise and Streams Reflowing were removed** because they added lag.
- Particular's waterfall particles are off by default.

## Dedicated servers

Start with these values in `server.properties` and adjust them for your player count:

- `view-distance=8`
- `simulation-distance=6`

Server RAM depends on player count, how much new terrain gets generated, and how many Create machines are loaded. 6 to 8 GB is a reasonable start for a small group of friends. Watch real use with spark before you raise it.

### Pre-generate terrain with Chunky

Generating new terrain is the heaviest thing a Lunchtime server does. Pre-generate an area around spawn before players spread out:

```text
/chunky center <spawnX> <spawnZ>
/chunky radius 3000
/chunky start
```

Run it while the server is empty, and back up the world first.

### Profile lag with spark

If the server has lag spikes or low TPS, run spark while the lag is happening:

```text
/spark profiler start --timeout 120
```

Keep playing normally for two minutes. spark then gives you a link to a report that shows which mod or machine is using the tick time. Use `/spark profiler stop` to end it early.

## Find the cause

**Low FPS, but the world runs at normal speed**
- Turn off shaders, then lower render distance, entity distance and particles.
- Check that Minecraft is using your dedicated graphics card.
- Close other GPU-heavy apps.

**Stutter while exploring**
- This is usually chunk generation. Lower render distance for a while, or pre-generate on a server.
- Go back to the same area after it has generated and compare.

**Server lag, rubber-banding or slow machines**
- Check whether everyone has it or only you.
- Lower simulation distance.
- Run a spark profile while it's happening. Large Create contraptions, mob farms and lots of item entities are the usual causes.

**Crashes or very long loading**
- Read `logs/latest.log` or the crash report and look for the first real error.
- Make sure you're on the matching Minecraft (1.20.1), Forge (47.4.29), Java (17) and Lunchtime versions.
- Remove any mods you added yourself before you report a pack bug.
- Back up your world before changing mods on an existing save.

## Asking for help

When you report a performance problem, include:

- Lunchtime version and launcher
- Minecraft, Forge and Java versions, and how much RAM you allocated
- Single-player, a hosted LAN/e4mc world, or a dedicated server
- Your CPU, GPU and total RAM
- Whether it's low FPS, stutter, server TPS or a crash
- `latest.log`, the crash report, or a spark link

Remove passwords, tokens and IP addresses from logs before sharing them. Report bugs on [GitHub Issues](https://github.com/Miso-Studio/Lunchtime-Cozy-Create-Farming/issues) or ask in the [Lunchtime Discord](https://discord.gg/68yhDdFpnx).
