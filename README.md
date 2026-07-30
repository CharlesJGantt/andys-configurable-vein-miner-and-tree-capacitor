# Andy's Configurable Vein Miner and Tree Capacitor

[![Andy's Configurable Vein Miner and Tree Capacitor — available on CurseForge](./Andys-Configurable-Vein-Miner-Tree-Capacitor-Hero.jpg)](https://www.curseforge.com/minecraft-bedrock/addons/andys-configurable-vein-miner-and-tree-capacitor)

Mine connected blocks and fell trees by crouching while you break the first block. Every option starts **off**, so the world owner decides exactly which blocks the add-on can affect.

## Features

- Crouch-to-activate vein mining and tree felling
- 25 configuration switches, all disabled by default
- Ores, Tree Logs, and Leaves category switches
- 22 individually controlled terrain and building-material groups
- Pickaxe, axe, shovel, hoe, and shears support
- One durability use per additional block in Survival
- Unbreaking, Fortune, Silk Touch, and custom loot-table support
- One matching material break sound per additional block
- Fast overlapping break waves with randomized 1–3 game-tick branch timing
- Ores and individual materials connect through faces, edges, and corners
- Exact-type logs connect through faces, edges, and corners to catch side branches
- Exact-type leaves remain face-connected and bounded to prevent canopy jumping
- Stone/deepslate and lit/unlit versions of the same ore connect
- Drops gather at the first broken block
- Gathered drops scatter upward and visibly fall at the first broken block
- Live gravity-block tracking keeps sand and concrete powder in the wave while they fall
- Optional All In One Tool and Core Craft compatibility
- No required resource pack or optional compatibility dependency

## Requirements

- Minecraft Bedrock Edition 1.26.30 or newer
- The behavior pack activated on the world
- At least one setting enabled

## Install

1. Download `Andys Configurable Vein Miner and Tree Capacitor 2.0.4.mcaddon`.
2. Open the file with Minecraft.
3. Wait for the successful-import message.
4. Create a world or edit an existing world.
5. Open **Behavior Packs**, select **My Packs**, and activate **Andy's Configurable Vein Miner and Tree Capacitor**.
6. Select the gear/settings button for the active pack.
7. Turn on the blocks you want the add-on to affect.
8. Enter the world.

All switches are intentionally off after installation.

## Update

1. Leave Minecraft before importing the new file.
2. Open the newest `.mcaddon`.
3. Let Minecraft replace the installed pack.
4. Confirm version **2.0.4** is active on the world.
5. Recheck the behavior-pack settings after updating.

The pack keeps the same identity as previous releases, so 2.0.4 replaces the installed version instead of appearing as a second pack.

## Use

1. Enable the relevant block setting.
2. Hold the correct tool.
3. Crouch.
4. Break one configured block.
5. Remain crouched while the connected blocks are processed.

Release crouch or change tools to stop the operation.

## Configuration

Open the active behavior pack's settings from the world editor. A visible `|` means the switch is on; `O` means it is off.

### Category switches

| Setting | Blocks | Tool |
|---|---|---|
| Ores | Vanilla ores and compatible custom ores | Pickaxe |
| Tree Logs | Touching logs of the exact same block type, including diagonal branches | Axe |
| Leaves | Face-connected leaves of the exact same type, including Nether tree foliage | Shears |

When Tree Logs and Leaves are both enabled, chopping a connected tree also clears its attached leaves. Those attached leaves do not consume extra axe durability.

### Individual switches

| Setting | Included blocks | Tool |
|---|---|---|
| Mud | Mud and compatible Core Craft mud | Shovel |
| Clay | Clay blocks | Shovel |
| Coarse Dirt | Coarse dirt | Shovel |
| Sand | Sand and red sand; suspicious sand is excluded | Shovel |
| Concrete Powder | All 16 concrete-powder colors | Shovel |
| Concrete | All 16 solid-concrete colors | Pickaxe |
| Diorite | Diorite and polished diorite | Pickaxe |
| Andesite | Andesite and polished andesite | Pickaxe |
| Granite | Granite and polished granite | Pickaxe |
| Tuff | Tuff, polished tuff, tuff bricks, and chiseled variants | Pickaxe |
| Basalt | Basalt and smooth basalt | Pickaxe |
| Soul Sand | Soul sand | Shovel |
| Soul Soil | Soul soil | Shovel |
| Terracotta | Normal, colored, and glazed terracotta | Pickaxe |
| Glowstone | Glowstone | Pickaxe |
| Netherrack | Netherrack | Pickaxe |
| Sculk | Sculk blocks, veins, sensors, catalysts, and shriekers | Hoe |
| Sulfur | Sulfur and its polished, brick, and chiseled variants | Pickaxe |
| Dripstone Blocks | Dripstone blocks | Pickaxe |
| Cinnabar | Cinnabar and its polished, brick, and chiseled variants | Pickaxe |
| Corals | Living and dead coral blocks, corals, fans, and wall fans | Pickaxe |
| Moss | Moss blocks and carpets with a hoe; hanging moss with shears | Hoe or shears |

## Tool and durability behavior

Minecraft handles the first block normally. The add-on applies one additional durability use for each additional block it removes.

- An unenchanted iron shovel provides 250 total durability uses, including the first block.
- Unbreaking is evaluated separately for every additional block.
- Unbreakable custom tools do not lose durability.
- The operation stops as soon as the held tool breaks.
- Creative mode does not consume durability or create Survival drops.

Minecraft's own block loot tables are used for additional blocks. This preserves Fortune, Silk Touch, custom drops, and tool-based drop conditions.

## Optional compatibility

### All In One Tool

The 26.30 All In One Tool items are recognized as universal pickaxe, axe, shovel, and hoe tools. Their current durability and enchantments are used directly.

AIOTs do not replace shears. Use shears to start vein-mining leaves or hanging moss.

### Core Craft

Core Craft 1.2.1 compatibility includes:

- Ruby Ore and Deepslate Ruby Ore
- Voidshard Ore
- Palm, end-spire, thin, hollow, and other properly named or tagged tree blocks
- Core Craft leaves and moss
- Core Craft axes and pickaxes that publish the standard Bedrock tool tags

Core Craft is optional. Its content is not bundled with this add-on.

## Connected-block behavior

- Every enabled category and individual material uses the same wave timing, per-block sound, durability, and gathered-drop rules.
- Sand and concrete powder refresh their connected frontier from live block positions, follow displaced blocks down their original columns, and retry briefly while falling blocks settle.
- Ores and individual configured materials connect through faces, edges, and corners.
- Ordinary individual blocks connect only to the same exact block type.
- Related stone/deepslate and lit/unlit ore variants connect as one ore family.
- Tree logs connect through faces, edges, and corners, but only to the exact same block type.
- Leaves connect face-to-face and only to the exact same leaf type.
- Attached tree leaves are limited to a bounded connected canopy around the felled logs.
- A single operation can remove up to 512 additional blocks.
- Connected branches run concurrently as expanding waves.
- Each branch uses randomized 1–3 game-tick timing, while its next connected frontier begins one tick later.
- The first visible wave normally begins within 2–4 game ticks.
- Every additional block plays a matching material break sound.

## Troubleshooting

### The add-on does nothing

Check all of the following:

1. The behavior pack is active on the world.
2. Its settings show at least one switch as `|`.
3. You are crouching while the first block breaks.
4. You are holding the correct tool.
5. The block belongs to the enabled setting.

### Only one block breaks

- Remain crouched until the operation starts.
- For ores and individual materials, confirm that neighboring blocks touch by a face, edge, or corner.
- For logs, confirm that blocks of the exact same type touch by a face, edge, or corner.
- For leaves, confirm that blocks of the exact same type touch face-to-face.
- Confirm that the correct setting is on.
- For ores, confirm the neighboring block belongs to the same ore family.

### Leaves do not work

- Turn on **Leaves**.
- Use shears when starting on leaves.
- Crouch before the leaf block breaks.
- AIOTs are not treated as shears.

### Mud, clay, sand, or concrete powder does not work

Use a shovel and enable that exact setting. These blocks are not controlled by the Ores switch.

### Granite, tuff, concrete, or another hard block does not work

Use a pickaxe and enable that exact setting. These blocks are not controlled by the Ores switch.

### Moss or sculk does not work

Use a hoe for ground moss and sculk. Use shears for hanging moss.

### Trees fall but leaves remain

Turn on both **Tree Logs** and **Leaves**. Tree Logs alone removes only the trunk.

### The tool loses durability quickly

This is expected for large connected areas. Every additional block costs one tool use unless Unbreaking prevents that use. Attached leaves cleared while felling a tree are the exception.

### Import says the file is invalid

1. Confirm the filename ends in `.mcaddon`.
2. Remove any `.zip` extension added by the browser.
3. Download the file again instead of opening a partial download.
4. Close Minecraft, reopen it, and import again.
5. Do not extract or recompress the package.

### An older version still appears

Delete the older installed copy from **Settings → Storage → Behavior Packs**, restart Minecraft, and import version 2.0.4 again.

## Support

- Website: [AndyTheMakerMC.xyz](https://AndyTheMakerMC.xyz)
- When reporting a problem, include the Minecraft version, add-on version, enabled switches, held tool, block type, and whether the issue occurs in a new test world.

## Ownership and license

Copyright © Andy. All rights reserved.

You may use the unmodified add-on in personal worlds, multiplayer worlds, Realms, servers, videos, livestreams, reviews, tutorials, and showcases.

Do not redistribute the `.mcaddon`, scripts, artwork, or modified versions; sell or repackage the add-on; publish mirrors; or claim the project as your own without written permission.

Minecraft is a trademark of Microsoft. This project is not affiliated with or endorsed by Microsoft or Mojang.

The promotional logo and hero are AI-assisted illustrative artwork. They are not in-game screenshots and do not add custom tool, ore, block, or tree textures.
