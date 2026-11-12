# Troubleshooting

Try these checks before reinstalling the pack or deleting a world. They solve many common problems and help the team identify real bugs.

## The game will not launch

1. Confirm that the launcher installed the correct Lunchtime release.
2. Check that the Minecraft version, Forge version, and Java runtime match that release.
3. Test without extra mods, shaders, or resource packs that you added yourself.
4. Read the crash report and logs. Look for the first meaningful error, not just the final line.

## The game has low FPS

- Start with 8 chunks of render distance and 5–6 chunks of simulation distance.
- Temporarily turn off shaders and high-resolution resource packs.
- Reduce particles and entity distance.
- Close other GPU-heavy applications.
- Change one setting at a time and test in the same place.

## The world stutters during exploration

New terrain can take extra time to generate, especially with many biome and structure mods. Lower render distance temporarily and compare performance after the area has generated. On a server, administrators can consider controlled chunk pre-generation.

## A recipe or quest does not work

- Confirm your pack version.
- Search the recipe viewer for the item or result.
- Check the quest description and any prerequisites.
- Confirm the required item, station, or interaction is exactly what the quest expects.
- Check the changelog for recent recipe or progression changes.

## Report a bug well

If the issue is reproducible, open a [GitHub issue](https://github.com/Miso-Studio/Lunchtime-Cozy-Create-Farming/issues) and include your pack version, what happened, what you expected, and steps to reproduce. Add a relevant sanitized log or crash report when possible.

You can upload a log to [mclo.gs](https://mclo.gs/) and share the link. Remove private details first. Never post passwords, tokens, private IPs, or server addresses.

For general gameplay help, use [Discord](https://discord.gg/68yhDdFpnx). See the full [Performance Guide](../PERFORMANCE_GUIDE.md) for memory, server settings, and profiling.