# mc26-data

Minecraft: Java Edition game data as JSON, extracted from Mojang's unobfuscated server
jars by [mc26-data-gen](../mc26-data-gen): registries, packet ids and their wire schema, data
components and their schema, items, blocks and block states, entities, block entities, biomes and
the language files, plus `_meta.json` (Minecraft version, data version, protocol, jar
checksum, extractor commit).

- One branch per Minecraft release: `mc-26.1`, `mc-26.2`, … `main` holds only this README.
- Tags `v0.<YYN>.<n>` pin an extraction (`v0.262.0` is Minecraft 26.2; `n` counts re-extractions
  with a newer extractor).
- JSON only, no code: fetch by tag, raw URL or submodule from any language.
- Snapshots and pre-releases live in [mc26-data-pre](../mc26-data-pre).

| branch | Minecraft | protocol | latest tag |
|---|---|---|---|
| `mc-26.2` | 26.2 | 776 | — |
| `mc-26.1` | 26.1 | 775 | — |
