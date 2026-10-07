# mc26-data — Minecraft 26.2

Game data of Minecraft: Java Edition 26.2 (protocol 776, data version
4903, Java 25), extracted from Mojang's server jar
(`823e2250d24b3ddac457a60c92a6a941943fcd6a`) by [mc26](https://github.com/mj41/mc26) `bef5fc043745` on
2026-10-07T17:28:39Z. Details in `_meta.json`.

| file | content |
|---|---|
| `registries.json` | every registry with numeric ids (Mojang's data generator report) |
| `blocks.json`, `block_properties.json` | block states and their properties |
| `block_behaviour.json` | per state the collision and outline shapes, the hardness, whether the drop needs the right tool, the fluid; per block the friction, speed and jump factors, explosion resistance — what a client needs to move, dig and place |
| `items.json` | per-item stack size and name, and every default component in its network encoding (`wire`, base64) |
| `entities.json`, `block_entities.json`, `biomes.json` | entity dimensions, block entity types, biome order |
| `packets.json`, `packet_schema.json` | packet ids per state and the typed wire layout of every packet |
| `components.json`, `component_schema.json` | item data component types and their wire schema |
| `commands.json`, `datapack.json`, `version.json` | command tree, built-in datapack list, version facts |
| `nbt_schema.json`, `save_schema.json` | the NBT shape of the registries sent at configuration time and of the save formats (rendered as `docs/registries.md` and `docs/save.md`) |
| `data/` | the vanilla data pack the data generator writes: every recipe, loot table, tag, advancement, the worldgen, the trades, as files |
| `lang/*.json` | every language file |
| `docs/*.md` | the same, for a reader: [protocol.md](docs/protocol.md) (the frame, the primitives, the node kinds), [packets.md](docs/packets.md), [components.md](docs/components.md), [registries.md](docs/registries.md) |

JSON and its documentation, no code; one branch per Minecraft version, tags `v0.<YYN>.<n>` pin an
extraction. The README on `main` lists the branches.
