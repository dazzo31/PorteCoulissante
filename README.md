# Porte Coulissante by Captain_Chaos
# PorteCoulissante

A modern Spigot plugin for creating working portcullises in Minecraft 1.21.8 and above.

## Legacy & Project Info
This plugin is a modern update of the classic PorteCoulissante Bukkit plugin ([CurseForge page](https://legacy.curseforge.com/minecraft/bukkit-plugins/portecoulissante)), originally by Pepijn Schmitz. It has been downloaded over 100,000 times and is loved for its simplicity and realism.

**Demo server:** mc.pepsoft.org — See working examples of PorteCoulissante and RetractableBridge in action.

**No commands required:** Just build your portcullis and power it with redstone!

**Stateless:** No data is saved to disk; everything is handled in-game.

**Redstone powered:** Flexible control using levers or redstone dust.

**Realistic movement:** The portcullis moves up and down like a real one, never disappears.

**Source code:** [Original SourceForge repo](https://sourceforge.net/p/portecoulissant/code/HEAD/tree/)

**Feedback:** Join the discussion and see more history on the [CurseForge comments](https://legacy.curseforge.com/minecraft/bukkit-plugins/portecoulissante#comments).

## Features
- Create realistic, moving portcullises using fences and iron bars
- Supports all modern fence types (Acacia, Birch, Crimson, Dark Oak, Jungle, Oak, Spruce, Warped)
- Customizable delays for hoisting and dropping
- Optional entity moving (entities on top of the portcullis are moved)
- Configurable power blocks and wall materials
- Sound effects for portcullis movement
- Fully compatible with Java 21 and Spigot 1.21.8

## Installation
1. Build the plugin using Maven (Java 21 required):
	```pwsh
	mvn clean package
	```
2. Copy the generated JAR from `target/PorteCullisante-1.2-SNAPSHOT.jar` to your server's `plugins` folder.
3. Start or restart your Spigot server.

## Usage
- Build the portcullis by stacking rows of fences (wood or iron), at least two wide and two high.
- Build the wall around it to contain it, leaving enough empty space above for movement.
- Power the portcullis by powering a block adjacent to it on either side (lever or redstone dust).
- When powered, the portcullis moves up slowly; when power is removed, it drops quickly.
- Decorate the gate with walls to make it look like it moves in a groove.
- Portcullises can be any size (at least 2x2), must be rectangular, and have no holes.
- The plugin supports diagonal portcullises and water/lava gates.

**See the [demo server](mc.pepsoft.org) for examples!**

## Configuration
Edit `plugins/PorteCoulissante/config.yml` to customize:
- `portcullisMaterials`: List of allowed block types for portcullises
- `powerBlocks`: List of allowed power block types
- `additionalWallMaterials`: List of allowed wall block types
- `hoistingDelay` and `droppingDelay`: Movement speed
- Sound effect URLs and settings

## Upgrading from older versions
- Numeric block IDs are no longer supported. Use material names (e.g., `OAK_FENCE`, `IRON_BARS`).
- Ensure your config files do not contain numbers like `85`, `101`, `113`.

## Known Issues
- If a chunk containing a moving portcullis is unloaded, it may stop mid-move. Power cycle to reset.
- Always ensure the portcullis is adjacent to a powered block for reliable operation.

## License
This project is licensed under the GNU GPL v3. See LICENSE for details.

## Credits
- Original author: Pepijn Schmitz
- Modernization and maintenance: Dolphindalt

## Support
Open an issue on GitHub for bug reports or feature requests.
This is a fork of Porte Coulissante by Captain_Chaos that is updated to work for paper-spigot 1.16.3.
>>>>>>> master
